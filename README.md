wdzizon@DESKTOP-LS6DH9N:~/lod-server-support-lod-only$ cd ~/lod-server-support-lod-only &&
> git pull --ff-only origin feat/lod-only-preservation-1.21.1 &&
> ./gradlew :common:test :neoforge:test :neoforge:compileGametestJava :neoforge:runGameTestServer :neoforge:build
remote: Enumerating objects: 52, done.
remote: Counting objects: 100% (52/52), done.
remote: Compressing objects: 100% (26/26), done.
remote: Total 33 (delta 12), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (33/33), 5.70 KiB | 37.00 KiB/s, done.
From https://github.com/WDzizon/lod-server-support-lod-only
 * branch                feat/lod-only-preservation-1.21.1 -> FETCH_HEAD
   680c48623..bb4763d7d  feat/lod-only-preservation-1.21.1 -> origin/feat/lod-only-preservation-1.21.1
Updating 680c48623..bb4763d7d
Fast-forward
 docs/planning/lod-only-preservation-plan.md                                       | 117 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java     |  17 +++++++++++++++++
 neoforge/src/main/java/dev/vox/lss/neoforge/NeoForgeOfflineWorldSessionLease.java |   8 ++++++--
 3 files changed, 140 insertions(+), 2 deletions(-)
│·······│██▌····│█████··│█████··│█████··│█████··│█████··│█████··│█████··│█████··│█████··│█████··│█████··
> Configure project :fabric> :common > :fabric > :fabric                               > :fabric > :fabric
Fabric Loom: 1.17.13
│██████│████│████│████│█│█
> Configure project :spongesponge
SpongePowered Plugin 'GRADLE' Toolset Version '2.3.0'
Targeting Minecraft '1.21.1' on a 'SERVER' platform
│███│███│███│███│███│███
> Task :neoforge:compileGametestJavaileGametestJava
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:286: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
            var firstPlayer = helper.makeMockServerPlayerInLevel();
                                    ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:307: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
            var secondPlayer = helper.makeMockServerPlayerInLevel();
                                     ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:424: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
        var player = helper.makeMockServerPlayerInLevel();
                           ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:440: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
        var player = helper.makeMockServerPlayerInLevel();
                           ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:457: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
        var player = helper.makeMockServerPlayerInLevel();
                           ^
5 warnings
│██│█│█│█│█│█
> Task :neoforge:runGameTestServer
WARN StatusConsoleListener Advanced terminal features are not available in this environment
│█│█[20:57:23] [main/INFO] [cp.mo.mo.Launcher/MODLAUNCHER]: ModLauncher running: args [--launchTarget, forgeserverdev, --gameDir, ., --fml.fmlVersion, 4.0.45, --fml.mcVersion, 1.21.1, --fml.neoForgeVersion, 21.1.267, --fml.neoFormVersion, 20240808.144430]
[20:57:23] [main/INFO] [cp.mo.mo.Launcher/MODLAUNCHER]: JVM identified as Ubuntu OpenJDK 64-Bit Server VM 21.0.13.1+2-1-24.04.1-Ubuntu
[20:57:23] [main/INFO] [cp.mo.mo.Launcher/MODLAUNCHER]: ModLauncher 11.0.5+main.901c6ea8 starting: java version 21.0.13.1 by Ubuntu; OS Linux arch amd64 version 6.18.40.1-microsoft-standard-WSL2
│█[20:57:23] [main/INFO] [ne.ne.fm.lo.ImmediateWindowHandler/]: ImmediateWindowProvider not loading because launch target is forgeserverdev
│█│█[20:57:23] [main/INFO] [mixin/]: SpongePowered MIXIN Subsystem Version=0.8.7 Source=union:/home/wdzizon/.gradle/caches/modules-2/files-2.1/net.fabricmc/sponge-mixin/0.16.4+mixin.0.8.7/26d01f0567ab46e9ca0d2ed89d0ecc11aadbd433/sponge-mixin-0.16.4+mixin.0.8.7.jar%2398!/ Service=ModLauncher Env=SERVER
│█│█[20:57:25] [main/INFO] [ne.ne.fm.lo.mo.lo.JarInJarDependencyLocator/]: Found 2 dependencies adding them to mods collection
[20:57:25] [main/INFO] [ne.ne.fm.lo.mo.ModDiscoverer/]:
     Mod List:
                Name Version (Mod Id)

                LOD Server Support 0.23.0 (lss)
                LSS NeoForge GameTests 1.0.0 (lsstest)
                Minecraft 1.21.1 (minecraft)
                NeoForge 21.1.267 (neoforge)
│█│█[20:57:26] [main/INFO] [mixin/]: Compatibility level set to JAVA_21
│█[20:57:26] [main/INFO] [cp.mo.mo.LaunchServiceHandler/MODLAUNCHER]: Launching target 'forgeserverdev' with arguments [--gameDir, .]
│█│█│█│█│█[20:57:31] [main/INFO] [MixinExtras|Service/]: Initializing MixinExtras via com.llamalad7.mixinextras.service.MixinExtrasServiceImpl(version=0.5.5).
│█│█│█│█│█│█│█│█│█│█│█│█│█│█│█│█│█│█[20:57:48] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, location] and [teleport, destination] with inputs: [0.1 -0.5 .9, 0 0 0]
[20:57:48] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, location] and [teleport, targets] with inputs: [0.1 -0.5 .9, 0 0 0]
│█[20:57:49] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, destination] and [teleport, targets] with inputs: [Player, 0123, @e, dd12be42-52a9-4a91-a8a1-11c01849e498]
[20:57:49] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, targets] and [teleport, destination] with inputs: [Player, 0123, dd12be42-52a9-4a91-a8a1-11c01849e498]
[20:57:49] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, targets, location] and [teleport, targets, destination] with inputs: [0.1 -0.5 .9, 0 0 0]
│█[20:57:49] [modloading-worker-0/INFO] [ne.ne.ne.co.NeoForgeMod/NEOFORGE-MOD]: NeoForge mod loading, version 21.1.267, for MC 1.21.1
│█│█│█[20:57:50] [main/INFO] [mojang/YggdrasilAuthenticationService]: Environment: Environment[sessionHost=https://sessionserver.mojang.com, servicesHost=https://api.minecraftservices.com, name=PROD]
│█[20:57:51] [main/WARN] [minecraft/VanillaPackResourcesBuilder]: Assets URL 'union:/home/wdzizon/lod-server-support-lod-only/neoforge/build/moddev/artifacts/neoforge-21.1.267.jar%23132!/assets/.mcassetsroot' uses unexpected schema
[20:57:51] [main/WARN] [minecraft/VanillaPackResourcesBuilder]: Assets URL 'union:/home/wdzizon/lod-server-support-lod-only/neoforge/build/moddev/artifacts/neoforge-21.1.267.jar%23132!/data/.mcassetsroot' uses unexpected schema
[20:57:51] [main/INFO] [ne.ne.ne.ga.GameTestHooks/]: Enabled Gametest Namespaces: [lsstest]
│█│█│█│█│█[20:57:52] [main/INFO] [minecraft/RecipeManager]: Loaded 1291 recipes
│█[20:57:53] [main/INFO] [minecraft/AdvancementTree]: Loaded 1400 advancements
│█│█│█│█[20:57:56] [Server thread/INFO] [minecraft/MinecraftServer]: Preparing start region for dimension minecraft:overworld
│█[20:57:57] [worldgen/INFO] [minecraft/LoggerChunkProgressListener]: Preparing spawn area: 2%
│█[20:57:57] [worldgen/INFO] [minecraft/LoggerChunkProgressListener]: Preparing spawn area: 87%
[20:57:57] [Server thread/INFO] [minecraft/LoggerChunkProgressListener]: Time elapsed: 552 ms
│█[20:57:57] [Server thread/INFO] [minecraft/GameTestServer]: Started game test server
[20:57:57] [Server thread/INFO] [ne.ne.ne.se.pe.PermissionAPI/]: Successfully initialized permission handler neoforge:default_handler
│█│█[20:57:58] [Server thread/INFO] [LSS/]: LOD-only durable archive ready: LOD-only archive: state=ready schema=2 queue=0/4096 visit_history=positive-only absence=unknown invalidations_pending=0 invalidation_jobs=0/0/0 invalidation_batches=0 archive_write_batches=0 invalidation_active=false invalidation_last_started_age_ms=-1 invalidation_last_completed_age_ms=-1 egress_invalidation_blocked=false egress_visit_publication_blocked=false archive_untrusted=false session_visits=0 session_visit_overflow=false session_invalidations=0 session_invalidation_overflow=false tracking_started_ms=1795867078717
[20:57:58] [Server thread/INFO] [LSS/]: Starting LSS LOD request processing service
│█│█[20:57:59] [Server thread/INFO] [LSS/]: LOD store active (driver=private/3.49.1.0). It stores served LOD bytes under <world>/lss-lod/ and, once fully warmed, occupies roughly as much space as the region files themselves. It is DERIVED data — deleting lss-lod/ is always safe. Set storage.lod_store.enabled to false and restart to disable; storage.lod_store.max_size_mib bounds its size after reload.
[20:57:59] [Server thread/INFO] [LSS/]: Effective config: useNbtTranscode=true, diskReaderThreads=3, useCompressedColumns=true, useBackgroundReadSplit=true, useSelectiveNbtParse=true, maxConcurrentDiskReads=2
[20:57:59] [LSS LOD Store SQLite/INFO] [LSS/]: LOD store sweep [minecraft:overworld]: 2 changed region(s), dropped 0 stale + 0 vanished-region row(s)
│█[20:57:59] [LSS Store Backfill/INFO] [LSS/]: Store backfill: 82 region(s) to process, estimated ~48 MB of new deposits (uncapped)
│█[20:57:59] [Server thread/INFO] [LSS/]: Dirty content filter: seeded 49 already-loaded chunk(s)
│█[20:58:00] [Server thread/INFO] [minecraft/GameTestServer]: 33 tests are now running at position -10517833, -59, -12695103!
│█│█[20:58:01] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyPoiMutation:0' (1 tests)...
│█[20:58:01] [Server thread/INFO] [minecraft/GameTestServer]: [                                 ]
│█[20:58:01] [Server thread/INFO] [minecraft/GameTestServer]: [                                 ]
│█[20:58:02] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyArchiveLifecycle:0' (1 tests)...
[20:58:02] [Server thread/INFO] [minecraft/GameTestServer]: [+                                ]
│█[20:58:02] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 1 at (-9.5, -60.0, -3.5)
│█│█[20:58:03] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
│█[20:58:03] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 2 at (7.5, -60.0, -9.5)
[20:58:03] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
│█[20:58:03] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlySideStoreCombined:0' (1 tests)...
│█[20:58:03] [Server thread/INFO] [minecraft/GameTestServer]: [++                               ]
│█[20:58:04] [Server thread/INFO] [minecraft/GameTestServer]: [++                               ]
│█[20:58:04] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyChunkMapMutation:0' (1 tests)...
│█[20:58:04] [Server thread/INFO] [minecraft/GameTestServer]: [+++                              ]
│█[20:58:04] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'defaultBatch:0' (12 tests)...
│█[20:58:04] [Server thread/INFO] [minecraft/GameTestServer]: [++++                             ]
│█[20:58:04] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 4 at (-6.5, -60.0, 5.5)
[20:58:04] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
[20:58:04] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v9999, capabilities=1)
[20:58:04] [Server thread/WARN] [LSS/]: Player test-mock-player has incompatible LSS protocol version 9999 (server: 20), skipping LOD distribution
│█│█│█│█[20:58:08] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 5 at (0.5, -60.0, -0.5)
[20:58:08] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
[20:58:08] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v20, capabilities=0)
[20:58:08] [Server thread/INFO] [LSS/]: Player test-mock-player has no LOD consumer (caps=0), skipping LOD registration
│█[20:58:08] [Server thread/WARN] [LSS/]: Auxiliary snapshot eligibility inspection failed; normal LOD delivery continues without archiving
java.lang.IllegalStateException: synthetic metadata observer failure
        at TRANSFORMER/lsstest@1.0.0/dev.vox.lss.neoforge.gametest.LSSNeoGameTests.lambda$generationObserverFailurePreservesNormalResult$7(LSSNeoGameTests.java:401) ~[%23134!/:?] {re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.ChunkGenerationService.tick(ChunkGenerationService.java:249) ~[%23135!/:?] {re:classloading}
        at TRANSFORMER/lsstest@1.0.0/dev.vox.lss.neoforge.gametest.LSSNeoGameTests.generationObserverFailurePreservesNormalResult(LSSNeoGameTests.java:409) ~[%23134!/:?] {re:classloading}
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
│█│█│█│█│█│█│█│█│█│█[20:58:18] [LSS Store Backfill/WARN] [LSS/]: Store backfill: read failed at minecraft:overworld [-156252,-253170] — skipping
java.util.concurrent.TimeoutException: null
        at java.base/java.util.concurrent.CompletableFuture.timedGet(CompletableFuture.java:1960) ~[?:?] {}
        at java.base/java.util.concurrent.CompletableFuture.get(CompletableFuture.java:2095) ~[?:?] {}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.NbtSectionSerializer.readAndSerializeSections(NbtSectionSerializer.java:173) ~[%23135!/:?] {re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.NbtSectionSerializer.readAndSerializeSections(NbtSectionSerializer.java:159) ~[%23135!/:?] {re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.ChunkDiskReader.readColumnBytesSyncForBackfill(ChunkDiskReader.java:171) ~[%23135!/:?] {re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.RequestProcessingService.lambda$new$15(RequestProcessingService.java:600) ~[%23135!/:?] {re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.common.store.StoreBackfill.run(StoreBackfill.java:451) ~[%23135!/:?] {re:classloading}
        at java.base/java.lang.Thread.run(Thread.java:1583) [?:?] {}
│█│█│█│█│█│█│█│█│█│█│█│█│█│█│█│█│█│█│█│█[20:58:35] [Server thread/WARN] [minecraft/MinecraftServer]: Can't keep up! Is the server overloaded? Running 30318ms or 606 ticks behind
│█[20:58:35] [Server thread/INFO] [minecraft/GameTestServer]: [+++++   _++++                    ]
│█[20:58:36] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 6 at (2.5, -60.0, 3.5)
[20:58:36] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
[20:58:36] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v20, capabilities=1)
[20:58:36] [Server thread/INFO] [LSS/]: Player test-mock-player registered for LSS LOD request processing (caps=1)
│█[20:58:36] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlySideStoreLifecycle:0' (1 tests)...
│█[20:58:36] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++++++++++                 ]
│█[20:58:36] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyCoordinatedRemoval:0' (1 tests)...
[20:58:36] [Server thread/INFO] [minecraft/GameTestServer]: [+++++++++++++++++                ]
│█[20:58:36] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyEntityStored:0' (1 tests)...
│█[20:58:36] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++++++++++++               ]
[20:58:36] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyEntityWorkerGate:0' (1 tests)...
[20:58:36] [Server thread/INFO] [minecraft/GameTestServer]: [+++++++++++++++++++              ]
│█[20:58:36] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyEntityMutation:0' (1 tests)...
[20:58:36] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++++++++++++++             ]
│█[20:58:36] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyPoiWorkerGate:0' (1 tests)...
[20:58:36] [Server thread/INFO] [minecraft/GameTestServer]: [+++++++++++++++++++++            ]
│█[20:58:36] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyBroadcast:0' (1 tests)...
[20:58:36] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++++++++++++++++           ]
│█│█[20:58:37] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyLiveChunkMapRemoval:0' (1 tests)...
│█[20:58:37] [Server thread/INFO] [minecraft/GameTestServer]: [+++++++++++++++++++++++          ]
[20:58:38] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyEntityAdmission:0' (1 tests)...
│█[20:58:38] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++++++++++++++++++         ]
[20:58:38] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++++++++++++++++++         ]
│█[20:58:38] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyStorage:0' (6 tests)...
[20:58:38] [Server thread/INFO] [minecraft/GameTestServer]: [+++++++++++++++++++++++++        ]
│█[20:58:38] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++++++++++++++++++++       ]
│█[20:58:39] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyOfflineWorldSessionLease:0' (1 tests)...
│█[20:58:39] [Server thread/INFO] [minecraft/GameTestServer]: [+++++++++++++++++++++++++++++++  ]
[20:58:39] [Server thread/INFO] [minecraft/GameTestServer]: [+++++++++++++++++++++++++++++++  ]
│█[20:58:39] [Server thread/ERROR] [minecraft/LogTestReporter]: offlineworldsessionleaserejectsconcurrentsessions failed at -10517791, -60, -12695082! offline world session lease GameTest failed: GameTestAssertException: the expected DirectoryLock side effect is its single-byte session marker
[20:58:39] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyTicketMutation:0' (1 tests)...
│█[20:58:39] [Server thread/INFO] [minecraft/GameTestServer]: [+++++++++++++++++++++++++++++++X ]
[20:58:39] [Server thread/INFO] [minecraft/GameTestServer]: [+++++++++++++++++++++++++++++++X+]
[20:58:39] [Server thread/INFO] [minecraft/GameTestServer]: ========= 33 GAME TESTS COMPLETE IN 41.78 s ======================
[20:58:39] [Server thread/INFO] [minecraft/GameTestServer]: 1 required tests failed :(
[20:58:39] [Server thread/INFO] [minecraft/GameTestServer]:    - offlineworldsessionleaserejectsconcurrentsessions
[20:58:39] [Server thread/INFO] [minecraft/GameTestServer]: ====================================================
│█[20:58:39] [Server thread/INFO] [LSS/]: Stopping LSS LOD generation admissions before final world save
[20:58:39] [Server thread/INFO] [minecraft/MinecraftServer]: Stopping server
[20:58:39] [Server thread/INFO] [minecraft/MinecraftServer]: Saving players
│█[20:58:40] [Server thread/INFO] [minecraft/ServerGamePacketListenerImpl]: test-mock-player lost connection: Server closed
[20:58:40] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player left the game
│█[20:58:40] [Server thread/INFO] [minecraft/ServerGamePacketListenerImpl]: test-mock-player lost connection: Server closed
[20:58:40] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player left the game
[20:58:40] [Server thread/INFO] [minecraft/ServerGamePacketListenerImpl]: test-mock-player lost connection: Server closed
[20:58:40] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player left the game
│█[20:58:40] [Server thread/INFO] [minecraft/MinecraftServer]: Saving worlds
│█[20:58:41] [Server thread/INFO] [minecraft/MinecraftServer]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:overworld
│█│█│█│█│█│█│█│█│█│█│█[20:58:51] [LSS Store Backfill/WARN] [LSS/]: Store backfill: read failed at minecraft:overworld [-156250,-253170] — skipping
java.util.concurrent.TimeoutException: null
        at java.base/java.util.concurrent.CompletableFuture.timedGet(CompletableFuture.java:1960) ~[?:?] {}
        at java.base/java.util.concurrent.CompletableFuture.get(CompletableFuture.java:2095) ~[?:?] {}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.NbtSectionSerializer.readAndSerializeSections(NbtSectionSerializer.java:173) ~[%23135!/:?] {re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.NbtSectionSerializer.readAndSerializeSections(NbtSectionSerializer.java:159) ~[%23135!/:?] {re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.ChunkDiskReader.readColumnBytesSyncForBackfill(ChunkDiskReader.java:171) ~[%23135!/:?] {re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.RequestProcessingService.lambda$new$15(RequestProcessingService.java:600) ~[%23135!/:?] {re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.common.store.StoreBackfill.run(StoreBackfill.java:451) ~[%23135!/:?] {re:classloading}
        at java.base/java.lang.Thread.run(Thread.java:1583) [?:?] {}
│█│█│█│█│█│█│█│█│█│█[20:58:59] [LSS Store Backfill/WARN] [LSS/]: Store backfill: read failed at minecraft:overworld [-156249,-253170] — skipping
java.util.concurrent.TimeoutException: null
        at java.base/java.util.concurrent.CompletableFuture.timedGet(CompletableFuture.java:1960) ~[?:?] {}
        at java.base/java.util.concurrent.CompletableFuture.get(CompletableFuture.java:2095) ~[?:?] {}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.NbtSectionSerializer.readAndSerializeSections(NbtSectionSerializer.java:173) ~[%23135!/:?] {re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.NbtSectionSerializer.readAndSerializeSections(NbtSectionSerializer.java:159) ~[%23135!/:?] {re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.ChunkDiskReader.readColumnBytesSyncForBackfill(ChunkDiskReader.java:171) ~[%23135!/:?] {re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.RequestProcessingService.lambda$new$15(RequestProcessingService.java:600) ~[%23135!/:?] {re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.common.store.StoreBackfill.run(StoreBackfill.java:451) ~[%23135!/:?] {re:classloading}
        at java.base/java.lang.Thread.run(Thread.java:1583) [?:?] {}
│█│█│█│█│█│█│█│█│█│█│█│█│█│█│█│█│█[20:59:15] [Server thread/INFO] [minecraft/MinecraftServer]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:the_end
[20:59:15] [Server thread/INFO] [minecraft/MinecraftServer]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:the_nether
│█[20:59:15] [Server thread/INFO] [minecraft/MinecraftServer]: ThreadedAnvilChunkStorage (world): All chunks are saved
[20:59:15] [Server thread/INFO] [minecraft/MinecraftServer]: ThreadedAnvilChunkStorage (DIM1): All chunks are saved
[20:59:15] [Server thread/INFO] [minecraft/MinecraftServer]: ThreadedAnvilChunkStorage (DIM-1): All chunks are saved
[20:59:15] [Server thread/INFO] [minecraft/MinecraftServer]: ThreadedAnvilChunkStorage: All dimensions are saved
│█[20:59:16] [Server thread/INFO] [LSS/]: Stopping LSS LOD request processing service
[20:59:16] [LSS Store Backfill/INFO] [LSS/]: Store backfill stopped: 0 regions, 6 deposited, 186 skipped, 4 errors, 41 pauses
[20:59:16] [Server thread/INFO] [minecraft/GameTestServer]: Game test server shutting down
│█│█
> Task :neoforge:runGameTestServer FAILED

[Incubating] Problems report is available at: file:///home/wdzizon/lod-server-support-lod-only/build/reports/problems/problems-report.html

FAILURE: Build failed with an exception.

* What went wrong:
Execution failed for task ':neoforge:runGameTestServer' (registered in build file 'neoforge/build.gradle').
> Process 'command '/usr/lib/jvm/java-21-openjdk-amd64/bin/java'' finished with non-zero exit value 1

* Try:
> Run with --stacktrace option to get the stack trace.
> Run with --info or --debug option to get more log output.
> Run with --scan to get full insights from a Build Scan (powered by Develocity).
> Get more help at https://help.gradle.org.

Deprecated Gradle features were used in this build, making it incompatible with Gradle 10.

You can use '--warning-mode all' to show the individual deprecation warnings and determine if they come from your own scripts or plugins.

For more on this, please refer to https://docs.gradle.org/9.5.1/userguide/command_line_interface.html#sec:command_line_warnings in the Gradle documentation.

BUILD FAILED in 2m 22s
24 actionable tasks: 5 executed, 19 up-to-date
