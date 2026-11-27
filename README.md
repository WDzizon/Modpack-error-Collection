wdzizon@DESKTOP-LS6DH9N:~/lod-server-support-lod-only$ cd ~/lod-server-support-lod-only
wdzizon@DESKTOP-LS6DH9N:~/lod-server-support-lod-only$ git pull --ff-only origin feat/lod-only-preservation-1.21.1

From https://github.com/WDzizon/lod-server-support-lod-only
 * branch                feat/lod-only-preservation-1.21.1 -> FETCH_HEAD
Already up to date.
wdzizon@DESKTOP-LS6DH9N:~/lod-server-support-lod-only$ ./gradlew :neoforge:test --rerun-tasks
│██▌····│█████··│█████··│█████··│█████··
> Configure project :fabricbric           > :fabric > :fabric
Fabric Loom: 1.17.13
│████│█
> Configure project :sponge
SpongePowered Plugin 'GRADLE' Toolset Version '2.3.0'
Targeting Minecraft '1.21.1' on a 'SERVER' platform
│·······│·······│·······│·······
> Task :common:compileJava
> Task :neoforge:createMinecraftArtifactsd-only/common/src/main/java/dev/vox/lss/common/config/LegacySettingsMigration.java uses or overrides a deprecated API.
Loaded 131 artifacts from /home/wdzizon/lod-server-support-lod-only/neoforge/build/tmp/createMinecraftArtifacts/nfrt_artifact_manifest.properties
*** Started working on downloadJson···│ 14% EXECUTING [2s]
 ✓ Completed downloadJson in 0.03sn:generateSqliteRuntime
*** Started working on downloadServerraftArtifacts
*** Started working on downloadClient
*** Started working on downloadClientMappings
 ✓ Completed downloadClientMappings in 0.05s
 ✓ Completed downloadServer in 0.05s
 ✓ Completed downloadClient in 0.05s
*** Started working on mergeMappings
 ♻ Used cache of mergeMappings in 0.00s
*** Started working on stripClient
 ♻ Used cache of stripClient in 0.00s
*** Started working on extractServer
 ♻ Used cache of extractServer in 0.00s
*** Started working on stripServer
 ♻ Used cache of stripServer in 0.00s
*** Started working on merge
 ♻ Used cache of merge in 0.00s
*** Started working on rename
 ♻ Used cache of rename in 0.00s
*** Started working on decompile
 ♻ Used cache of decompile in 0.00s
│██▏····*** Started working on injectNG [2s]
 ♻ Used cache of inject in 0.00siteRuntime
*** Started working on patchteMinecraftArtifacts
 ♻ Used cache of patch in 0.00s
│██▏····│██▏····*** Started working on applyNeoforgePatches
 ♻ Used cache of applyNeoforgePatches in 0.00s
*** Started working on transformSourcesArtifacts
 ♻ Used cache of transformSources in 0.00s
│██▏····*** Started working on recompile[3s]
 ♻ Used cache of recompile in 0.00sRuntime
│█████▎·*** Started working on sourcesWithNeoForge
 ♻ Used cache of sourcesWithNeoForge in 0.00s
│█████▎·*** Started working on compiledWithNeoForge
 ♻ Used cache of compiledWithNeoForge in 0.00s
│█████▎·*** Started working on sourcesAndCompiledWithNeoForge
 ♻ Used cache of sourcesAndCompiledWithNeoForge in 0.00s
│██████▍│██████▍Total runtime: 3.08s

│██████│██████│██████
> Task :neoforge:compileJava
Note: /home/wdzizon/lod-server-support-lod-only/xplat/src/main/java/dev/vox/lss/compat/XaeroTileExtractor.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
│███
> Task :neoforge:compileTestJava FAILED
/home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:3: error: package net.minecraft.world.level does not exist
import net.minecraft.world.level.ChunkPos;
                                ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:4: error: package net.minecraft.world.level does not exist
import net.minecraft.world.level.Level;
                                ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:5: error: package net.minecraft.nbt does not exist
import net.minecraft.nbt.CompoundTag;
                        ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:6: error: package net.minecraft.world.level.chunk.storage does not exist
import net.minecraft.world.level.chunk.storage.IOWorker;
                                              ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:7: error: package net.minecraft.world.level.chunk.storage does not exist
import net.minecraft.world.level.chunk.storage.RegionStorageInfo;
                                              ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:26: error: cannot find symbol
    private static final ChunkPos TARGET = new ChunkPos(10, 10);
                         ^
  symbol:   class ChunkPos
  location: class NeoForgeIOWorkerNullStoreTest
/home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:27: error: cannot find symbol
    private static final ChunkPos NEIGHBOR = new ChunkPos(11, 10);
                         ^
  symbol:   class ChunkPos
  location: class NeoForgeIOWorkerNullStoreTest
/home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:63: error: cannot find symbol
    private static void assertPayload(IOWorker worker, ChunkPos position, String expected)
                                      ^
  symbol:   class IOWorker
  location: class NeoForgeIOWorkerNullStoreTest
/home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:63: error: cannot find symbol
    private static void assertPayload(IOWorker worker, ChunkPos position, String expected)
                                                       ^
  symbol:   class ChunkPos
  location: class NeoForgeIOWorkerNullStoreTest
/home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:70: error: cannot find symbol
    private static CompoundTag payload(String marker) {
                   ^
  symbol:   class CompoundTag
  location: class NeoForgeIOWorkerNullStoreTest
/home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:80: error: cannot find symbol
    private static final class TestWorker extends IOWorker {
                                                  ^
  symbol:   class IOWorker
  location: class NeoForgeIOWorkerNullStoreTest
/home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:26: error: cannot find symbol
    private static final ChunkPos TARGET = new ChunkPos(10, 10);
                                               ^
  symbol:   class ChunkPos
  location: class NeoForgeIOWorkerNullStoreTest
/home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:27: error: cannot find symbol
    private static final ChunkPos NEIGHBOR = new ChunkPos(11, 10);
                                                 ^
  symbol:   class ChunkPos
  location: class NeoForgeIOWorkerNullStoreTest
/home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:34: error: incompatible types: try-with-resources not applicable to variable type
        try (TestWorker worker = new TestWorker(temporaryRegionDirectory)) {
                        ^
    (TestWorker cannot be converted to AutoCloseable)
/home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:39: error: cannot find symbol
            await(worker.synchronize(true));
                        ^
  symbol:   method synchronize(boolean)
  location: variable worker of type TestWorker
/home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:47: error: cannot find symbol
            await(worker.synchronize(true));
                        ^
  symbol:   method synchronize(boolean)
  location: variable worker of type TestWorker
/home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:56: error: incompatible types: try-with-resources not applicable to variable type
        try (TestWorker reopened = new TestWorker(temporaryRegionDirectory)) {
                        ^
    (TestWorker cannot be converted to AutoCloseable)
/home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:65: error: cannot find symbol
        Optional<CompoundTag> stored = await(worker.loadAsync(position));
                 ^
  symbol:   class CompoundTag
  location: class NeoForgeIOWorkerNullStoreTest
/home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:71: error: cannot find symbol
        CompoundTag tag = new CompoundTag();
        ^
  symbol:   class CompoundTag
  location: class NeoForgeIOWorkerNullStoreTest
/home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:71: error: cannot find symbol
        CompoundTag tag = new CompoundTag();
                              ^
  symbol:   class CompoundTag
  location: class NeoForgeIOWorkerNullStoreTest
/home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:82: error: cannot find symbol
            super(new RegionStorageInfo("lss-null-store-test", Level.OVERWORLD, "chunk"),
                      ^
  symbol:   class RegionStorageInfo
  location: class TestWorker
/home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:82: error: cannot find symbol
            super(new RegionStorageInfo("lss-null-store-test", Level.OVERWORLD, "chunk"),
                                                               ^
  symbol:   variable Level
  location: class TestWorker
22 errors

[Incubating] Problems report is available at: file:///home/wdzizon/lod-server-support-lod-only/build/reports/problems/problems-report.html

FAILURE: Build failed with an exception.

* What went wrong:
Execution failed for task ':neoforge:compileTestJava' (registered by plugin class 'org.gradle.api.plugins.JavaBasePlugin').
> Compilation failed; see the compiler output below.
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:34: error: incompatible types: try-with-resources not applicable to variable type
          try (TestWorker worker = new TestWorker(temporaryRegionDirectory)) {
                          ^
      (TestWorker cannot be converted to AutoCloseable)
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:56: error: incompatible types: try-with-resources not applicable to variable type
          try (TestWorker reopened = new TestWorker(temporaryRegionDirectory)) {
                          ^
      (TestWorker cannot be converted to AutoCloseable)
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:26: error: cannot find symbol
      private static final ChunkPos TARGET = new ChunkPos(10, 10);
                           ^
    symbol:   class ChunkPos
    location: class NeoForgeIOWorkerNullStoreTest
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:27: error: cannot find symbol
      private static final ChunkPos NEIGHBOR = new ChunkPos(11, 10);
                           ^
    symbol:   class ChunkPos
    location: class NeoForgeIOWorkerNullStoreTest
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:63: error: cannot find symbol
      private static void assertPayload(IOWorker worker, ChunkPos position, String expected)
                                        ^
    symbol:   class IOWorker
    location: class NeoForgeIOWorkerNullStoreTest
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:63: error: cannot find symbol
      private static void assertPayload(IOWorker worker, ChunkPos position, String expected)
                                                         ^
    symbol:   class ChunkPos
    location: class NeoForgeIOWorkerNullStoreTest
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:70: error: cannot find symbol
      private static CompoundTag payload(String marker) {
                     ^
    symbol:   class CompoundTag
    location: class NeoForgeIOWorkerNullStoreTest
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:80: error: cannot find symbol
      private static final class TestWorker extends IOWorker {
                                                    ^
    symbol:   class IOWorker
    location: class NeoForgeIOWorkerNullStoreTest
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:26: error: cannot find symbol
      private static final ChunkPos TARGET = new ChunkPos(10, 10);
                                                 ^
    symbol:   class ChunkPos
    location: class NeoForgeIOWorkerNullStoreTest
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:27: error: cannot find symbol
      private static final ChunkPos NEIGHBOR = new ChunkPos(11, 10);
                                                   ^
    symbol:   class ChunkPos
    location: class NeoForgeIOWorkerNullStoreTest
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:65: error: cannot find symbol
          Optional<CompoundTag> stored = await(worker.loadAsync(position));
                   ^
    symbol:   class CompoundTag
    location: class NeoForgeIOWorkerNullStoreTest
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:71: error: cannot find symbol
          CompoundTag tag = new CompoundTag();
          ^
    symbol:   class CompoundTag
    location: class NeoForgeIOWorkerNullStoreTest
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:71: error: cannot find symbol
          CompoundTag tag = new CompoundTag();
                                ^
    symbol:   class CompoundTag
    location: class NeoForgeIOWorkerNullStoreTest
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:82: error: cannot find symbol
              super(new RegionStorageInfo("lss-null-store-test", Level.OVERWORLD, "chunk"),
                        ^
    symbol:   class RegionStorageInfo
    location: class TestWorker
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:82: error: cannot find symbol
              super(new RegionStorageInfo("lss-null-store-test", Level.OVERWORLD, "chunk"),
                                                                 ^
    symbol:   variable Level
    location: class TestWorker
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:39: error: cannot find symbol
              await(worker.synchronize(true));
                          ^
    symbol:   method synchronize(boolean)
    location: variable worker of type TestWorker
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:47: error: cannot find symbol
              await(worker.synchronize(true));
                          ^
    symbol:   method synchronize(boolean)
    location: variable worker of type TestWorker
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:3: error: package net.minecraft.world.level does not exist
  import net.minecraft.world.level.ChunkPos;
                                  ^
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:4: error: package net.minecraft.world.level does not exist
  import net.minecraft.world.level.Level;
                                  ^
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:5: error: package net.minecraft.nbt does not exist
  import net.minecraft.nbt.CompoundTag;
                          ^
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:6: error: package net.minecraft.world.level.chunk.storage does not exist
  import net.minecraft.world.level.chunk.storage.IOWorker;
                                                ^
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreTest.java:7: error: package net.minecraft.world.level.chunk.storage does not exist
  import net.minecraft.world.level.chunk.storage.RegionStorageInfo;
                                                ^
  22 errors

* Try:
> Check your code and dependencies to fix the compilation error(s)
> Run with --scan to get full insights from a Build Scan (powered by Develocity).

Deprecated Gradle features were used in this build, making it incompatible with Gradle 10.

You can use '--warning-mode all' to show the individual deprecation warnings and determine if they come from your own scripts or plugins.

For more on this, please refer to https://docs.gradle.org/9.5.1/userguide/command_line_interface.html#sec:command_line_warnings in the Gradle documentation.

BUILD FAILED in 6s
9 actionable tasks: 9 executed
