>   net.minecraft.util.DirectoryLock \
>   net.minecraft.world.level.chunk.storage.RegionFile \
>   net.minecraft.world.level.chunk.storage.RegionFileStorage \
>   net.minecraft.world.level.chunk.storage.ChunkStorage \
>   net.minecraft.world.level.chunk.storage.SimpleRegionStorage \
>   net.minecraft.world.level.chunk.storage.IOWorker \
>   net.minecraft.world.level.chunk.storage.EntityStorage \
>   net.minecraft.world.level.chunk.storage.SectionStorage \
>   net.minecraft.world.entity.ai.village.poi.PoiManager
> do
>   echo
>   echo "========== $CLASS =========="
>
>   if javap -classpath "$JAR" -p "$CLASS" >/dev/null 2>&1; then
>     echo "--- API ---"
>     javap -classpath "$JAR" -p "$CLASS"
>
>     echo "--- FILE I/O BYTECODE ---"
>     javap -classpath "$JAR" -p -c "$CLASS" |
>       grep -n -E -B 3 -A 5 \
>       'FileChannel.open|StandardOpenOption|RandomAccessFile|Files\.|createDirectories|createTempFile|deleteIfExists|move\(|force\(|write\(|read\(|flush\(|synchronize\(|close\(|padToFullSector|RegionFile\(' \
>       || true
>   else
>     echo "CLASS_NOT_FOUND: $CLASS"
>   fi
> done | tee /tmp/lss-offline-storage-bytecode-audit.txt

========== net.minecraft.util.DirectoryLock ==========
--- API ---
Compiled from "DirectoryLock.java"
public class net.minecraft.util.DirectoryLock implements java.lang.AutoCloseable {
  public static final java.lang.String LOCK_FILE;
  private final java.nio.channels.FileChannel lockFile;
  private final java.nio.channels.FileLock lock;
  private static final java.nio.ByteBuffer DUMMY;
  public static net.minecraft.util.DirectoryLock create(java.nio.file.Path) throws java.io.IOException;
  private net.minecraft.util.DirectoryLock(java.nio.channels.FileChannel, java.nio.channels.FileLock);
  public void close() throws java.io.IOException;
  public boolean isValid();
  public static boolean isLocked(java.nio.file.Path) throws java.io.IOException;
  static {};
}
--- FILE I/O BYTECODE ---
15-       3: invokeinterface #3,  2            // InterfaceMethod java/nio/file/Path.resolve:(Ljava/lang/String;)Ljava/nio/file/Path;
16-       8: astore_1
17-       9: aload_0
18:      10: invokestatic  #9                  // Method net/minecraft/FileUtil.createDirectoriesSafe:(Ljava/nio/file/Path;)V
19-      13: aload_1
20-      14: iconst_2
21-      15: anewarray     #15                 // class java/nio/file/OpenOption
22-      18: dup
23-      19: iconst_0
24:      20: getstatic     #17                 // Field java/nio/file/StandardOpenOption.CREATE:Ljava/nio/file/StandardOpenOption;
25-      23: aastore
26-      24: dup
27-      25: iconst_1
28:      26: getstatic     #23                 // Field java/nio/file/StandardOpenOption.WRITE:Ljava/nio/file/StandardOpenOption;
29-      29: aastore
30:      30: invokestatic  #26                 // Method java/nio/channels/FileChannel.open:(Ljava/nio/file/Path;[Ljava/nio/file/OpenOption;)Ljava/nio/channels/FileChannel;
31-      33: astore_2
32-      34: aload_2
33-      35: getstatic     #32                 // Field DUMMY:Ljava/nio/ByteBuffer;
34-      38: invokevirtual #38                 // Method java/nio/ByteBuffer.duplicate:()Ljava/nio/ByteBuffer;
35-      41: invokevirtual #44                 // Method java/nio/channels/FileChannel.write:(Ljava/nio/ByteBuffer;)I
--
78-      11: putfield      #84                 // Field lock:Ljava/nio/channels/FileLock;
79-      14: return
80-
81:  public void close() throws java.io.IOException;
82-    Code:
83-       0: aload_0
84-       1: getfield      #84                 // Field lock:Ljava/nio/channels/FileLock;
85-       4: invokevirtual #88                 // Method java/nio/channels/FileLock.isValid:()Z
86-       7: ifeq          17
--
128-      11: anewarray     #15                 // class java/nio/file/OpenOption
129-      14: dup
130-      15: iconst_0
131:      16: getstatic     #23                 // Field java/nio/file/StandardOpenOption.WRITE:Ljava/nio/file/StandardOpenOption;
132-      19: aastore
133:      20: invokestatic  #26                 // Method java/nio/channels/FileChannel.open:(Ljava/nio/file/Path;[Ljava/nio/file/OpenOption;)Ljava/nio/channels/FileChannel;
134-      23: astore_3
135-      24: aload_3
136-      25: invokevirtual #52                 // Method java/nio/channels/FileChannel.tryLock:()Ljava/nio/channels/FileLock;
137-      28: astore        4
138-      30: aload         4

========== net.minecraft.world.level.chunk.storage.RegionFile ==========
--- API ---
Compiled from "RegionFile.java"
public class net.minecraft.world.level.chunk.storage.RegionFile implements java.lang.AutoCloseable {
  private static final org.slf4j.Logger LOGGER;
  private static final int SECTOR_BYTES;
  protected static final int SECTOR_INTS;
  private static final int CHUNK_HEADER_SIZE;
  private static final int HEADER_OFFSET;
  private static final java.nio.ByteBuffer PADDING_BUFFER;
  private static final java.lang.String EXTERNAL_FILE_EXTENSION;
  private static final int EXTERNAL_STREAM_FLAG;
  private static final int EXTERNAL_CHUNK_THRESHOLD;
  private static final int CHUNK_NOT_PRESENT;
  final net.minecraft.world.level.chunk.storage.RegionStorageInfo info;
  private final java.nio.file.Path path;
  private final java.nio.channels.FileChannel file;
  private final java.nio.file.Path externalFileDir;
  final net.minecraft.world.level.chunk.storage.RegionFileVersion version;
  private final java.nio.ByteBuffer header;
  private final java.nio.IntBuffer offsets;
  private final java.nio.IntBuffer timestamps;
  protected final net.minecraft.world.level.chunk.storage.RegionBitmap usedSectors;
  public net.minecraft.world.level.chunk.storage.RegionFile(net.minecraft.world.level.chunk.storage.RegionStorageInfo, java.nio.file.Path, java.nio.file.Path, boolean) throws java.io.IOException;
  public net.minecraft.world.level.chunk.storage.RegionFile(net.minecraft.world.level.chunk.storage.RegionStorageInfo, java.nio.file.Path, java.nio.file.Path, net.minecraft.world.level.chunk.storage.RegionFileVersion, boolean) throws java.io.IOException;
  public java.nio.file.Path getPath();
  private java.nio.file.Path getExternalChunkPath(net.minecraft.world.level.ChunkPos);
  public synchronized java.io.DataInputStream getChunkDataInputStream(net.minecraft.world.level.ChunkPos) throws java.io.IOException;
  private static int getTimestamp();
  private static boolean isExternalStreamChunk(byte);
  private static byte getExternalChunkVersion(byte);
  private java.io.DataInputStream createChunkInputStream(net.minecraft.world.level.ChunkPos, byte, java.io.InputStream) throws java.io.IOException;
  private java.io.DataInputStream createExternalChunkInputStream(net.minecraft.world.level.ChunkPos, byte) throws java.io.IOException;
  private static java.io.ByteArrayInputStream createStream(java.nio.ByteBuffer, int);
  private int packSectorOffset(int, int);
  private static int getNumSectors(int);
  private static int getSectorNumber(int);
  private static int sizeToSectors(int);
  public boolean doesChunkExist(net.minecraft.world.level.ChunkPos);
  public java.io.DataOutputStream getChunkDataOutputStream(net.minecraft.world.level.ChunkPos) throws java.io.IOException;
  public void flush() throws java.io.IOException;
  public void clear(net.minecraft.world.level.ChunkPos) throws java.io.IOException;
  protected synchronized void write(net.minecraft.world.level.ChunkPos, java.nio.ByteBuffer) throws java.io.IOException;
  private java.nio.ByteBuffer createExternalStub();
  private net.minecraft.world.level.chunk.storage.RegionFile$CommitOp writeToExternalFile(java.nio.file.Path, java.nio.ByteBuffer) throws java.io.IOException;
  private void writeHeader() throws java.io.IOException;
  private int getOffset(net.minecraft.world.level.ChunkPos);
  public boolean hasChunk(net.minecraft.world.level.ChunkPos);
  private static int getOffsetIndex(net.minecraft.world.level.ChunkPos);
  public void close() throws java.io.IOException;
  private void padToFullSector() throws java.io.IOException;
  private static void lambda$writeToExternalFile$1(java.nio.file.Path, java.nio.file.Path) throws java.io.IOException;
  private void lambda$write$0(net.minecraft.world.level.ChunkPos) throws java.io.IOException;
  static {};
}
--- FILE I/O BYTECODE ---
38-
39-  protected final net.minecraft.world.level.chunk.storage.RegionBitmap usedSectors;
40-
41:  public net.minecraft.world.level.chunk.storage.RegionFile(net.minecraft.world.level.chunk.storage.RegionStorageInfo, java.nio.file.Path, java.nio.file.Path, boolean) throws java.io.IOException;
42-    Code:
43-       0: aload_0
44-       1: aload_1
45-       2: aload_2
46-       3: aload_3
--
49-       9: invokespecial #7                  // Method "<init>":(Lnet/minecraft/world/level/chunk/storage/RegionStorageInfo;Ljava/nio/file/Path;Ljava/nio/file/Path;Lnet/minecraft/world/level/chunk/storage/RegionFileVersion;Z)V
50-      12: return
51-
52:  public net.minecraft.world.level.chunk.storage.RegionFile(net.minecraft.world.level.chunk.storage.RegionStorageInfo, java.nio.file.Path, java.nio.file.Path, net.minecraft.world.level.chunk.storage.RegionFileVersion, boolean) throws java.io.IOException;
53-    Code:
54-       0: aload_0
55-       1: invokespecial #13                 // Method java/lang/Object."<init>":()V
56-       4: aload_0
57-       5: sipush        8192
--
74-      41: aload_3
75-      42: iconst_0
76-      43: anewarray     #47                 // class java/nio/file/LinkOption
77:      46: invokestatic  #49                 // Method java/nio/file/Files.isDirectory:(Ljava/nio/file/Path;[Ljava/nio/file/LinkOption;)Z
78-      49: ifne          74
79-      52: new           #55                 // class java/lang/IllegalArgumentException
80-      55: dup
81-      56: aload_3
82-      57: invokeinterface #57,  1           // InterfaceMethod java/nio/file/Path.toAbsolutePath:()Ljava/nio/file/Path;
--
115-     131: anewarray     #99                 // class java/nio/file/OpenOption
116-     134: dup
117-     135: iconst_0
118:     136: getstatic     #101                // Field java/nio/file/StandardOpenOption.CREATE:Ljava/nio/file/StandardOpenOption;
119-     139: aastore
120-     140: dup
121-     141: iconst_1
122:     142: getstatic     #107                // Field java/nio/file/StandardOpenOption.READ:Ljava/nio/file/StandardOpenOption;
123-     145: aastore
124-     146: dup
125-     147: iconst_2
126:     148: getstatic     #110                // Field java/nio/file/StandardOpenOption.WRITE:Ljava/nio/file/StandardOpenOption;
127-     151: aastore
128-     152: dup
129-     153: iconst_3
130:     154: getstatic     #113                // Field java/nio/file/StandardOpenOption.DSYNC:Ljava/nio/file/StandardOpenOption;
131-     157: aastore
132:     158: invokestatic  #116                // Method java/nio/channels/FileChannel.open:(Ljava/nio/file/Path;[Ljava/nio/file/OpenOption;)Ljava/nio/channels/FileChannel;
133-     161: putfield      #122                // Field file:Ljava/nio/channels/FileChannel;
134-     164: goto          197
135-     167: aload_0
136-     168: aload_2
137-     169: iconst_3
138-     170: anewarray     #99                 // class java/nio/file/OpenOption
139-     173: dup
140-     174: iconst_0
141:     175: getstatic     #101                // Field java/nio/file/StandardOpenOption.CREATE:Ljava/nio/file/StandardOpenOption;
142-     178: aastore
143-     179: dup
144-     180: iconst_1
145:     181: getstatic     #107                // Field java/nio/file/StandardOpenOption.READ:Ljava/nio/file/StandardOpenOption;
146-     184: aastore
147-     185: dup
148-     186: iconst_2
149:     187: getstatic     #110                // Field java/nio/file/StandardOpenOption.WRITE:Ljava/nio/file/StandardOpenOption;
150-     190: aastore
151:     191: invokestatic  #116                // Method java/nio/channels/FileChannel.open:(Ljava/nio/file/Path;[Ljava/nio/file/OpenOption;)Ljava/nio/channels/FileChannel;
152-     194: putfield      #122                // Field file:Ljava/nio/channels/FileChannel;
153-     197: aload_0
154-     198: getfield      #31                 // Field usedSectors:Lnet/minecraft/world/level/chunk/storage/RegionBitmap;
155-     201: iconst_0
156-     202: iconst_2
--
180-     251: invokestatic  #140                // Method java/lang/Integer.valueOf:(I)Ljava/lang/Integer;
181-     254: invokeinterface #145,  4          // InterfaceMethod org/slf4j/Logger.warn:(Ljava/lang/String;Ljava/lang/Object;Ljava/lang/Object;)V
182-     259: aload_2
183:     260: invokestatic  #151                // Method java/nio/file/Files.size:(Ljava/nio/file/Path;)J
184-     263: lstore        7
185-     265: iconst_0
186-     266: istore        9
187-     268: iload         9
188-     270: sipush        1024
--
537-       6: aload_3
538-       7: iconst_0
539-       8: anewarray     #47                 // class java/nio/file/LinkOption
540:      11: invokestatic  #318                // Method java/nio/file/Files.isRegularFile:(Ljava/nio/file/Path;[Ljava/nio/file/LinkOption;)Z
541-      14: ifne          31
542-      17: getstatic     #134                // Field LOGGER:Lorg/slf4j/Logger;
543-      20: ldc_w         #321                // String External chunk path {} is not file
544-      23: aload_3
545-      24: invokeinterface #299,  3          // InterfaceMethod org/slf4j/Logger.error:(Ljava/lang/String;Ljava/lang/Object;)V
--
551-      34: aload_3
552-      35: iconst_0
553-      36: anewarray     #99                 // class java/nio/file/OpenOption
554:      39: invokestatic  #323                // Method java/nio/file/Files.newInputStream:(Ljava/nio/file/Path;[Ljava/nio/file/OpenOption;)Ljava/io/InputStream;
555-      42: invokevirtual #263                // Method createChunkInputStream:(Lnet/minecraft/world/level/ChunkPos;BLjava/io/InputStream;)Ljava/io/DataInputStream;
556-      45: areturn
557-
558-  private static java.io.ByteArrayInputStream createStream(java.nio.ByteBuffer, int);
559-    Code:
--
660-      99: invokevirtual #314                // Method getExternalChunkPath:(Lnet/minecraft/world/level/ChunkPos;)Ljava/nio/file/Path;
661-     102: iconst_0
662-     103: anewarray     #47                 // class java/nio/file/LinkOption
663:     106: invokestatic  #318                // Method java/nio/file/Files.isRegularFile:(Ljava/nio/file/Path;[Ljava/nio/file/LinkOption;)Z
664-     109: ifne          155
665-     112: iconst_0
666-     113: ireturn
667-     114: iload         7
668-     116: invokestatic  #339                // Method net/minecraft/world/level/chunk/storage/RegionFileVersion.isValidVersion:(I)Z
--
716-      20: invokespecial #355                // Method java/io/DataOutputStream."<init>":(Ljava/io/OutputStream;)V
717-      23: areturn
718-
719:  public void flush() throws java.io.IOException;
720-    Code:
721-       0: aload_0
722-       1: getfield      #122                // Field file:Ljava/nio/channels/FileChannel;
723-       4: iconst_1
724-       5: invokevirtual #358                // Method java/nio/channels/FileChannel.force:(Z)V
--
753-      44: aload_0
754-      45: aload_1
755-      46: invokevirtual #314                // Method getExternalChunkPath:(Lnet/minecraft/world/level/ChunkPos;)Ljava/nio/file/Path;
756:      49: invokestatic  #370                // Method java/nio/file/Files.deleteIfExists:(Ljava/nio/file/Path;)Z
757-      52: pop
758-      53: aload_0
759-      54: getfield      #31                 // Field usedSectors:Lnet/minecraft/world/level/chunk/storage/RegionBitmap;
760-      57: iload_3
761-      58: invokestatic  #159                // Method getSectorNumber:(I)I
--
764-      65: invokevirtual #374                // Method net/minecraft/world/level/chunk/storage/RegionBitmap.free:(II)V
765-      68: return
766-
767:  protected synchronized void write(net.minecraft.world.level.ChunkPos, java.nio.ByteBuffer) throws java.io.IOException;
768-    Code:
769-       0: aload_1
770-       1: invokestatic  #361                // Method getOffsetIndex:(Lnet/minecraft/world/level/ChunkPos;)I
771-       4: istore_3
772-       5: aload_0
--
914-       7: aconst_null
915-       8: iconst_0
916-       9: anewarray     #417                // class java/nio/file/attribute/FileAttribute
917:      12: invokestatic  #419                // Method java/nio/file/Files.createTempFile:(Ljava/nio/file/Path;Ljava/lang/String;Ljava/lang/String;[Ljava/nio/file/attribute/FileAttribute;)Ljava/nio/file/Path;
918-      15: astore_3
919-      16: aload_3
920-      17: iconst_2
921-      18: anewarray     #99                 // class java/nio/file/OpenOption
922-      21: dup
923-      22: iconst_0
924:      23: getstatic     #101                // Field java/nio/file/StandardOpenOption.CREATE:Ljava/nio/file/StandardOpenOption;
925-      26: aastore
926-      27: dup
927-      28: iconst_1
928:      29: getstatic     #110                // Field java/nio/file/StandardOpenOption.WRITE:Ljava/nio/file/StandardOpenOption;
929-      32: aastore
930:      33: invokestatic  #116                // Method java/nio/channels/FileChannel.open:(Ljava/nio/file/Path;[Ljava/nio/file/OpenOption;)Ljava/nio/channels/FileChannel;
931-      36: astore        4
932-      38: aload_2
933-      39: iconst_5
934-      40: invokevirtual #93                 // Method java/nio/ByteBuffer.position:(I)Ljava/nio/ByteBuffer;
935-      43: pop
--
1010-      11: iadd
1011-      12: ireturn
1012-
1013:  public void close() throws java.io.IOException;
1014-    Code:
1015-       0: aload_0
1016:       1: invokevirtual #444                // Method padToFullSector:()V
1017-       4: aload_0
1018-       5: getfield      #122                // Field file:Ljava/nio/channels/FileChannel;
1019-       8: iconst_1
1020-       9: invokevirtual #358                // Method java/nio/channels/FileChannel.force:(Z)V
1021-      12: aload_0
--
1053-           0     4    35   any
1054-          36    44    54   any
1055-
1056:  private void padToFullSector() throws java.io.IOException;
1057-    Code:
1058-       0: aload_0
1059-       1: getfield      #122                // Field file:Ljava/nio/channels/FileChannel;
1060-       4: invokevirtual #447                // Method java/nio/channels/FileChannel.size:()J
1061-       7: l2i
--
1096-       7: iconst_0
1097-       8: getstatic     #457                // Field java/nio/file/StandardCopyOption.REPLACE_EXISTING:Ljava/nio/file/StandardCopyOption;
1098-      11: aastore
1099:      12: invokestatic  #463                // Method java/nio/file/Files.move:(Ljava/nio/file/Path;Ljava/nio/file/Path;[Ljava/nio/file/CopyOption;)Ljava/nio/file/Path;
1100-      15: pop
1101-      16: return
1102-
1103-  private void lambda$write$0(net.minecraft.world.level.ChunkPos) throws java.io.IOException;
1104-    Code:
1105-       0: aload_0
1106-       1: aload_1
1107-       2: invokevirtual #314                // Method getExternalChunkPath:(Lnet/minecraft/world/level/ChunkPos;)Ljava/nio/file/Path;
1108:       5: invokestatic  #370                // Method java/nio/file/Files.deleteIfExists:(Ljava/nio/file/Path;)Z
1109-       8: pop
1110-       9: return
1111-
1112-  static {};
1113-    Code:

========== net.minecraft.world.level.chunk.storage.RegionFileStorage ==========
--- API ---
Compiled from "RegionFileStorage.java"
public final class net.minecraft.world.level.chunk.storage.RegionFileStorage implements java.lang.AutoCloseable {
  public static final java.lang.String ANVIL_EXTENSION;
  private static final int MAX_CACHE_SIZE;
  private final it.unimi.dsi.fastutil.longs.Long2ObjectLinkedOpenHashMap<net.minecraft.world.level.chunk.storage.RegionFile> regionCache;
  private final net.minecraft.world.level.chunk.storage.RegionStorageInfo info;
  private final java.nio.file.Path folder;
  private final boolean sync;
  net.minecraft.world.level.chunk.storage.RegionFileStorage(net.minecraft.world.level.chunk.storage.RegionStorageInfo, java.nio.file.Path, boolean);
  private net.minecraft.world.level.chunk.storage.RegionFile getRegionFile(net.minecraft.world.level.ChunkPos) throws java.io.IOException;
  public net.minecraft.nbt.CompoundTag read(net.minecraft.world.level.ChunkPos) throws java.io.IOException;
  public void scanChunk(net.minecraft.world.level.ChunkPos, net.minecraft.nbt.StreamTagVisitor) throws java.io.IOException;
  protected void write(net.minecraft.world.level.ChunkPos, net.minecraft.nbt.CompoundTag) throws java.io.IOException;
  public void close() throws java.io.IOException;
  public void flush() throws java.io.IOException;
  public net.minecraft.world.level.chunk.storage.RegionStorageInfo info();
}
--- FILE I/O BYTECODE ---
32-      27: putfield      #24                 // Field info:Lnet/minecraft/world/level/chunk/storage/RegionStorageInfo;
33-      30: return
34-
35:  private net.minecraft.world.level.chunk.storage.RegionFile getRegionFile(net.minecraft.world.level.ChunkPos) throws java.io.IOException;
36-    Code:
37-       0: aload_1
38-       1: invokevirtual #28                 // Method net/minecraft/world/level/ChunkPos.getRegionX:()I
39-       4: aload_1
40-       5: invokevirtual #34                 // Method net/minecraft/world/level/ChunkPos.getRegionZ:()I
--
62-      56: invokevirtual #54                 // Method net/minecraft/world/level/chunk/storage/RegionFile.close:()V
63-      59: aload_0
64-      60: getfield      #16                 // Field folder:Ljava/nio/file/Path;
65:      63: invokestatic  #57                 // Method net/minecraft/FileUtil.createDirectoriesSafe:(Ljava/nio/file/Path;)V
66-      66: aload_0
67-      67: getfield      #16                 // Field folder:Ljava/nio/file/Path;
68-      70: aload_1
69-      71: invokevirtual #28                 // Method net/minecraft/world/level/ChunkPos.getRegionX:()I
70-      74: aload_1
--
92-     124: aload         6
93-     126: areturn
94-
95:  public net.minecraft.nbt.CompoundTag read(net.minecraft.world.level.ChunkPos) throws java.io.IOException;
96-    Code:
97-       0: aload_0
98-       1: aload_1
99-       2: invokevirtual #80                 // Method getRegionFile:(Lnet/minecraft/world/level/ChunkPos;)Lnet/minecraft/world/level/chunk/storage/RegionFile;
100-       5: astore_2
--
179-          13    27    40   Class java/lang/Throwable
180-          47    52    55   Class java/lang/Throwable
181-
182:  protected void write(net.minecraft.world.level.ChunkPos, net.minecraft.nbt.CompoundTag) throws java.io.IOException;
183-    Code:
184-       0: aload_0
185-       1: aload_1
186-       2: invokevirtual #80                 // Method getRegionFile:(Lnet/minecraft/world/level/ChunkPos;)Lnet/minecraft/world/level/chunk/storage/RegionFile;
187-       5: astore_3
--
221-          25    31    44   Class java/lang/Throwable
222-          51    56    59   Class java/lang/Throwable
223-
224:  public void close() throws java.io.IOException;
225-    Code:
226-       0: new           #128                // class net/minecraft/util/ExceptionCollector
227-       3: dup
228-       4: invokespecial #130                // Method net/minecraft/util/ExceptionCollector."<init>":()V
229-       7: astore_1
--
254-       from    to  target type
255-          40    44    47   Class java/io/IOException
256-
257:  public void flush() throws java.io.IOException;
258-    Code:
259-       0: aload_0
260-       1: getfield      #10                 // Field regionCache:Lit/unimi/dsi/fastutil/longs/Long2ObjectLinkedOpenHashMap;
261-       4: invokevirtual #131                // Method it/unimi/dsi/fastutil/longs/Long2ObjectLinkedOpenHashMap.values:()Lit/unimi/dsi/fastutil/objects/ObjectCollection;
262-       7: invokeinterface #135,  1          // InterfaceMethod it/unimi/dsi/fastutil/objects/ObjectCollection.iterator:()Lit/unimi/dsi/fastutil/objects/ObjectIterator;

========== net.minecraft.world.level.chunk.storage.ChunkStorage ==========
--- API ---
Compiled from "ChunkStorage.java"
public class net.minecraft.world.level.chunk.storage.ChunkStorage implements java.lang.AutoCloseable {
  public static final int LAST_MONOLYTH_STRUCTURE_DATA_VERSION;
  private final net.minecraft.world.level.chunk.storage.IOWorker worker;
  protected final com.mojang.datafixers.DataFixer fixerUpper;
  private volatile net.minecraft.world.level.levelgen.structure.LegacyStructureDataHandler legacyStructureHandler;
  public net.minecraft.world.level.chunk.storage.ChunkStorage(net.minecraft.world.level.chunk.storage.RegionStorageInfo, java.nio.file.Path, com.mojang.datafixers.DataFixer, boolean);
  public boolean isOldChunkAround(net.minecraft.world.level.ChunkPos, int);
  public net.minecraft.nbt.CompoundTag upgradeChunkTag(net.minecraft.resources.ResourceKey<net.minecraft.world.level.Level>, java.util.function.Supplier<net.minecraft.world.level.storage.DimensionDataStorage>, net.minecraft.nbt.CompoundTag, java.util.Optional<net.minecraft.resources.ResourceKey<com.mojang.serialization.MapCodec<? extends net.minecraft.world.level.chunk.ChunkGenerator>>>);
  private net.minecraft.world.level.levelgen.structure.LegacyStructureDataHandler getLegacyStructureHandler(net.minecraft.resources.ResourceKey<net.minecraft.world.level.Level>, java.util.function.Supplier<net.minecraft.world.level.storage.DimensionDataStorage>);
  public static void injectDatafixingContext(net.minecraft.nbt.CompoundTag, net.minecraft.resources.ResourceKey<net.minecraft.world.level.Level>, java.util.Optional<net.minecraft.resources.ResourceKey<com.mojang.serialization.MapCodec<? extends net.minecraft.world.level.chunk.ChunkGenerator>>>);
  private static void removeDatafixingContext(net.minecraft.nbt.CompoundTag);
  public static int getVersion(net.minecraft.nbt.CompoundTag);
  public java.util.concurrent.CompletableFuture<java.util.Optional<net.minecraft.nbt.CompoundTag>> read(net.minecraft.world.level.ChunkPos);
  public java.util.concurrent.CompletableFuture<java.lang.Void> write(net.minecraft.world.level.ChunkPos, net.minecraft.nbt.CompoundTag);
  protected void handleLegacyStructureIndex(net.minecraft.world.level.ChunkPos);
  public void flushWorker();
  public void close() throws java.io.IOException;
  public net.minecraft.world.level.chunk.storage.ChunkScanAccess chunkScanner();
  protected net.minecraft.world.level.chunk.storage.RegionStorageInfo storageInfo();
  private static void lambda$injectDatafixingContext$0(net.minecraft.nbt.CompoundTag, net.minecraft.resources.ResourceKey);
}
--- FILE I/O BYTECODE ---
193-       2: invokestatic  #193                // Method net/minecraft/nbt/NbtUtils.getDataVersion:(Lnet/minecraft/nbt/CompoundTag;I)I
194-       5: ireturn
195-
196:  public java.util.concurrent.CompletableFuture<java.util.Optional<net.minecraft.nbt.CompoundTag>> read(net.minecraft.world.level.ChunkPos);
197-    Code:
198-       0: aload_0
199-       1: getfield      #18                 // Field worker:Lnet/minecraft/world/level/chunk/storage/IOWorker;
200-       4: aload_1
201-       5: invokevirtual #196                // Method net/minecraft/world/level/chunk/storage/IOWorker.loadAsync:(Lnet/minecraft/world/level/ChunkPos;)Ljava/util/concurrent/CompletableFuture;
202-       8: areturn
203-
204:  public java.util.concurrent.CompletableFuture<java.lang.Void> write(net.minecraft.world.level.ChunkPos, net.minecraft.nbt.CompoundTag);
205-    Code:
206-       0: aload_0
207-       1: aload_1
208-       2: invokevirtual #200                // Method handleLegacyStructureIndex:(Lnet/minecraft/world/level/ChunkPos;)V
209-       5: aload_0
--
235-      11: pop
236-      12: return
237-
238:  public void close() throws java.io.IOException;
239-    Code:
240-       0: aload_0
241-       1: getfield      #18                 // Field worker:Lnet/minecraft/world/level/chunk/storage/IOWorker;
242-       4: invokevirtual #227                // Method net/minecraft/world/level/chunk/storage/IOWorker.close:()V
243-       7: return

========== net.minecraft.world.level.chunk.storage.SimpleRegionStorage ==========
--- API ---
Compiled from "SimpleRegionStorage.java"
public class net.minecraft.world.level.chunk.storage.SimpleRegionStorage implements java.lang.AutoCloseable {
  private final net.minecraft.world.level.chunk.storage.IOWorker worker;
  private final com.mojang.datafixers.DataFixer fixerUpper;
  private final net.minecraft.util.datafix.DataFixTypes dataFixType;
  public net.minecraft.world.level.chunk.storage.SimpleRegionStorage(net.minecraft.world.level.chunk.storage.RegionStorageInfo, java.nio.file.Path, com.mojang.datafixers.DataFixer, boolean, net.minecraft.util.datafix.DataFixTypes);
  public java.util.concurrent.CompletableFuture<java.util.Optional<net.minecraft.nbt.CompoundTag>> read(net.minecraft.world.level.ChunkPos);
  public java.util.concurrent.CompletableFuture<java.lang.Void> write(net.minecraft.world.level.ChunkPos, net.minecraft.nbt.CompoundTag);
  public net.minecraft.nbt.CompoundTag upgradeChunkTag(net.minecraft.nbt.CompoundTag, int);
  public com.mojang.serialization.Dynamic<net.minecraft.nbt.Tag> upgradeChunkTag(com.mojang.serialization.Dynamic<net.minecraft.nbt.Tag>, int);
  public java.util.concurrent.CompletableFuture<java.lang.Void> synchronize(boolean);
  public void close() throws java.io.IOException;
  public net.minecraft.world.level.chunk.storage.RegionStorageInfo storageInfo();
}
--- FILE I/O BYTECODE ---
26-      27: putfield      #22                 // Field worker:Lnet/minecraft/world/level/chunk/storage/IOWorker;
27-      30: return
28-
29:  public java.util.concurrent.CompletableFuture<java.util.Optional<net.minecraft.nbt.CompoundTag>> read(net.minecraft.world.level.ChunkPos);
30-    Code:
31-       0: aload_0
32-       1: getfield      #22                 // Field worker:Lnet/minecraft/world/level/chunk/storage/IOWorker;
33-       4: aload_1
34-       5: invokevirtual #26                 // Method net/minecraft/world/level/chunk/storage/IOWorker.loadAsync:(Lnet/minecraft/world/level/ChunkPos;)Ljava/util/concurrent/CompletableFuture;
35-       8: areturn
36-
37:  public java.util.concurrent.CompletableFuture<java.lang.Void> write(net.minecraft.world.level.ChunkPos, net.minecraft.nbt.CompoundTag);
38-    Code:
39-       0: aload_0
40-       1: getfield      #22                 // Field worker:Lnet/minecraft/world/level/chunk/storage/IOWorker;
41-       4: aload_1
42-       5: aload_2
--
69-      10: invokevirtual #46                 // Method net/minecraft/util/datafix/DataFixTypes.updateToCurrentVersion:(Lcom/mojang/datafixers/DataFixer;Lcom/mojang/serialization/Dynamic;I)Lcom/mojang/serialization/Dynamic;
70-      13: areturn
71-
72:  public java.util.concurrent.CompletableFuture<java.lang.Void> synchronize(boolean);
73-    Code:
74-       0: aload_0
75-       1: getfield      #22                 // Field worker:Lnet/minecraft/world/level/chunk/storage/IOWorker;
76-       4: iload_1
77-       5: invokevirtual #49                 // Method net/minecraft/world/level/chunk/storage/IOWorker.synchronize:(Z)Ljava/util/concurrent/CompletableFuture;
78-       8: areturn
79-
80:  public void close() throws java.io.IOException;
81-    Code:
82-       0: aload_0
83-       1: getfield      #22                 // Field worker:Lnet/minecraft/world/level/chunk/storage/IOWorker;
84-       4: invokevirtual #53                 // Method net/minecraft/world/level/chunk/storage/IOWorker.close:()V
85-       7: return

========== net.minecraft.world.level.chunk.storage.IOWorker ==========
--- API ---
Compiled from "IOWorker.java"
public class net.minecraft.world.level.chunk.storage.IOWorker implements net.minecraft.world.level.chunk.storage.ChunkScanAccess,java.lang.AutoCloseable {
  private static final org.slf4j.Logger LOGGER;
  private final java.util.concurrent.atomic.AtomicBoolean shutdownRequested;
  private final net.minecraft.util.thread.ProcessorMailbox<net.minecraft.util.thread.StrictQueue$IntRunnable> mailbox;
  private final net.minecraft.world.level.chunk.storage.RegionFileStorage storage;
  private final java.util.Map<net.minecraft.world.level.ChunkPos, net.minecraft.world.level.chunk.storage.IOWorker$PendingStore> pendingWrites;
  private final it.unimi.dsi.fastutil.longs.Long2ObjectLinkedOpenHashMap<java.util.concurrent.CompletableFuture<java.util.BitSet>> regionCacheForBlender;
  private static final int REGION_CACHE_SIZE;
  protected net.minecraft.world.level.chunk.storage.IOWorker(net.minecraft.world.level.chunk.storage.RegionStorageInfo, java.nio.file.Path, boolean);
  public boolean isOldChunkAround(net.minecraft.world.level.ChunkPos, int);
  private java.util.concurrent.CompletableFuture<java.util.BitSet> getOrCreateOldDataForRegion(int, int);
  private java.util.concurrent.CompletableFuture<java.util.BitSet> createOldDataForRegion(int, int);
  private boolean isOldChunk(net.minecraft.nbt.CompoundTag);
  public java.util.concurrent.CompletableFuture<java.lang.Void> store(net.minecraft.world.level.ChunkPos, net.minecraft.nbt.CompoundTag);
  public java.util.concurrent.CompletableFuture<java.util.Optional<net.minecraft.nbt.CompoundTag>> loadAsync(net.minecraft.world.level.ChunkPos);
  public java.util.concurrent.CompletableFuture<java.lang.Void> synchronize(boolean);
  public java.util.concurrent.CompletableFuture<java.lang.Void> scanChunk(net.minecraft.world.level.ChunkPos, net.minecraft.nbt.StreamTagVisitor);
  private <T> java.util.concurrent.CompletableFuture<T> submitTask(java.util.function.Supplier<com.mojang.datafixers.util.Either<T, java.lang.Exception>>);
  private void storePendingChunk();
  private void tellStorePending();
  private void runStore(net.minecraft.world.level.ChunkPos, net.minecraft.world.level.chunk.storage.IOWorker$PendingStore);
  public void close() throws java.io.IOException;
  public net.minecraft.world.level.chunk.storage.RegionStorageInfo storageInfo();
  private static net.minecraft.util.thread.StrictQueue$IntRunnable lambda$close$16(net.minecraft.util.thread.ProcessorHandle);
  private static void lambda$close$15(net.minecraft.util.thread.ProcessorHandle);
  private net.minecraft.util.thread.StrictQueue$IntRunnable lambda$submitTask$14(java.util.function.Supplier, net.minecraft.util.thread.ProcessorHandle);
  private void lambda$submitTask$13(net.minecraft.util.thread.ProcessorHandle, java.util.function.Supplier);
  private com.mojang.datafixers.util.Either lambda$scanChunk$12(net.minecraft.world.level.ChunkPos, net.minecraft.nbt.StreamTagVisitor);
  private java.util.concurrent.CompletionStage lambda$synchronize$11(java.lang.Void);
  private static com.mojang.datafixers.util.Either lambda$synchronize$10();
  private java.util.concurrent.CompletionStage lambda$synchronize$9(java.lang.Void);
  private com.mojang.datafixers.util.Either lambda$synchronize$8();
  private com.mojang.datafixers.util.Either lambda$synchronize$7();
  private static java.util.concurrent.CompletableFuture[] lambda$synchronize$6(int);
  private static java.util.concurrent.CompletableFuture lambda$synchronize$5(net.minecraft.world.level.chunk.storage.IOWorker$PendingStore);
  private com.mojang.datafixers.util.Either lambda$loadAsync$4(net.minecraft.world.level.ChunkPos);
  private com.mojang.datafixers.util.Either lambda$store$3(net.minecraft.world.level.ChunkPos, net.minecraft.nbt.CompoundTag);
  private static net.minecraft.world.level.chunk.storage.IOWorker$PendingStore lambda$store$2(net.minecraft.nbt.CompoundTag, net.minecraft.world.level.ChunkPos);
  private java.util.BitSet lambda$createOldDataForRegion$1(int, int);
  private void lambda$createOldDataForRegion$0(java.util.BitSet, net.minecraft.world.level.ChunkPos);
  static {};
}
--- FILE I/O BYTECODE ---
278-       8: invokevirtual #178                // Method submitTask:(Ljava/util/function/Supplier;)Ljava/util/concurrent/CompletableFuture;
279-      11: areturn
280-
281:  public java.util.concurrent.CompletableFuture<java.lang.Void> synchronize(boolean);
282-    Code:
283-       0: aload_0
284-       1: aload_0
285-       2: invokedynamic #195,  0            // InvokeDynamic #4:get:(Lnet/minecraft/world/level/chunk/storage/IOWorker;)Ljava/util/function/Supplier;
286-       7: invokevirtual #178                // Method submitTask:(Ljava/util/function/Supplier;)Ljava/util/concurrent/CompletableFuture;
--
393-       from    to  target type
394-           0    21    24   Class java/lang/Exception
395-
396:  public void close() throws java.io.IOException;
397-    Code:
398-       0: aload_0
399-       1: getfield      #10                 // Field shutdownRequested:Ljava/util/concurrent/atomic/AtomicBoolean;
400-       4: iconst_0
401-       5: iconst_1

========== net.minecraft.world.level.chunk.storage.EntityStorage ==========
--- API ---
Compiled from "EntityStorage.java"
public class net.minecraft.world.level.chunk.storage.EntityStorage implements net.minecraft.world.level.entity.EntityPersistentStorage<net.minecraft.world.entity.Entity> {
  private static final org.slf4j.Logger LOGGER;
  private static final java.lang.String ENTITIES_TAG;
  private static final java.lang.String POSITION_TAG;
  private final net.minecraft.server.level.ServerLevel level;
  private final net.minecraft.world.level.chunk.storage.SimpleRegionStorage simpleRegionStorage;
  private final it.unimi.dsi.fastutil.longs.LongSet emptyChunks;
  private final net.minecraft.util.thread.ProcessorMailbox<java.lang.Runnable> entityDeserializerQueue;
  public net.minecraft.world.level.chunk.storage.EntityStorage(net.minecraft.world.level.chunk.storage.SimpleRegionStorage, net.minecraft.server.level.ServerLevel, java.util.concurrent.Executor);
  public java.util.concurrent.CompletableFuture<net.minecraft.world.level.entity.ChunkEntities<net.minecraft.world.entity.Entity>> loadEntities(net.minecraft.world.level.ChunkPos);
  private static net.minecraft.world.level.ChunkPos readChunkPos(net.minecraft.nbt.CompoundTag);
  private static void writeChunkPos(net.minecraft.nbt.CompoundTag, net.minecraft.world.level.ChunkPos);
  private static net.minecraft.world.level.entity.ChunkEntities<net.minecraft.world.entity.Entity> emptyChunk(net.minecraft.world.level.ChunkPos);
  public void storeEntities(net.minecraft.world.level.entity.ChunkEntities<net.minecraft.world.entity.Entity>);
  private void reportSaveFailureIfPresent(java.util.concurrent.CompletableFuture<?>, net.minecraft.world.level.ChunkPos);
  private void reportLoadFailureIfPresent(java.util.concurrent.CompletableFuture<?>, net.minecraft.world.level.ChunkPos);
  public void flush(boolean);
  public void close() throws java.io.IOException;
  private java.lang.Object lambda$reportLoadFailureIfPresent$3(net.minecraft.world.level.ChunkPos, java.lang.Throwable);
  private java.lang.Object lambda$reportSaveFailureIfPresent$2(net.minecraft.world.level.ChunkPos, java.lang.Throwable);
  private static void lambda$storeEntities$1(net.minecraft.nbt.ListTag, net.minecraft.world.entity.Entity);
  private net.minecraft.world.level.entity.ChunkEntities lambda$loadEntities$0(net.minecraft.world.level.ChunkPos, java.util.Optional);
  static {};
}
--- FILE I/O BYTECODE ---
200-      11: pop
201-      12: return
202-
203:  public void flush(boolean);
204-    Code:
205-       0: aload_0
206-       1: getfield      #16                 // Field simpleRegionStorage:Lnet/minecraft/world/level/chunk/storage/SimpleRegionStorage;
207-       4: iload_1
208-       5: invokevirtual #181                // Method net/minecraft/world/level/chunk/storage/SimpleRegionStorage.synchronize:(Z)Ljava/util/concurrent/CompletableFuture;
--
213-      16: invokevirtual #189                // Method net/minecraft/util/thread/ProcessorMailbox.runAll:()V
214-      19: return
215-
216:  public void close() throws java.io.IOException;
217-    Code:
218-       0: aload_0
219-       1: getfield      #16                 // Field simpleRegionStorage:Lnet/minecraft/world/level/chunk/storage/SimpleRegionStorage;
220-       4: invokevirtual #192                // Method net/minecraft/world/level/chunk/storage/SimpleRegionStorage.close:()V
221-       7: return

========== net.minecraft.world.level.chunk.storage.SectionStorage ==========
--- API ---
Compiled from "SectionStorage.java"
public class net.minecraft.world.level.chunk.storage.SectionStorage<R> implements java.lang.AutoCloseable {
  private static final org.slf4j.Logger LOGGER;
  private static final java.lang.String SECTIONS_TAG;
  private final net.minecraft.world.level.chunk.storage.SimpleRegionStorage simpleRegionStorage;
  private final it.unimi.dsi.fastutil.longs.Long2ObjectMap<java.util.Optional<R>> storage;
  private final it.unimi.dsi.fastutil.longs.LongLinkedOpenHashSet dirty;
  private final java.util.function.Function<java.lang.Runnable, com.mojang.serialization.Codec<R>> codec;
  private final java.util.function.Function<java.lang.Runnable, R> factory;
  private final net.minecraft.core.RegistryAccess registryAccess;
  private final net.minecraft.world.level.chunk.storage.ChunkIOErrorReporter errorReporter;
  protected final net.minecraft.world.level.LevelHeightAccessor levelHeightAccessor;
  public net.minecraft.world.level.chunk.storage.SectionStorage(net.minecraft.world.level.chunk.storage.SimpleRegionStorage, java.util.function.Function<java.lang.Runnable, com.mojang.serialization.Codec<R>>, java.util.function.Function<java.lang.Runnable, R>, net.minecraft.core.RegistryAccess, net.minecraft.world.level.chunk.storage.ChunkIOErrorReporter, net.minecraft.world.level.LevelHeightAccessor);
  protected void tick(java.util.function.BooleanSupplier);
  public boolean hasWork();
  protected java.util.Optional<R> get(long);
  protected java.util.Optional<R> getOrLoad(long);
  protected boolean outsideStoredRange(long);
  protected R getOrCreate(long);
  private void readColumn(net.minecraft.world.level.ChunkPos);
  private java.util.concurrent.CompletableFuture<java.util.Optional<net.minecraft.nbt.CompoundTag>> tryRead(net.minecraft.world.level.ChunkPos);
  private void readColumn(net.minecraft.world.level.ChunkPos, net.minecraft.resources.RegistryOps<net.minecraft.nbt.Tag>, net.minecraft.nbt.CompoundTag);
  private void writeColumn(net.minecraft.world.level.ChunkPos);
  private <T> com.mojang.serialization.Dynamic<T> writeColumn(net.minecraft.world.level.ChunkPos, com.mojang.serialization.DynamicOps<T>);
  private static long getKey(net.minecraft.world.level.ChunkPos, int);
  protected void onSectionLoad(long);
  protected void setDirty(long);
  private static int getVersion(com.mojang.serialization.Dynamic<?>);
  public void flush(net.minecraft.world.level.ChunkPos);
  public void close() throws java.io.IOException;
  public void remove(long);
  private static void lambda$writeColumn$7(java.util.Map, com.mojang.serialization.DynamicOps, java.lang.String, java.lang.Object);
  private void lambda$writeColumn$6(long);
  private java.lang.Void lambda$writeColumn$5(net.minecraft.world.level.ChunkPos, java.lang.Throwable);
  private void lambda$readColumn$4(long, boolean, java.lang.Object);
  private java.util.Optional lambda$readColumn$3(long, com.mojang.serialization.Dynamic);
  private void lambda$readColumn$2(long);
  private java.util.Optional lambda$tryRead$1(net.minecraft.world.level.ChunkPos, java.lang.Throwable);
  private void lambda$getOrCreate$0(long);
  static {};
}
--- FILE I/O BYTECODE ---
481-      10: invokevirtual #368                // Method com/mojang/serialization/OptionalDynamic.asInt:(I)I
482-      13: ireturn
483-
484:  public void flush(net.minecraft.world.level.ChunkPos);
485-    Code:
486-       0: aload_0
487-       1: invokevirtual #46                 // Method hasWork:()Z
488-       4: ifeq          59
489-       7: aload_0
--
512-      56: goto          17
513-      59: return
514-
515:  public void close() throws java.io.IOException;
516-    Code:
517-       0: aload_0
518-       1: getfield      #23                 // Field simpleRegionStorage:Lnet/minecraft/world/level/chunk/storage/SimpleRegionStorage;
519-       4: invokevirtual #374                // Method net/minecraft/world/level/chunk/storage/SimpleRegionStorage.close:()V
520-       7: return
521-
522:  public void remove(long);
523-    Code:
524-       0: aload_0
525-       1: getfield      #10                 // Field storage:Lit/unimi/dsi/fastutil/longs/Long2ObjectMap;
526-       4: lload_1
527-       5: invokeinterface #377,  3          // InterfaceMethod it/unimi/dsi/fastutil/longs/Long2ObjectMap.remove:(J)Ljava/lang/Object;

========== net.minecraft.world.entity.ai.village.poi.PoiManager ==========
--- API ---
Compiled from "PoiManager.java"
public class net.minecraft.world.entity.ai.village.poi.PoiManager extends net.minecraft.world.level.chunk.storage.SectionStorage<net.minecraft.world.entity.ai.village.poi.PoiSection> {
  public static final int MAX_VILLAGE_DISTANCE;
  public static final int VILLAGE_SECTION_SIZE;
  private final net.minecraft.world.entity.ai.village.poi.PoiManager$DistanceTracker distanceTracker;
  private final it.unimi.dsi.fastutil.longs.LongSet loadedChunks;
  public net.minecraft.world.entity.ai.village.poi.PoiManager(net.minecraft.world.level.chunk.storage.RegionStorageInfo, java.nio.file.Path, com.mojang.datafixers.DataFixer, boolean, net.minecraft.core.RegistryAccess, net.minecraft.world.level.chunk.storage.ChunkIOErrorReporter, net.minecraft.world.level.LevelHeightAccessor);
  public void add(net.minecraft.core.BlockPos, net.minecraft.core.Holder<net.minecraft.world.entity.ai.village.poi.PoiType>);
  public void remove(net.minecraft.core.BlockPos);
  public long getCountInRange(java.util.function.Predicate<net.minecraft.core.Holder<net.minecraft.world.entity.ai.village.poi.PoiType>>, net.minecraft.core.BlockPos, int, net.minecraft.world.entity.ai.village.poi.PoiManager$Occupancy);
  public boolean existsAtPosition(net.minecraft.resources.ResourceKey<net.minecraft.world.entity.ai.village.poi.PoiType>, net.minecraft.core.BlockPos);
  public java.util.stream.Stream<net.minecraft.world.entity.ai.village.poi.PoiRecord> getInSquare(java.util.function.Predicate<net.minecraft.core.Holder<net.minecraft.world.entity.ai.village.poi.PoiType>>, net.minecraft.core.BlockPos, int, net.minecraft.world.entity.ai.village.poi.PoiManager$Occupancy);
  public java.util.stream.Stream<net.minecraft.world.entity.ai.village.poi.PoiRecord> getInRange(java.util.function.Predicate<net.minecraft.core.Holder<net.minecraft.world.entity.ai.village.poi.PoiType>>, net.minecraft.core.BlockPos, int, net.minecraft.world.entity.ai.village.poi.PoiManager$Occupancy);
  public java.util.stream.Stream<net.minecraft.world.entity.ai.village.poi.PoiRecord> getInChunk(java.util.function.Predicate<net.minecraft.core.Holder<net.minecraft.world.entity.ai.village.poi.PoiType>>, net.minecraft.world.level.ChunkPos, net.minecraft.world.entity.ai.village.poi.PoiManager$Occupancy);
  public java.util.stream.Stream<net.minecraft.core.BlockPos> findAll(java.util.function.Predicate<net.minecraft.core.Holder<net.minecraft.world.entity.ai.village.poi.PoiType>>, java.util.function.Predicate<net.minecraft.core.BlockPos>, net.minecraft.core.BlockPos, int, net.minecraft.world.entity.ai.village.poi.PoiManager$Occupancy);
  public java.util.stream.Stream<com.mojang.datafixers.util.Pair<net.minecraft.core.Holder<net.minecraft.world.entity.ai.village.poi.PoiType>, net.minecraft.core.BlockPos>> findAllWithType(java.util.function.Predicate<net.minecraft.core.Holder<net.minecraft.world.entity.ai.village.poi.PoiType>>, java.util.function.Predicate<net.minecraft.core.BlockPos>, net.minecraft.core.BlockPos, int, net.minecraft.world.entity.ai.village.poi.PoiManager$Occupancy);
  public java.util.stream.Stream<com.mojang.datafixers.util.Pair<net.minecraft.core.Holder<net.minecraft.world.entity.ai.village.poi.PoiType>, net.minecraft.core.BlockPos>> findAllClosestFirstWithType(java.util.function.Predicate<net.minecraft.core.Holder<net.minecraft.world.entity.ai.village.poi.PoiType>>, java.util.function.Predicate<net.minecraft.core.BlockPos>, net.minecraft.core.BlockPos, int, net.minecraft.world.entity.ai.village.poi.PoiManager$Occupancy);
  public java.util.Optional<net.minecraft.core.BlockPos> find(java.util.function.Predicate<net.minecraft.core.Holder<net.minecraft.world.entity.ai.village.poi.PoiType>>, java.util.function.Predicate<net.minecraft.core.BlockPos>, net.minecraft.core.BlockPos, int, net.minecraft.world.entity.ai.village.poi.PoiManager$Occupancy);
  public java.util.Optional<net.minecraft.core.BlockPos> findClosest(java.util.function.Predicate<net.minecraft.core.Holder<net.minecraft.world.entity.ai.village.poi.PoiType>>, net.minecraft.core.BlockPos, int, net.minecraft.world.entity.ai.village.poi.PoiManager$Occupancy);
  public java.util.Optional<com.mojang.datafixers.util.Pair<net.minecraft.core.Holder<net.minecraft.world.entity.ai.village.poi.PoiType>, net.minecraft.core.BlockPos>> findClosestWithType(java.util.function.Predicate<net.minecraft.core.Holder<net.minecraft.world.entity.ai.village.poi.PoiType>>, net.minecraft.core.BlockPos, int, net.minecraft.world.entity.ai.village.poi.PoiManager$Occupancy);
  public java.util.Optional<net.minecraft.core.BlockPos> findClosest(java.util.function.Predicate<net.minecraft.core.Holder<net.minecraft.world.entity.ai.village.poi.PoiType>>, java.util.function.Predicate<net.minecraft.core.BlockPos>, net.minecraft.core.BlockPos, int, net.minecraft.world.entity.ai.village.poi.PoiManager$Occupancy);
  public java.util.Optional<net.minecraft.core.BlockPos> take(java.util.function.Predicate<net.minecraft.core.Holder<net.minecraft.world.entity.ai.village.poi.PoiType>>, java.util.function.BiPredicate<net.minecraft.core.Holder<net.minecraft.world.entity.ai.village.poi.PoiType>, net.minecraft.core.BlockPos>, net.minecraft.core.BlockPos, int);
  public java.util.Optional<net.minecraft.core.BlockPos> getRandom(java.util.function.Predicate<net.minecraft.core.Holder<net.minecraft.world.entity.ai.village.poi.PoiType>>, java.util.function.Predicate<net.minecraft.core.BlockPos>, net.minecraft.world.entity.ai.village.poi.PoiManager$Occupancy, net.minecraft.core.BlockPos, int, net.minecraft.util.RandomSource);
  public boolean release(net.minecraft.core.BlockPos);
  public boolean exists(net.minecraft.core.BlockPos, java.util.function.Predicate<net.minecraft.core.Holder<net.minecraft.world.entity.ai.village.poi.PoiType>>);
  public java.util.Optional<net.minecraft.core.Holder<net.minecraft.world.entity.ai.village.poi.PoiType>> getType(net.minecraft.core.BlockPos);
  public int getFreeTickets(net.minecraft.core.BlockPos);
  public int sectionsToVillage(net.minecraft.core.SectionPos);
  boolean isVillageCenter(long);
  public void tick(java.util.function.BooleanSupplier);
  protected void setDirty(long);
  protected void onSectionLoad(long);
  public void checkConsistencyWithBlocks(net.minecraft.core.SectionPos, net.minecraft.world.level.chunk.LevelChunkSection);
  private static boolean mayHavePoi(net.minecraft.world.level.chunk.LevelChunkSection);
  private void updateFromSection(net.minecraft.world.level.chunk.LevelChunkSection, net.minecraft.core.SectionPos, java.util.function.BiConsumer<net.minecraft.core.BlockPos, net.minecraft.core.Holder<net.minecraft.world.entity.ai.village.poi.PoiType>>);
  public void ensureLoadedAndValid(net.minecraft.world.level.LevelReader, net.minecraft.core.BlockPos, int);
  private static void lambda$ensureLoadedAndValid$33(net.minecraft.world.level.LevelReader, net.minecraft.world.level.ChunkPos);
  private boolean lambda$ensureLoadedAndValid$32(net.minecraft.world.level.ChunkPos);
  private static net.minecraft.world.level.ChunkPos lambda$ensureLoadedAndValid$31(com.mojang.datafixers.util.Pair);
  private static boolean lambda$ensureLoadedAndValid$30(com.mojang.datafixers.util.Pair);
  private com.mojang.datafixers.util.Pair lambda$ensureLoadedAndValid$29(net.minecraft.core.SectionPos);
  private static void lambda$updateFromSection$28(net.minecraft.world.level.chunk.LevelChunkSection, java.util.function.BiConsumer, net.minecraft.core.BlockPos);
  private static void lambda$updateFromSection$27(java.util.function.BiConsumer, net.minecraft.core.BlockPos, net.minecraft.core.Holder);
  private void lambda$checkConsistencyWithBlocks$26(net.minecraft.world.level.chunk.LevelChunkSection, net.minecraft.core.SectionPos);
  private void lambda$checkConsistencyWithBlocks$25(net.minecraft.world.level.chunk.LevelChunkSection, net.minecraft.core.SectionPos, net.minecraft.world.entity.ai.village.poi.PoiSection);
  private void lambda$checkConsistencyWithBlocks$24(net.minecraft.world.level.chunk.LevelChunkSection, net.minecraft.core.SectionPos, java.util.function.BiConsumer);
  private static java.lang.Boolean lambda$isVillageCenter$23(net.minecraft.world.entity.ai.village.poi.PoiSection);
  private static boolean lambda$isVillageCenter$22(net.minecraft.core.Holder);
  private static java.lang.Integer lambda$getFreeTickets$21(net.minecraft.core.BlockPos, net.minecraft.world.entity.ai.village.poi.PoiSection);
  private static java.util.Optional lambda$getType$20(net.minecraft.core.BlockPos, net.minecraft.world.entity.ai.village.poi.PoiSection);
  private static java.lang.Boolean lambda$exists$19(net.minecraft.core.BlockPos, java.util.function.Predicate, net.minecraft.world.entity.ai.village.poi.PoiSection);
  private static java.lang.IllegalStateException lambda$release$18(net.minecraft.core.BlockPos);
  private static java.lang.Boolean lambda$release$17(net.minecraft.core.BlockPos, net.minecraft.world.entity.ai.village.poi.PoiSection);
  private static boolean lambda$getRandom$16(java.util.function.Predicate, net.minecraft.world.entity.ai.village.poi.PoiRecord);
  private static net.minecraft.core.BlockPos lambda$take$15(net.minecraft.world.entity.ai.village.poi.PoiRecord);
  private static boolean lambda$take$14(java.util.function.BiPredicate, net.minecraft.world.entity.ai.village.poi.PoiRecord);
  private static double lambda$findClosest$13(net.minecraft.core.BlockPos, net.minecraft.core.BlockPos);
  private static com.mojang.datafixers.util.Pair lambda$findClosestWithType$12(net.minecraft.world.entity.ai.village.poi.PoiRecord);
  private static double lambda$findClosestWithType$11(net.minecraft.core.BlockPos, net.minecraft.world.entity.ai.village.poi.PoiRecord);
  private static double lambda$findClosest$10(net.minecraft.core.BlockPos, net.minecraft.core.BlockPos);
  private static double lambda$findAllClosestFirstWithType$9(net.minecraft.core.BlockPos, com.mojang.datafixers.util.Pair);
  private static com.mojang.datafixers.util.Pair lambda$findAllWithType$8(net.minecraft.world.entity.ai.village.poi.PoiRecord);
  private static boolean lambda$findAllWithType$7(java.util.function.Predicate, net.minecraft.world.entity.ai.village.poi.PoiRecord);
  private static java.util.stream.Stream lambda$getInChunk$6(java.util.function.Predicate, net.minecraft.world.entity.ai.village.poi.PoiManager$Occupancy, java.util.Optional);
  private java.util.Optional lambda$getInChunk$5(net.minecraft.world.level.ChunkPos, java.lang.Integer);
  private static boolean lambda$getInRange$4(net.minecraft.core.BlockPos, int, net.minecraft.world.entity.ai.village.poi.PoiRecord);
  private static boolean lambda$getInSquare$3(net.minecraft.core.BlockPos, int, net.minecraft.world.entity.ai.village.poi.PoiRecord);
  private java.util.stream.Stream lambda$getInSquare$2(java.util.function.Predicate, net.minecraft.world.entity.ai.village.poi.PoiManager$Occupancy, net.minecraft.world.level.ChunkPos);
  private static boolean lambda$existsAtPosition$1(net.minecraft.resources.ResourceKey, net.minecraft.core.Holder);
  private static void lambda$remove$0(net.minecraft.core.BlockPos, net.minecraft.world.entity.ai.village.poi.PoiSection);
}
--- FILE I/O BYTECODE ---
50-      13: invokevirtual #55                 // Method net/minecraft/world/entity/ai/village/poi/PoiSection.add:(Lnet/minecraft/core/BlockPos;Lnet/minecraft/core/Holder;)V
51-      16: return
52-
53:  public void remove(net.minecraft.core.BlockPos);
54-    Code:
55-       0: aload_0
56-       1: aload_1
57-       2: invokestatic  #43                 // Method net/minecraft/core/SectionPos.asLong:(Lnet/minecraft/core/BlockPos;)J
58-       5: invokevirtual #59                 // Method getOrLoad:(J)Ljava/util/Optional;
