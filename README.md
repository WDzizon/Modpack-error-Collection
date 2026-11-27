wdzizon@DESKTOP-LS6DH9N:~/lod-server-support-lod-only$ cd ~/lod-server-support-lod-only &&
> git pull --ff-only origin feat/lod-only-preservation-1.21.1 &&
> ./gradlew :neoforge:test :neoforge:compileGametestJava :neoforge:runGameTestServer
remote: Enumerating objects: 46, done.
remote: Counting objects: 100% (46/46), done.
remote: Compressing objects: 100% (18/18), done.
remote: Total 28 (delta 9), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (28/28), 4.24 KiB | 241.00 KiB/s, done.
From https://github.com/WDzizon/lod-server-support-lod-only
 * branch                feat/lod-only-preservation-1.21.1 -> FETCH_HEAD
   25c7699ca..54071c72a  feat/lod-only-preservation-1.21.1 -> origin/feat/lod-only-preservation-1.21.1
Updating 25c7699ca..54071c72a
Fast-forward
 docs/planning/lod-only-preservation-plan.md                                            |  31 +++++++++++++++++++++++++++++++
 neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java          | 102 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreContractTest.java |   6 ++++++
 3 files changed, 139 insertions(+)
│██▌····│█████··│█████··│█████··│█████··│█████··│█████··
> Configure project :fabricbric                               > :fabric > :fabric
Fabric Loom: 1.17.13
│██████│████│█
> Configure project :sponge
SpongePowered Plugin 'GRADLE' Toolset Version '2.3.0'
Targeting Minecraft '1.21.1' on a 'SERVER' platform
│████│████
> Task :neoforge:compileGametestJava
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:233: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
            var firstPlayer = helper.makeMockServerPlayerInLevel();
                                    ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:254: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
            var secondPlayer = helper.makeMockServerPlayerInLevel();
                                     ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:371: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
        var player = helper.makeMockServerPlayerInLevel();
                           ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:387: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
        var player = helper.makeMockServerPlayerInLevel();
                           ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:404: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
        var player = helper.makeMockServerPlayerInLevel();
                           ^
5 warnings

> Task :neoforge:runGameTestServer
WARN StatusConsoleListener Advanced terminal features are not available in this environment
[15:27:16] [main/INFO] [cp.mo.mo.Launcher/MODLAUNCHER]: ModLauncher running: args [--launchTarget, forgeserverdev, --gameDir, ., --fml.fmlVersion, 4.0.45, --fml.mcVersion, 1.21.1, --fml.neoForgeVersion, 21.1.267, --fml.neoFormVersion, 20240808.144430]
[15:27:16] [main/INFO] [cp.mo.mo.Launcher/MODLAUNCHER]: JVM identified as Ubuntu OpenJDK 64-Bit Server VM 21.0.13.1+2-1-24.04.1-Ubuntu
[15:27:16] [main/INFO] [cp.mo.mo.Launcher/MODLAUNCHER]: ModLauncher 11.0.5+main.901c6ea8 starting: java version 21.0.13.1 by Ubuntu; OS Linux arch amd64 version 6.18.40.1-microsoft-standard-WSL2
[15:27:17] [main/INFO] [ne.ne.fm.lo.ImmediateWindowHandler/]: ImmediateWindowProvider not loading because launch target is forgeserverdev
[15:27:17] [main/INFO] [mixin/]: SpongePowered MIXIN Subsystem Version=0.8.7 Source=union:/home/wdzizon/.gradle/caches/modules-2/files-2.1/net.fabricmc/sponge-mixin/0.16.4+mixin.0.8.7/26d01f0567ab46e9ca0d2ed89d0ecc11aadbd433/sponge-mixin-0.16.4+mixin.0.8.7.jar%2398!/ Service=ModLauncher Env=SERVER
[15:27:17] [main/INFO] [ne.ne.fm.lo.mo.lo.JarInJarDependencyLocator/]: Found 2 dependencies adding them to mods collection
[15:27:17] [main/INFO] [ne.ne.fm.lo.mo.ModDiscoverer/]:
     Mod List:
                Name Version (Mod Id)

                LOD Server Support 0.23.0 (lss)
                LSS NeoForge GameTests 1.0.0 (lsstest)
                Minecraft 1.21.1 (minecraft)
                NeoForge 21.1.267 (neoforge)
[15:27:18] [main/INFO] [mixin/]: Compatibility level set to JAVA_21
[15:27:18] [main/INFO] [cp.mo.mo.LaunchServiceHandler/MODLAUNCHER]: Launching target 'forgeserverdev' with arguments [--gameDir, .]
[15:27:19] [main/INFO] [MixinExtras|Service/]: Initializing MixinExtras via com.llamalad7.mixinextras.service.MixinExtrasServiceImpl(version=0.5.5).
[15:27:27] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, location] and [teleport, destination] with inputs: [0.1 -0.5 .9, 0 0 0]
[15:27:27] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, location] and [teleport, targets] with inputs: [0.1 -0.5 .9, 0 0 0]
[15:27:27] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, destination] and [teleport, targets] with inputs: [Player, 0123, @e, dd12be42-52a9-4a91-a8a1-11c01849e498]
[15:27:27] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, targets] and [teleport, destination] with inputs: [Player, 0123, dd12be42-52a9-4a91-a8a1-11c01849e498]
[15:27:27] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, targets, location] and [teleport, targets, destination] with inputs: [0.1 -0.5 .9, 0 0 0]
[15:27:27] [modloading-worker-0/INFO] [ne.ne.ne.co.NeoForgeMod/NEOFORGE-MOD]: NeoForge mod loading, version 21.1.267, for MC 1.21.1
[15:27:28] [main/INFO] [mojang/YggdrasilAuthenticationService]: Environment: Environment[sessionHost=https://sessionserver.mojang.com, servicesHost=https://api.minecraftservices.com, name=PROD]
[15:27:28] [main/WARN] [minecraft/VanillaPackResourcesBuilder]: Assets URL 'union:/home/wdzizon/lod-server-support-lod-only/neoforge/build/moddev/artifacts/neoforge-21.1.267.jar%23132!/assets/.mcassetsroot' uses unexpected schema
[15:27:28] [main/WARN] [minecraft/VanillaPackResourcesBuilder]: Assets URL 'union:/home/wdzizon/lod-server-support-lod-only/neoforge/build/moddev/artifacts/neoforge-21.1.267.jar%23132!/data/.mcassetsroot' uses unexpected schema
[15:27:28] [main/INFO] [ne.ne.ne.ga.GameTestHooks/]: Enabled Gametest Namespaces: [lsstest]
[15:27:30] [main/INFO] [minecraft/RecipeManager]: Loaded 1291 recipes
[15:27:30] [main/INFO] [minecraft/AdvancementTree]: Loaded 1400 advancements
[15:27:32] [Server thread/INFO] [minecraft/MinecraftServer]: Preparing start region for dimension minecraft:overworld
[15:27:32] [worldgen/INFO] [minecraft/LoggerChunkProgressListener]: Preparing spawn area: 2%
[15:27:32] [Server thread/INFO] [minecraft/LoggerChunkProgressListener]: Time elapsed: 371 ms
[15:27:32] [Server thread/INFO] [minecraft/GameTestServer]: Started game test server
[15:27:32] [Server thread/INFO] [ne.ne.ne.se.pe.PermissionAPI/]: Successfully initialized permission handler neoforge:default_handler
[15:27:33] [Server thread/INFO] [LSS/]: LOD-only durable archive ready: LOD-only archive: state=ready schema=2 queue=0/4096 visit_history=positive-only absence=unknown invalidations_pending=0 invalidation_jobs=0/0/0 invalidation_batches=0 archive_write_batches=0 invalidation_active=false invalidation_last_started_age_ms=-1 invalidation_last_completed_age_ms=-1 egress_invalidation_blocked=false egress_visit_publication_blocked=false archive_untrusted=false session_visits=0 session_visit_overflow=false session_invalidations=0 session_invalidation_overflow=false tracking_started_ms=1795496799715
[15:27:33] [Server thread/INFO] [LSS/]: Starting LSS LOD request processing service
[15:27:33] [Server thread/INFO] [LSS/]: LOD store active (driver=private/3.49.1.0). It stores served LOD bytes under <world>/lss-lod/ and, once fully warmed, occupies roughly as much space as the region files themselves. It is DERIVED data — deleting lss-lod/ is always safe. Set storage.lod_store.enabled to false and restart to disable; storage.lod_store.max_size_mib bounds its size after reload.
[15:27:33] [Server thread/INFO] [LSS/]: Effective config: useNbtTranscode=true, diskReaderThreads=3, useCompressedColumns=true, useBackgroundReadSplit=true, useSelectiveNbtParse=true, maxConcurrentDiskReads=2
[15:27:33] [LSS LOD Store SQLite/INFO] [LSS/]: LOD store sweep [minecraft:overworld]: 2 changed region(s), dropped 0 stale + 0 vanished-region row(s)
[15:27:33] [LSS Store Backfill/INFO] [LSS/]: Store backfill: 49 region(s) to process, estimated ~26 MB of new deposits (uncapped)
[15:27:34] [Server thread/INFO] [LSS/]: Dirty content filter: seeded 49 already-loaded chunk(s)
[15:27:34] [Server thread/INFO] [minecraft/GameTestServer]: 15 tests are now running at position -373857, -59, -4076138!
[15:27:35] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyStorage:0' (3 tests)...
[15:27:35] [Server thread/INFO] [minecraft/GameTestServer]: [               ]
[15:27:35] [Server thread/INFO] [minecraft/GameTestServer]: [               ]
[15:27:35] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyArchiveLifecycle:0' (1 tests)...
[15:27:35] [Server thread/INFO] [minecraft/GameTestServer]: [+++            ]
[15:27:35] [Server thread/INFO] [minecraft/GameTestServer]: [+++            ]
[15:27:35] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 1 at (-3.5, -60.0, 6.5)
[15:27:36] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
[15:27:36] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 2 at (-8.5, -60.0, -1.5)
[15:27:36] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
[15:27:36] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'defaultBatch:0' (11 tests)...
[15:27:36] [Server thread/INFO] [minecraft/GameTestServer]: [++++           ]
[15:27:36] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 3 at (1.5, -60.0, -5.5)
[15:27:36] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
[15:27:36] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v9999, capabilities=1)
[15:27:36] [Server thread/WARN] [LSS/]: Player test-mock-player has incompatible LSS protocol version 9999 (server: 20), skipping LOD distribution
[15:27:36] [Server thread/WARN] [LSS/]: Auxiliary snapshot eligibility inspection failed; normal LOD delivery continues without archiving
java.lang.IllegalStateException: synthetic metadata observer failure
        at TRANSFORMER/lsstest@1.0.0/dev.vox.lss.neoforge.gametest.LSSNeoGameTests.lambda$generationObserverFailurePreservesNormalResult$7(LSSNeoGameTests.java:348) ~[%23134!/:?] {re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.ChunkGenerationService.tick(ChunkGenerationService.java:249) ~[%23135!/:?] {re:classloading}
        at TRANSFORMER/lsstest@1.0.0/dev.vox.lss.neoforge.gametest.LSSNeoGameTests.generationObserverFailurePreservesNormalResult(LSSNeoGameTests.java:356) ~[%23134!/:?] {re:classloading}
        at java.base/jdk.internal.reflect.DirectMethodHandleAccessor.invoke(DirectMethodHandleAccessor.java:103) ~[?:?] {}
        at java.base/java.lang.reflect.Method.invoke(Method.java:580) ~[?:?] {}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.gametest.framework.GameTestRegistry.lambda$turnMethodIntoConsumer$5(GameTestRegistry.java:157) ~[neoforge-21.1.267.jar%23132!/:?] {re:classloading}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.gametest.framework.TestFunction.run(TestFunction.java:40) ~[neoforge-21.1.267.jar%23132!/:?] {re:classloading}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.gametest.framework.GameTestInfo.startTest(GameTestInfo.java:162) ~[neoforge-21.1.267.jar%23132!/:?] {re:classloading,pl:accesstransformer:B}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.gametest.framework.GameTestInfo.tickInternal(GameTestInfo.java:124) ~[neoforge-21.1.267.jar%23132!/:?] {re:classloading,pl:accesstransformer:B}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.gametest.framework.GameTestInfo.tick(GameTestInfo.java:107) ~[neoforge-21.1.267.jar%23132!/:?] {re:classloading,pl:accesstransformer:B}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.gametest.framework.GameTestTicker.lambda$tick$0(GameTestTicker.java:39) ~[neoforge-21.1.267.jar%23132!/:?] {re:classloading}
        at java.base/java.util.concurrent.CopyOnWriteArrayList.forEach(CopyOnWriteArrayList.java:891) ~[?:?] {}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.gametest.framework.GameTestTicker.tick(GameTestTicker.java:39) ~[neoforge-21.1.267.jar%23132!/:?] {re:classloading}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.MinecraftServer.tickChildren(MinecraftServer.java:1055) ~[neoforge-21.1.267.jar%23132!/:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,pl:mixin:APP:lss.neoforge.mixins.json:ServerStopCompletionHook from mod lss,pl:mixin:A}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.MinecraftServer.tickServer(MinecraftServer.java:917) ~[neoforge-21.1.267.jar%23132!/:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,pl:mixin:APP:lss.neoforge.mixins.json:ServerStopCompletionHook from mod lss,pl:mixin:A}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.gametest.framework.GameTestServer.tickServer(GameTestServer.java:168) ~[neoforge-21.1.267.jar%23132!/:?] {re:classloading}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.MinecraftServer.runServer(MinecraftServer.java:707) ~[neoforge-21.1.267.jar%23132!/:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,pl:mixin:APP:lss.neoforge.mixins.json:ServerStopCompletionHook from mod lss,pl:mixin:A}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.MinecraftServer.lambda$spin$2(MinecraftServer.java:267) ~[neoforge-21.1.267.jar%23132!/:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,pl:mixin:APP:lss.neoforge.mixins.json:ServerStopCompletionHook from mod lss,pl:mixin:A}
        at java.base/java.lang.Thread.run(Thread.java:1583) [?:?] {}
[15:27:37] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 4 at (7.5, -60.0, 6.5)
[15:27:37] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
[15:27:37] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v20, capabilities=0)
[15:27:37] [Server thread/INFO] [LSS/]: Player test-mock-player has no LOD consumer (caps=0), skipping LOD registration
[15:27:37] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 5 at (4.5, -60.0, 9.5)
[15:27:37] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
[15:27:37] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v20, capabilities=1)
[15:27:37] [Server thread/INFO] [LSS/]: Player test-mock-player registered for LSS LOD request processing (caps=1)
[15:27:47] [LSS Store Backfill/WARN] [LSS/]: Store backfill: read failed at minecraft:overworld [696426,749056] — skipping
java.util.concurrent.TimeoutException: null
        at java.base/java.util.concurrent.CompletableFuture.timedGet(CompletableFuture.java:1960) ~[?:?] {}
        at java.base/java.util.concurrent.CompletableFuture.get(CompletableFuture.java:2095) ~[?:?] {}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.NbtSectionSerializer.readAndSerializeSections(NbtSectionSerializer.java:173) ~[%23135!/:?] {re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.NbtSectionSerializer.readAndSerializeSections(NbtSectionSerializer.java:159) ~[%23135!/:?] {re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.ChunkDiskReader.readColumnBytesSyncForBackfill(ChunkDiskReader.java:171) ~[%23135!/:?] {re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.RequestProcessingService.lambda$new$15(RequestProcessingService.java:600) ~[%23135!/:?] {re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.common.store.StoreBackfill.run(StoreBackfill.java:451) ~[%23135!/:?] {re:classloading}
        at java.base/java.lang.Thread.run(Thread.java:1583) [?:?] {}
[15:27:48] [Server thread/WARN] [minecraft/MinecraftServer]: Can't keep up! Is the server overloaded? Running 9227ms or 184 ticks behind
[15:27:48] [Server thread/INFO] [minecraft/GameTestServer]: [+++++++++++++++]
[15:27:48] [Server thread/INFO] [minecraft/GameTestServer]: ========= 15 GAME TESTS COMPLETE IN 14.85 s ======================
[15:27:48] [Server thread/INFO] [minecraft/GameTestServer]: All 15 required tests passed :)
[15:27:48] [Server thread/INFO] [minecraft/GameTestServer]: ====================================================
[15:27:48] [Server thread/INFO] [LSS/]: Stopping LSS LOD generation admissions before final world save
[15:27:48] [Server thread/INFO] [minecraft/MinecraftServer]: Stopping server
[15:27:48] [Server thread/INFO] [minecraft/MinecraftServer]: Saving players
[15:27:49] [Server thread/INFO] [minecraft/ServerGamePacketListenerImpl]: test-mock-player lost connection: Server closed
[15:27:49] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player left the game
[15:27:49] [Server thread/INFO] [minecraft/ServerGamePacketListenerImpl]: test-mock-player lost connection: Server closed
[15:27:49] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player left the game
[15:27:49] [Server thread/INFO] [minecraft/ServerGamePacketListenerImpl]: test-mock-player lost connection: Server closed
[15:27:49] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player left the game
[15:27:49] [Server thread/INFO] [minecraft/MinecraftServer]: Saving worlds
[15:27:48] [Server thread/INFO] [minecraft/MinecraftServer]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:overworld
[15:27:54] [Server thread/INFO] [minecraft/MinecraftServer]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:the_nether
[15:27:54] [Server thread/INFO] [minecraft/MinecraftServer]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:the_end
[15:27:54] [Server thread/INFO] [minecraft/MinecraftServer]: ThreadedAnvilChunkStorage (world): All chunks are saved
[15:27:54] [Server thread/INFO] [minecraft/MinecraftServer]: ThreadedAnvilChunkStorage (DIM-1): All chunks are saved
[15:27:54] [Server thread/INFO] [minecraft/MinecraftServer]: ThreadedAnvilChunkStorage (DIM1): All chunks are saved
[15:27:54] [Server thread/INFO] [minecraft/MinecraftServer]: ThreadedAnvilChunkStorage: All dimensions are saved
[15:27:54] [Server thread/INFO] [LSS/]: Stopping LSS LOD request processing service
[15:27:54] [LSS Store Backfill/INFO] [LSS/]: Store backfill stopped (shutdown): 2 regions, 16 deposited, 856 skipped, 1 errors
[15:27:54] [Server thread/INFO] [minecraft/GameTestServer]: Game test server shutting down

[Incubating] Problems report is available at: file:///home/wdzizon/lod-server-support-lod-only/build/reports/problems/problems-report.html

BUILD SUCCESSFUL in 44s
16 actionable tasks: 4 executed, 12 up-to-date
Consider enabling configuration cache to speed up this build: https://docs.gradle.org/9.5.1/userguide/configuration_cache_enabling.html
               wdzizon@DESKTOP-LS6DH9N:~/lod-server-support-lod-only$ cd ~/lod-server-support-lod-only &&
> git pull --ff-only origin feat/lod-only-preservation-1.21.1 &&
> ./gradlew :neoforge:test :neoforge:compileGametestJava :neoforge:runGameTestServer
remote: Enumerating objects: 98, done.
remote: Counting objects: 100% (98/98), done.
remote: Compressing objects: 100% (46/46), done.
remote: Total 70 (delta 23), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (70/70), 15.10 KiB | 351.00 KiB/s, done.
From https://github.com/WDzizon/lod-server-support-lod-only
 * branch                feat/lod-only-preservation-1.21.1 -> FETCH_HEAD
   54071c72a..ce49823b4  feat/lod-only-preservation-1.21.1 -> origin/feat/lod-only-preservation-1.21.1
Updating 54071c72a..ce49823b4
Fast-forward
 docs/planning/lod-only-preservation-plan.md                                                 |  68 +++++++++++++++++++++++++++++
 neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java               | 232 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++------------
 neoforge/src/main/java/dev/vox/lss/mixin/IOWorkerChunkIoGateMixin.java                      |  63 +++++++++++++++++++++++++++
 neoforge/src/main/java/dev/vox/lss/networking/server/NeoForgeChunkIoGate.java               | 325 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 neoforge/src/main/java/dev/vox/lss/networking/server/NeoForgeChunkRecordRemovalAdapter.java | 120 +++++++++++++++++++++++++++++++++++++--------------
 neoforge/src/main/resources/lss.neoforge.mixins.json                                        |   1 +
 neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreContractTest.java      |  55 +++++++++++++++++-------
 7 files changed, 788 insertions(+), 76 deletions(-)
 create mode 100644 neoforge/src/main/java/dev/vox/lss/mixin/IOWorkerChunkIoGateMixin.java
 create mode 100644 neoforge/src/main/java/dev/vox/lss/networking/server/NeoForgeChunkIoGate.java
│·······│·······│·······│██▌····│██▌····│█████··│█████··│█████··│█████··│█████··│█████··
> Configure project :fabric   > Evaluating se> root proje> :common > > :common > :fabric > :fabric                               > :fabric
Fabric Loom: 1.17.13
│██████│██████│████│█
> Configure project :spongenge
SpongePowered Plugin 'GRADLE' Toolset Version '2.3.0'
Targeting Minecraft '1.21.1' on a 'SERVER' platform
│▋······│████▎··│█████··│█████··│█████··│██████│████│████
> Task :neoforge:test FAILED

NeoForgeIOWorkerNullStoreContractTest > executableProbeUsesOnlyAnIsolatedTemporaryStorageDirectory() FAILED
    org.opentest4j.AssertionFailedError at NeoForgeIOWorkerNullStoreContractTest.java:54

54 tests completed, 1 failed

FAILURE: Build failed with an exception.

* What went wrong:
Execution failed for task ':neoforge:test'.
> There were failing tests. See the report at: file:///home/wdzizon/lod-server-support-lod-only/neoforge/build/reports/tests/test/index.html

* Try:
> Run with --scan to get full insights from a Build Scan (powered by Develocity).

BUILD FAILED in 7s
10 actionable tasks: 4 executed, 6 up-to-date
