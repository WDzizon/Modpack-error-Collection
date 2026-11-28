wdzizon@DESKTOP-LS6DH9N:~/lod-server-support-lod-only$ cd ~/lod-server-support-lod-only &&
> git pull --ff-only origin feat/lod-only-preservation-1.21.1 &&
> ./gradlew :common:test :neoforge:test :neoforge:compileGametestJava :neoforge:runGameTestServer :neoforge:build
remote: Enumerating objects: 86, done.
remote: Counting objects: 100% (86/86), done.
remote: Compressing objects: 100% (43/43), done.
remote: Total 58 (delta 21), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (58/58), 10.53 KiB | 371.00 KiB/s, done.
From https://github.com/WDzizon/lod-server-support-lod-only
 * branch                feat/lod-only-preservation-1.21.1 -> FETCH_HEAD
   4fc16a312..d12b9a956  feat/lod-only-preservation-1.21.1 -> origin/feat/lod-only-preservation-1.21.1
Updating 4fc16a312..d12b9a956
Fast-forward
 docs/planning/lod-only-preservation-plan.md                                 |  44 +++++++++++++
 .../src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java    |  65 ++++++++++++++++++++
 .../vox/lss/mixin/PersistentEntitySectionManagerCallbackMutationMixin.java  |  43 +++++++++++++
 .../vox/lss/mixin/PersistentEntitySectionManagerMutationTrackerMixin.java   | 119 ++++++++++++++++++++++++++++++++++++
 .../dev/vox/lss/networking/server/NeoForgeChunkSideStoreCoordinator.java    |  38 ++++++++++--
 .../vox/lss/networking/server/NeoForgeEntityLifecycleMutationTracker.java   | 102 +++++++++++++++++++++++++++++++
 neoforge/src/main/resources/lss.neoforge.mixins.json                        |   2 +
 .../dev/vox/lss/neoforge/NeoForgeChunkSideStoreCoordinatorContractTest.java |  47 ++++++++++++++
 8 files changed, 456 insertions(+), 4 deletions(-)
 create mode 100644 neoforge/src/main/java/dev/vox/lss/mixin/PersistentEntitySectionManagerCallbackMutationMixin.java
 create mode 100644 neoforge/src/main/java/dev/vox/lss/mixin/PersistentEntitySectionManagerMutationTrackerMixin.java
 create mode 100644 neoforge/src/main/java/dev/vox/lss/networking/server/NeoForgeEntityLifecycleMutationTracker.java
│█████··│█████··│█████··
> Configure project :fabricve > :fabric
Fabric Loom: 1.17.13
│██████│████│█
> Configure project :sponge
SpongePowered Plugin 'GRADLE' Toolset Version '2.3.0'
Targeting Minecraft '1.21.1' on a 'SERVER' platform
│███│███│███
> Task :neoforge:compileGametestJava
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:279: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
            var firstPlayer = helper.makeMockServerPlayerInLevel();
                                    ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:300: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
            var secondPlayer = helper.makeMockServerPlayerInLevel();
                                     ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:417: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
        var player = helper.makeMockServerPlayerInLevel();
                           ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:433: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
        var player = helper.makeMockServerPlayerInLevel();
                           ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:450: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
        var player = helper.makeMockServerPlayerInLevel();
                           ^
│███│███5 warnings
│███│██│█│█│█│█│█│█
> Task :neoforge:runGameTestServer
WARN StatusConsoleListener Advanced terminal features are not available in this environment
│█│█[14:57:13] [main/INFO] [cp.mo.mo.Launcher/MODLAUNCHER]: ModLauncher running: args [--launchTarget, forgeserverdev, --gameDir, ., --fml.fmlVersion, 4.0.45, --fml.mcVersion, 1.21.1, --fml.neoForgeVersion, 21.1.267, --fml.neoFormVersion, 20240808.144430]
[14:57:13] [main/INFO] [cp.mo.mo.Launcher/MODLAUNCHER]: JVM identified as Ubuntu OpenJDK 64-Bit Server VM 21.0.13.1+2-1-24.04.1-Ubuntu
│█[14:57:13] [main/INFO] [cp.mo.mo.Launcher/MODLAUNCHER]: ModLauncher 11.0.5+main.901c6ea8 starting: java version 21.0.13.1 by Ubuntu; OS Linux arch amd64 version 6.18.40.1-microsoft-standard-WSL2
│█│█[14:57:14] [main/INFO] [ne.ne.fm.lo.ImmediateWindowHandler/]: ImmediateWindowProvider not loading because launch target is forgeserverdev
│█[14:57:14] [main/INFO] [mixin/]: SpongePowered MIXIN Subsystem Version=0.8.7 Source=union:/home/wdzizon/.gradle/caches/modules-2/files-2.1/net.fabricmc/sponge-mixin/0.16.4+mixin.0.8.7/26d01f0567ab46e9ca0d2ed89d0ecc11aadbd433/sponge-mixin-0.16.4+mixin.0.8.7.jar%2398!/ Service=ModLauncher Env=SERVER
│█│█[14:57:15] [main/INFO] [ne.ne.fm.lo.mo.lo.JarInJarDependencyLocator/]: Found 2 dependencies adding them to mods collection
[14:57:15] [main/INFO] [ne.ne.fm.lo.mo.ModDiscoverer/]:
     Mod List:
                Name Version (Mod Id)

                LOD Server Support 0.23.0 (lss)
                LSS NeoForge GameTests 1.0.0 (lsstest)
                Minecraft 1.21.1 (minecraft)
                NeoForge 21.1.267 (neoforge)
│█│█[14:57:16] [main/INFO] [mixin/]: Compatibility level set to JAVA_21
[14:57:17] [main/INFO] [cp.mo.mo.LaunchServiceHandler/MODLAUNCHER]: Launching target 'forgeserverdev' with arguments [--gameDir, .]
│█│█│█│█[14:57:19] [main/INFO] [MixinExtras|Service/]: Initializing MixinExtras via com.llamalad7.mixinextras.service.MixinExtrasServiceImpl(version=0.5.5).
│█│█│█│█│█│█│█│█│█│█│█│█[14:57:29] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, location] and [teleport, destination] with inputs: [0.1 -0.5 .9, 0 0 0]
[14:57:29] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, location] and [teleport, targets] with inputs: [0.1 -0.5 .9, 0 0 0]
[14:57:29] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, destination] and [teleport, targets] with inputs: [Player, 0123, @e, dd12be42-52a9-4a91-a8a1-11c01849e498]
[14:57:29] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, targets] and [teleport, destination] with inputs: [Player, 0123, dd12be42-52a9-4a91-a8a1-11c01849e498]
[14:57:29] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, targets, location] and [teleport, targets, destination] with inputs: [0.1 -0.5 .9, 0 0 0]
│█[14:57:29] [modloading-worker-0/INFO] [ne.ne.ne.co.NeoForgeMod/NEOFORGE-MOD]: NeoForge mod loading, version 21.1.267, for MC 1.21.1
│█[14:57:29] [main/INFO] [mojang/YggdrasilAuthenticationService]: Environment: Environment[sessionHost=https://sessionserver.mojang.com, servicesHost=https://api.minecraftservices.com, name=PROD]
│█│█[14:57:30] [main/WARN] [minecraft/VanillaPackResourcesBuilder]: Assets URL 'union:/home/wdzizon/lod-server-support-lod-only/neoforge/build/moddev/artifacts/neoforge-21.1.267.jar%23132!/assets/.mcassetsroot' uses unexpected schema
[14:57:30] [main/WARN] [minecraft/VanillaPackResourcesBuilder]: Assets URL 'union:/home/wdzizon/lod-server-support-lod-only/neoforge/build/moddev/artifacts/neoforge-21.1.267.jar%23132!/data/.mcassetsroot' uses unexpected schema
[14:57:30] [main/INFO] [ne.ne.ne.ga.GameTestHooks/]: Enabled Gametest Namespaces: [lsstest]
│█│█│█[14:57:32] [main/INFO] [minecraft/RecipeManager]: Loaded 1291 recipes
│█[14:57:32] [main/INFO] [minecraft/AdvancementTree]: Loaded 1400 advancements
│█│█│█[14:57:34] [Server thread/INFO] [minecraft/MinecraftServer]: Preparing start region for dimension minecraft:overwo│█[14:57:34] [worldgen/INFO] [minecraft/LoggerChunkProgressListener]: Preparing spawn area: 2%
│█[14:57:35] [Server thread/INFO] [minecraft/LoggerChunkProgressListener]: Time elapsed: 490 ms
[14:57:35] [Server thread/INFO] [minecraft/GameTestServer]: Started game test server
│█[14:57:35] [Server thread/INFO] [ne.ne.ne.se.pe.PermissionAPI/]: Successfully initialized permission handler neoforge:default_handler
│█[14:57:35] [Server thread/INFO] [LSS/]: LOD-only durable archive ready: LOD-only archive: state=ready schema=2 queue=0/4096 visit_history=positive-only absence=unknown invalidations_pending=0 invalidation_jobs=0/0/0 invalidation_batches=0 archive_write_batches=0 invalidation_active=false invalidation_last_started_age_ms=-1 invalidation_last_completed_age_ms=-1 egress_invalidation_blocked=false egress_visit_publication_blocked=false archive_untrusted=false session_visits=0 session_visit_overflow=false session_invalidations=0 session_invalidation_overflow=false tracking_started_ms=1795845455734
[14:57:35] [Server thread/INFO] [LSS/]: Starting LSS LOD request processing service
│█[14:57:36] [Server thread/INFO] [LSS/]: LOD store active (driver=private/3.49.1.0). It stores served LOD bytes under <world>/lss-lod/ and, once fully warmed, occupies roughly as much space as the region files themselves. It is DERIVED data — deleting lss-lod/ is always safe. Set storage.lod_store.enabled to false and restart to disable; storage.lod_store.max_size_mib bounds its size after reload.
[14:57:36] [Server thread/INFO] [LSS/]: Effective config: useNbtTranscode=true, diskReaderThreads=3, useCompressedColumns=true, useBackgroundReadSplit=true, useSelectiveNbtParse=true, maxConcurrentDiskReads=2
[14:57:36] [LSS LOD Store SQLite/INFO] [LSS/]: LOD store sweep [minecraft:overworld]: 1 changed region(s), dropped 0 stale + 0 vanished-region row(s)
[14:57:36] [LSS Store Backfill/INFO] [LSS/]: Store backfill: 52 region(s) to process, estimated ~26 MB of new deposits (uncapped)
│█[14:57:36] [Server thread/INFO] [LSS/]: Dirty content filter: seeded 49 already-loaded chunk(s)
│█[14:57:36] [Server thread/INFO] [minecraft/GameTestServer]: 27 tests are now running at position -11291497, -59, 7180456!
│█[14:57:36] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyEntityAdmission:0' (1 tests)...
│█[14:57:37] [Server thread/INFO] [minecraft/GameTestServer]: [                           ]
[14:57:37] [Server thread/INFO] [minecraft/GameTestServer]: [                           ]
[14:57:37] [Server thread/INFO] [minecraft/GameTestServer]: [                           ]
│█[14:57:37] [Server thread/INFO] [minecraft/GameTestServer]: [                           ]
[14:57:37] [Server thread/INFO] [minecraft/GameTestServer]: [                           ]
[14:57:37] [Server thread/INFO] [minecraft/GameTestServer]: [                           ]
[14:57:37] [Server thread/INFO] [minecraft/GameTestServer]: [                           ]
[14:57:37] [Server thread/INFO] [minecraft/GameTestServer]: [                           ]
[14:57:37] [Server thread/INFO] [minecraft/GameTestServer]: [                           ]
│█[14:57:37] [Server thread/INFO] [minecraft/GameTestServer]: [                           ]
[14:57:37] [Server thread/INFO] [minecraft/GameTestServer]: [                           ]
[14:57:37] [Server thread/INFO] [minecraft/GameTestServer]: [                           ]
[14:57:37] [Server thread/INFO] [minecraft/GameTestServer]: [                           ]
│█[14:57:37] [Server thread/INFO] [minecraft/GameTestServer]: [                           ]
[14:57:37] [Server thread/INFO] [minecraft/GameTestServer]: [                           ]
[14:57:37] [Server thread/INFO] [minecraft/GameTestServer]: [                           ]
[14:57:37] [Server thread/INFO] [minecraft/GameTestServer]: [                           ]
[14:57:37] [Server thread/INFO] [minecraft/GameTestServer]: [                           ]
│█[14:57:37] [Server thread/INFO] [minecraft/GameTestServer]: [                           ]
[14:57:37] [Server thread/INFO] [minecraft/GameTestServer]: [                           ]
[14:57:37] [Server thread/INFO] [minecraft/GameTestServer]: [                           ]
│█[14:57:37] [Server thread/INFO] [minecraft/GameTestServer]: [                           ]
│█[14:57:37] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyStorage:0' (9 tests)...
[14:57:37] [Server thread/INFO] [minecraft/GameTestServer]: [+                          ]
│█[14:57:38] [Server thread/INFO] [minecraft/GameTestServer]: [+++++++ ++                 ]
[14:57:38] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyArchiveLifecycle:0' (1 tests)...
│█[14:57:38] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++++                 ]
│█[14:57:38] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 4 at (0.5, -60.0, 9.5)
│█[14:57:38] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
│█[14:57:38] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 5 at (4.5, -60.0, -4.5)
[14:57:38] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
[14:57:38] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlySideStoreCombined:0' (1 tests)...
│█[14:57:38] [Server thread/INFO] [minecraft/GameTestServer]: [+++++++++++                ]
│█[14:57:38] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'defaultBatch:0' (12 tests)...
│█[14:57:39] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++++++               ]
[14:57:39] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 6 at (8.5, -60.0, 9.5)
[14:57:39] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
│█[14:57:39] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v9999, capabilities=1)
[14:57:39] [Server thread/WARN] [LSS/]: Player test-mock-player has incompatible LSS protocol version 9999 (server: 20), skipping LOD distribution
[14:57:39] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++++++++++           ]
│█[14:57:39] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 7 at (3.5, -60.0, -5.5)
[14:57:39] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
[14:57:39] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v20, capabilities=0)
[14:57:39] [Server thread/INFO] [LSS/]: Player test-mock-player has no LOD consumer (caps=0), skipping LOD registration
[14:57:40] [Server thread/WARN] [LSS/]: Auxiliary snapshot eligibility inspection failed; normal LOD delivery continues without archiving
java.lang.IllegalStateException: synthetic metadata observer failure
        at TRANSFORMER/lsstest@1.0.0/dev.vox.lss.neoforge.gametest.LSSNeoGameTests.lambda$generationObserverFailurePreservesNormalResult$7(LSSNeoGameTests.java:394) ~[%23134!/:?] {re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.ChunkGenerationService.tick(ChunkGenerationService.java:249) ~[%23135!/:?] {re:classloading}
        at TRANSFORMER/lsstest@1.0.0/dev.vox.lss.neoforge.gametest.LSSNeoGameTests.generationObserverFailurePreservesNormalResult(LSSNeoGameTests.java:402) ~[%23134!/:?] {re:classloading}
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
│█[14:57:40] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 8 at (-9.5, -60.0, -7.5)
[14:57:40] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
[14:57:40] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v20, capabilities=1)
[14:57:40] [Server thread/INFO] [LSS/]: Player test-mock-player registered for LSS LOD request processing (caps=1)
│█│█│█│█│█│█[14:57:45] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlySideStoreLifecycle:0' (1 tests)...
│█[14:57:45] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++++++++++++++++++   ]
[14:57:45] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyEntityMutation:0' (1 tests)...
[14:57:45] [Server thread/INFO] [minecraft/GameTestServer]: [+++++++++++++++++++++++++  ]
│█[14:57:45] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyBroadcast:0' (1 tests)...
[14:57:45] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++++++++++++++++++++ ]
│█[14:57:45] [Server thread/INFO] [minecraft/GameTestServer]: [+++++++++++++++++++++++++++]
[14:57:45] [Server thread/INFO] [minecraft/GameTestServer]: ========= 27 GAME TESTS COMPLETE IN 9.072 s ======================
[14:57:45] [Server thread/INFO] [minecraft/GameTestServer]: All 27 required tests passed :)
[14:57:45] [Server thread/INFO] [minecraft/GameTestServer]: ====================================================
[14:57:45] [Server thread/INFO] [LSS/]: Stopping LSS LOD generation admissions before final world save
[14:57:45] [Server thread/INFO] [minecraft/MinecraftServer]: Stopping server
[14:57:45] [Server thread/INFO] [minecraft/MinecraftServer]: Saving players
│█[14:57:45] [Server thread/INFO] [minecraft/ServerGamePacketListenerImpl]: test-mock-player lost connection: Server closed
[14:57:45] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player left the game
[14:57:45] [Server thread/INFO] [minecraft/ServerGamePacketListenerImpl]: test-mock-player lost connection: Server closed
[14:57:45] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player left the game
│█[14:57:45] [Server thread/INFO] [minecraft/ServerGamePacketListenerImpl]: test-mock-player lost connection: Server closed
[14:57:45] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player left the game
│█[14:57:45] [Server thread/INFO] [minecraft/MinecraftServer]: Saving worlds
│█[14:57:46] [Server thread/INFO] [minecraft/MinecraftServer]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:overworld
│█│█│█│█│█│█[14:57:50] [Server thread/INFO] [minecraft/MinecraftServer]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:the_nether
[14:57:50] [Server thread/INFO] [minecraft/MinecraftServer]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:the_end
│█[14:57:50] [Server thread/INFO] [minecraft/MinecraftServer]: ThreadedAnvilChunkStorage (world): All chunks are saved
[14:57:50] [Server thread/INFO] [minecraft/MinecraftServer]: ThreadedAnvilChunkStorage (DIM-1): All chunks are saved
[14:57:50] [Server thread/INFO] [minecraft/MinecraftServer]: ThreadedAnvilChunkStorage (DIM1): All chunks are saved
[14:57:50] [Server thread/INFO] [minecraft/MinecraftServer]: ThreadedAnvilChunkStorage: All dimensions are saved
[14:57:51] [Server thread/INFO] [LSS/]: Stopping LSS LOD request processing service
[14:57:51] [LSS Store Backfill/INFO] [LSS/]: Store backfill stopped (shutdown): 4 regions, 1 deposited, 765 skipped, 0 errors
[14:57:51] [Server thread/INFO] [minecraft/GameTestServer]: Game test server shutting down
│█
[Incubating] Problems report is available at: file:///home/wdzizon/lod-server-support-lod-only/build/reports/problems/problems-report.html

Deprecated Gradle features were used in this build, making it incompatible with Gradle 10.

You can use '--warning-mode all' to show the individual deprecation warnings and determine if they come from your own scripts or plugins.

For more on this, please refer to https://docs.gradle.org/9.5.1/userguide/command_line_interface.html#sec:command_line_warnings in the Gradle documentation.

BUILD SUCCESSFUL in 54s
25 actionable tasks: 8 executed, 17 up-to-date
