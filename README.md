wdzizon@DESKTOP-LS6DH9N:~/lod-server-support-lod-only$ cd ~/lod-server-support-lod-only &&
> git pull --ff-only origin feat/lod-only-preservation-1.21.1 &&
> ./gradlew :common:test :neoforge:test :neoforge:compileGametestJava :neoforge:runGameTestServer :neoforge:build
remote: Enumerating objects: 32, done.
remote: Counting objects: 100% (8/8), done.
remote: Total 32 (delta 7), reused 7 (delta 7), pack-reused 24 (from 1)
Unpacking objects: 100% (32/32), 62.68 KiB | 1.36 MiB/s, done.
From https://github.com/WDzizon/lod-server-support-lod-only
 * branch                feat/lod-only-preservation-1.21.1 -> FETCH_HEAD
   e66a0c9a9..ec3035f41  feat/lod-only-preservation-1.21.1 -> origin/feat/lod-only-preservation-1.21.1
Updating e66a0c9a9..ec3035f41
Fast-forward
 docs/planning/lod-only-preservation-plan.md                                            | 98 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeIOWorkerNullStoreContractTest.java | 28 ++++++++++++++++++++--------
 2 files changed, 118 insertions(+), 8 deletions(-)
│██▌····│█████··│█████··│█████··│█████··│█████··
> Configure project :fabricbric                     > :fabric > :fabric
Fabric Loom: 1.17.13
│████│████│█
> Configure project :sponge
SpongePowered Plugin 'GRADLE' Toolset Version '2.3.0'
Targeting Minecraft '1.21.1' on a 'SERVER' platform
│███│███
> Task :neoforge:compileGametestJava
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:284: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
            var firstPlayer = helper.makeMockServerPlayerInLevel();
                                    ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:305: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
            var secondPlayer = helper.makeMockServerPlayerInLevel();
                                     ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:422: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
        var player = helper.makeMockServerPlayerInLevel();
                           ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:438: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
        var player = helper.makeMockServerPlayerInLevel();
                           ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:455: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
        var player = helper.makeMockServerPlayerInLevel();
                           ^
5 warnings
│█│█│█│█
> Task :neoforge:runGameTestServer
WARN StatusConsoleListener Advanced terminal features are not available in this environment
[17:52:06] [main/INFO] [cp.mo.mo.Launcher/MODLAUNCHER]: ModLauncher running: args [--launchTarget, forgeserverdev, --gameDir, ., --fml.fmlVersion, 4.0.45, --fml.mcVersion, 1.21.1, --fml.neoForgeVersion, 21.1.267, --fml.neoFormVersion, 20240808.144430]
[17:52:06] [main/INFO] [cp.mo.mo.Launcher/MODLAUNCHER]: JVM identified as Ubuntu OpenJDK 64-Bit Server VM 21.0.13.1+2-1-24.04.1-Ubuntu
[17:52:06] [main/INFO] [cp.mo.mo.Launcher/MODLAUNCHER]: ModLauncher 11.0.5+main.901c6ea8 starting: java version 21.0.13.1 by Ubuntu; OS Linux arch amd64 version 6.18.40.1-microsoft-standard-WSL2
[17:52:06] [main/INFO] [ne.ne.fm.lo.ImmediateWindowHandler/]: ImmediateWindowProvider not loading because launch target is forgeserverdev
[17:52:07] [main/INFO] [mixin/]: SpongePowered MIXIN Subsystem Version=0.8.7 Source=union:/home/wdzizon/.gradle/caches/modules-2/files-2.1/net.fabricmc/sponge-mixin/0.16.4+mixin.0.8.7/26d01f0567ab46e9ca0d2ed89d0ecc11aadbd433/sponge-mixin-0.16.4+mixin.0.8.7.jar%2398!/ Service=ModLauncher Env=SERVER
[17:52:07] [main/INFO] [ne.ne.fm.lo.mo.lo.JarInJarDependencyLocator/]: Found 2 dependencies adding them to mods collection
[17:52:07] [main/INFO] [ne.ne.fm.lo.mo.ModDiscoverer/]:
     Mod List:
                Name Version (Mod Id)

                LOD Server Support 0.23.0 (lss)
                LSS NeoForge GameTests 1.0.0 (lsstest)
                Minecraft 1.21.1 (minecraft)
                NeoForge 21.1.267 (neoforge)
[17:52:07] [main/INFO] [mixin/]: Compatibility level set to JAVA_21
[17:52:07] [main/INFO] [cp.mo.mo.LaunchServiceHandler/MODLAUNCHER]: Launching target 'forgeserverdev' with arguments [--gameDir, .]
│█│█[17:52:09] [main/INFO] [MixinExtras|Service/]: Initializing MixinExtras via com.llamalad7.mixinextras.service.MixinExtrasServiceImpl(version=0.5.5).
│█│█│█│█│█│█│█[17:52:15] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, location] and [teleport, destination] with inputs: [0.1 -0.5 .9, 0 0 0]
[17:52:15] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, location] and [teleport, targets] with inputs: [0.1 -0.5 .9, 0 0 0]
[17:52:15] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, destination] and [teleport, targets] with inputs: [Player, 0123, @e, dd12be42-52a9-4a91-a8a1-11c01849e498]
[17:52:15] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, targets] and [teleport, destination] with inputs: [Player, 0123, dd12be42-52a9-4a91-a8a1-11c01849e498]
[17:52:15] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, targets, location] and [teleport, targets, destination] with inputs: [0.1 -0.5 .9, 0 0 0]
[17:52:15] [modloading-worker-0/INFO] [ne.ne.ne.co.NeoForgeMod/NEOFORGE-MOD]: NeoForge mod loading, version 21.1.267, for MC 1.21.1
│█[17:52:15] [main/INFO] [mojang/YggdrasilAuthenticationService]: Environment: Environment[sessionHost=https://sessionserver.mojang.com, servicesHost=https://api.minecraftservices.com, name=PROD]
│█│█[17:52:15] [main/WARN] [minecraft/VanillaPackResourcesBuilder]: Assets URL 'union:/home/wdzizon/lod-server-support-lod-only/neoforge/build/moddev/artifacts/neoforge-21.1.267.jar%23132!/assets/.mcassetsroot' uses unexpected schema
[17:52:15] [main/WARN] [minecraft/VanillaPackResourcesBuilder]: Assets URL 'union:/home/wdzizon/lod-server-support-lod-only/neoforge/build/moddev/artifacts/neoforge-21.1.267.jar%23132!/data/.mcassetsroot' uses unexpected schema
[17:52:15] [main/INFO] [ne.ne.ne.ga.GameTestHooks/]: Enabled Gametest Namespaces: [lsstest]
│█│█[17:52:17] [main/INFO] [minecraft/RecipeManager]: Loaded 1291 recipes
│█[17:52:17] [main/INFO] [minecraft/AdvancementTree]: Loaded 1400 advancements
│█│█[17:52:18] [Server thread/INFO] [minecraft/MinecraftServer]: Preparing start region for dimension minecraft:overworld
│█[17:52:18] [worldgen/INFO] [minecraft/LoggerChunkProgressListener]: Preparing spawn area: 2%
│█[17:52:18] [Server thread/INFO] [minecraft/LoggerChunkProgressListener]: Time elapsed: 198 ms
[17:52:18] [Server thread/INFO] [minecraft/GameTestServer]: Started game test server
[17:52:18] [Server thread/INFO] [ne.ne.ne.se.pe.PermissionAPI/]: Successfully initialized permission handler neoforge:default_handler
│█│█[17:52:18] [Server thread/INFO] [LSS/]: LOD-only durable archive ready: LOD-only archive: state=ready schema=2 queue=0/4096 visit_history=positive-only absence=unknown invalidations_pending=0 invalidation_jobs=0/0/0 invalidation_batches=0 archive_write_batches=0 invalidation_active=false invalidation_last_started_age_ms=-1 invalidation_last_completed_age_ms=-1 egress_invalidation_blocked=false egress_visit_publication_blocked=false archive_untrusted=false session_visits=0 session_visit_overflow=false session_invalidations=0 session_invalidation_overflow=false tracking_started_ms=1795855938921
[17:52:18] [Server thread/INFO] [LSS/]: Starting LSS LOD request processing service
│█[17:52:19] [Server thread/INFO] [LSS/]: LOD store active (driver=private/3.49.1.0). It stores served LOD bytes under <world>/lss-lod/ and, once fully warmed, occupies roughly as much space as the region files themselves. It is DERIVED data — deleting lss-lod/ is always safe. Set storage.lod_store.enabled to false and restart to disable; storage.lod_store.max_size_mib bounds its size after reload.
│█[17:52:19] [Server thread/INFO] [LSS/]: Effective config: useNbtTranscode=true, diskReaderThreads=3, useCompressedColumns=true, useBackgroundReadSplit=true, useSelectiveNbtParse=true, maxConcurrentDiskReads=2
[17:52:19] [LSS LOD Store SQLite/INFO] [LSS/]: LOD store sweep [minecraft:overworld]: 3 changed region(s), dropped 0 stale + 0 vanished-region row(s)
[17:52:19] [LSS Store Backfill/INFO] [LSS/]: Store backfill: 63 region(s) to process, estimated ~35 MB of new deposits (uncapped)
│█[17:52:19] [Server thread/INFO] [LSS/]: Dirty content filter: seeded 49 already-loaded chunk(s)
│█[17:52:19] [Server thread/INFO] [minecraft/GameTestServer]: 32 tests are now running at position 11464768, -59, 6785190!
│█│█[17:52:20] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyEntityAdmission:0' (1 tests)...
│█[17:52:20] [Server thread/INFO] [minecraft/GameTestServer]: [                                ]
│█[17:52:20] [Server thread/INFO] [minecraft/GameTestServer]: [                                ]
│█[17:52:20] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyStorage:0' (10 tests)...
│█[17:52:20] [Server thread/INFO] [minecraft/GameTestServer]: [+                               ]
[17:52:20] [Server thread/ERROR] [minecraft/LogTestReporter]: poimanagerflushusesindependentworkergate failed at 11464768, -60, 6785197! an IOWorker chunk-removal or shutdown lease is already active
│█[17:52:20] [Server thread/ERROR] [minecraft/LogTestReporter]: entitystoragestorewaitsbehindindependentworkergate failed at 11464780, -60, 6785197! an IOWorker chunk-removal or shutdown lease is already active
[17:52:20] [Server thread/INFO] [minecraft/GameTestServer]: [+++     X+X                     ]
│█[17:52:21] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyPoiMutation:0' (1 tests)...
│█[17:52:21] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++X+X                     ]
[17:52:21] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyArchiveLifecycle:0' (1 tests)...
[17:52:21] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++X+X+                    ]
│█[17:52:21] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 3 at (-9.5, -60.0, -8.5)
│█│█[17:52:21] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
│█[17:52:21] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 4 at (-9.5, -60.0, 8.5)
[17:52:21] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
[17:52:21] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlySideStoreCombined:0' (1 tests)...
│█[17:52:22] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++X+X++                   ]
│█[17:52:22] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyChunkMapMutation:0' (1 tests)...
│█[17:52:22] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++X+X+++                  ]
│█[17:52:22] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'defaultBatch:0' (12 tests)...
│█[17:52:22] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++X+X++++                 ]
│█[17:52:22] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 7 at (-0.5, -60.0, -0.5)
[17:52:22] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
[17:52:22] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v9999, capabilities=1)
[17:52:22] [Server thread/WARN] [LSS/]: Player test-mock-player has incompatible LSS protocol version 9999 (server: 20), skipping LOD distribution
[17:52:22] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++X+X+++++                ]
[17:52:22] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 8 at (2.5, -60.0, 6.5)
[17:52:22] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
[17:52:22] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v20, capabilities=1)
[17:52:22] [Server thread/INFO] [LSS/]: Player test-mock-player registered for LSS LOD request processing (caps=1)
│█│█[17:52:22] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 9 at (5.5, -60.0, 10.5)
[17:52:22] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
[17:52:22] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v20, capabilities=0)
[17:52:22] [Server thread/INFO] [LSS/]: Player test-mock-player has no LOD consumer (caps=0), skipping LOD registration
[17:52:22] [Server thread/WARN] [LSS/]: Auxiliary snapshot eligibility inspection failed; normal LOD delivery continues without archiving
java.lang.IllegalStateException: synthetic metadata observer failure
        at TRANSFORMER/lsstest@1.0.0/dev.vox.lss.neoforge.gametest.LSSNeoGameTests.lambda$generationObserverFailurePreservesNormalResult$7(LSSNeoGameTests.java:399) ~[%23134!/:?] {re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.ChunkGenerationService.tick(ChunkGenerationService.java:249) ~[%23135!/:?] {re:classloading}
        at TRANSFORMER/lsstest@1.0.0/dev.vox.lss.neoforge.gametest.LSSNeoGameTests.generationObserverFailurePreservesNormalResult(LSSNeoGameTests.java:407) ~[%23134!/:?] {re:classloading}
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
│█│█│█│█[17:52:26] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++X+X++++++++_+++++++     ]
[17:52:26] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlySideStoreLifecycle:0' (1 tests)...
│█[17:52:26] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++X+X++++++++++++++++     ]
[17:52:26] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyEntityStored:0' (1 tests)...
[17:52:26] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++X+X+++++++++++++++++    ]
[17:52:26] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyEntityMutation:0' (1 tests)...
[17:52:26] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++X+X++++++++++++++++++   ]
[17:52:26] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyTicketMutation:0' (1 tests)...
[17:52:26] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++X+X+++++++++++++++++++  ]
[17:52:26] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyBroadcast:0' (1 tests)...
│█[17:52:26] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++X+X++++++++++++++++++++ ]
│█[17:52:26] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++X+X+++++++++++++++++++++]
[17:52:26] [Server thread/INFO] [minecraft/GameTestServer]: ========= 32 GAME TESTS COMPLETE IN 6.901 s ======================
[17:52:26] [Server thread/INFO] [minecraft/GameTestServer]: 2 required tests failed :(
[17:52:26] [Server thread/INFO] [minecraft/GameTestServer]:    - poimanagerflushusesindependentworkergate
[17:52:26] [Server thread/INFO] [minecraft/GameTestServer]:    - entitystoragestorewaitsbehindindependentworkergate
[17:52:26] [Server thread/INFO] [minecraft/GameTestServer]: ====================================================
[17:52:26] [Server thread/INFO] [LSS/]: Stopping LSS LOD generation admissions before final world save
[17:52:26] [Server thread/INFO] [minecraft/MinecraftServer]: Stopping server
[17:52:26] [Server thread/INFO] [minecraft/MinecraftServer]: Saving players
│█[17:52:26] [Server thread/INFO] [minecraft/ServerGamePacketListenerImpl]: test-mock-player lost connection: Server closed
[17:52:26] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player left the game
[17:52:26] [Server thread/INFO] [minecraft/ServerGamePacketListenerImpl]: test-mock-player lost connection: Server closed
[17:52:26] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player left the game
[17:52:26] [Server thread/INFO] [minecraft/ServerGamePacketListenerImpl]: test-mock-player lost connection: Server closed
[17:52:26] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player left the game
[17:52:26] [Server thread/INFO] [minecraft/MinecraftServer]: Saving worlds
│█│█[17:52:26] [Server thread/INFO] [minecraft/MinecraftServer]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:overworld
│█│█│█│█[17:52:28] [Server thread/INFO] [minecraft/MinecraftServer]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:the_nether
[17:52:28] [Server thread/INFO] [minecraft/MinecraftServer]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:the_end
│█[17:52:28] [Server thread/INFO] [minecraft/MinecraftServer]: ThreadedAnvilChunkStorage (world): All chunks are saved
[17:52:28] [Server thread/INFO] [minecraft/MinecraftServer]: ThreadedAnvilChunkStorage (DIM-1): All chunks are saved
[17:52:28] [Server thread/INFO] [minecraft/MinecraftServer]: ThreadedAnvilChunkStorage (DIM1): All chunks are saved
[17:52:28] [Server thread/INFO] [minecraft/MinecraftServer]: ThreadedAnvilChunkStorage: All dimensions are saved
[17:52:28] [Server thread/INFO] [LSS/]: Stopping LSS LOD request processing service
[17:52:28] [LSS Store Backfill/INFO] [LSS/]: Store backfill stopped (shutdown): 1 regions, 0 deposited, 358 skipped, 0 errors
[17:52:28] [Server thread/INFO] [minecraft/GameTestServer]: Game test server shutting down
│█│█
> Task :neoforge:runGameTestServer FAILED

[Incubating] Problems report is available at: file:///home/wdzizon/lod-server-support-lod-only/build/reports/problems/problems-report.html

FAILURE: Build failed with an exception.

* What went wrong:
Execution failed for task ':neoforge:runGameTestServer' (registered in build file 'neoforge/build.gradle').
> Process 'command '/usr/lib/jvm/java-21-openjdk-amd64/bin/java'' finished with non-zero exit value 2

* Try:
> Run with --stacktrace option to get the stack trace.
> Run with --info or --debug option to get more log output.
> Run with --scan to get full insights from a Build Scan (powered by Develocity).
> Get more help at https://help.gradle.org.

Deprecated Gradle features were used in this build, making it incompatible with Gradle 10.

You can use '--warning-mode all' to show the individual deprecation warnings and determine if they come from your own scripts or plugins.

For more on this, please refer to https://docs.gradle.org/9.5.1/userguide/command_line_interface.html#sec:command_line_warnings in the Gradle documentation.

BUILD FAILED in 29s
24 actionable tasks: 4 executed, 20 up-to-date
               wdzizon@DESKTOP-LS6DH9N:~/lod-server-support-lod-only$ cd ~/lod-server-support-lod-only &&
> git pull --ff-only origin feat/lod-only-preservation-1.21.1 &&
> ./gradlew :common:test :neoforge:test :neoforge:compileGametestJava :neoforge:runGameTestServer :neoforge:build
From https://github.com/WDzizon/lod-server-support-lod-only
 * branch                feat/lod-only-preservation-1.21.1 -> FETCH_HEAD
Already up to date.
│█████··│█████··│█████··│█████··│█████··│█████··
> Configure project :fabric
Fabric Loom: 1.17.13
│████│█
> Configure project :sponge
SpongePowered Plugin 'GRADLE' Toolset Version '2.3.0'
Targeting Minecraft '1.21.1' on a 'SERVER' platform
│████···│█████▋·│█│█│█│█
> Task :neoforge:runGameTestServere:runGameTestServer
WARN StatusConsoleListener Advanced terminal features are not available in this environment
│█[18:10:35] [main/INFO] [cp.mo.mo.Launcher/MODLAUNCHER]: ModLauncher running: args [--launchTarget, forgeserverdev, --gameDir, ., --fml.fmlVersion, 4.0.45, --fml.mcVersion, 1.21.1, --fml.neoForgeVersion, 21.1.267, --fml.neoFormVersion, 20240808.144430]
[18:10:35] [main/INFO] [cp.mo.mo.Launcher/MODLAUNCHER]: JVM identified as Ubuntu OpenJDK 64-Bit Server VM 21.0.13.1+2-1-24.04.1-Ubuntu
│█[18:10:35] [main/INFO] [cp.mo.mo.Launcher/MODLAUNCHER]: ModLauncher 11.0.5+main.901c6ea8 starting: java version 21.0.13.1 by Ubuntu; OS Linux arch amd64 version 6.18.40.1-microsoft-standard-WSL2
│█│█[18:10:36] [main/INFO] [ne.ne.fm.lo.ImmediateWindowHandler/]: ImmediateWindowProvider not loading because launch target is forgeserverdev
│█[18:10:36] [main/INFO] [mixin/]: SpongePowered MIXIN Subsystem Version=0.8.7 Source=union:/home/wdzizon/.gradle/caches/modules-2/files-2.1/net.fabricmc/sponge-mixin/0.16.4+mixin.0.8.7/26d01f0567ab46e9ca0d2ed89d0ecc11aadbd433/sponge-mixin-0.16.4+mixin.0.8.7.jar%2398!/ Service=ModLauncher Env=SERVER
│█│█[18:10:37] [main/INFO] [ne.ne.fm.lo.mo.lo.JarInJarDependencyLocator/]: Found 2 dependencies adding them to mods collection
[18:10:37] [main/INFO] [ne.ne.fm.lo.mo.ModDiscoverer/]:
     Mod List:
                Name Version (Mod Id)

                LOD Server Support 0.23.0 (lss)
                LSS NeoForge GameTests 1.0.0 (lsstest)
                Minecraft 1.21.1 (minecraft)
                NeoForge 21.1.267 (neoforge)
│█│█│█[18:10:39] [main/INFO] [mixin/]: Compatibility level set to JAVA_21
[18:10:39] [main/INFO] [cp.mo.mo.LaunchServiceHandler/MODLAUNCHER]: Launching target 'forgeserverdev' with arguments [--gameDir, .]
│█│█[18:10:40] [main/INFO] [MixinExtras|Service/]: Initializing MixinExtras via com.llamalad7.mixinextras.service.MixinExtrasServiceImpl(version=0.5.5).
│█│█│█│█│█│█│█[18:10:47] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, location] and [teleport, destination] with inputs: [0.1 -0.5 .9, 0 0 0]
[18:10:47] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, location] and [teleport, targets] with inputs: [0.1 -0.5 .9, 0 0 0]
[18:10:47] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, destination] and [teleport, targets] with inputs: [Player, 0123, @e, dd12be42-52a9-4a91-a8a1-11c01849e498]
[18:10:47] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, targets] and [teleport, destination] with inputs: [Player, 0123, dd12be42-52a9-4a91-a8a1-11c01849e498]
[18:10:47] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, targets, location] and [teleport, targets, destination] with inputs: [0.1 -0.5 .9, 0 0 0]
│█[18:10:47] [modloading-worker-0/INFO] [ne.ne.ne.co.NeoForgeMod/NEOFORGE-MOD]: NeoForge mod loading, version 21.1.267, for MC 1.21.1
│█[18:10:47] [main/INFO] [mojang/YggdrasilAuthenticationService]: Environment: Environment[sessionHost=https://sessionserver.mojang.com, servicesHost=https://api.minecraftservices.com, name=PROD]
│█[18:10:47] [main/WARN] [minecraft/VanillaPackResourcesBuilder]: Assets URL 'union:/home/wdzizon/lod-server-support-lod-only/neoforge/build/moddev/artifacts/neoforge-21.1.267.jar%23132!/assets/.mcassetsroot' uses unexpected schema
[18:10:47] [main/WARN] [minecraft/VanillaPackResourcesBuilder]: Assets URL 'union:/home/wdzizon/lod-server-support-lod-only/neoforge/build/moddev/artifacts/neoforge-21.1.267.jar%23132!/data/.mcassetsroot' uses unexpected schema
│█[18:10:47] [main/INFO] [ne.ne.ne.ga.GameTestHooks/]: Enabled Gametest Namespaces: [lsstest]
│█│█│█[18:10:47] [main/INFO] [minecraft/RecipeManager]: Loaded 1291 recipes
│█[18:10:47] [main/INFO] [minecraft/AdvancementTree]: Loaded 1400 advancements
│█│█[18:10:48] [Server thread/INFO] [minecraft/MinecraftServer]: Preparing start region for dimension minecraft:overworld
│█[18:10:48] [worldgen/INFO] [minecraft/LoggerChunkProgressListener]: Preparing spawn area: 2%
│█[18:10:48] [Server thread/INFO] [minecraft/LoggerChunkProgressListener]: Time elapsed: 193 ms
[18:10:48] [Server thread/INFO] [minecraft/GameTestServer]: Started game test server
[18:10:49] [Server thread/INFO] [ne.ne.ne.se.pe.PermissionAPI/]: Successfully initialized permission handler neoforge:default_handler
│█[18:10:49] [Server thread/INFO] [LSS/]: LOD-only durable archive ready: LOD-only archive: state=ready schema=2 queue=0/4096 visit_history=positive-only absence=unknown invalidations_pending=0 invalidation_jobs=0/0/0 invalidation_batches=0 archive_write_batches=0 invalidation_active=false invalidation_last_started_age_ms=-1 invalidation_last_completed_age_ms=-1 egress_invalidation_blocked=false egress_visit_publication_blocked=false archive_untrusted=false session_visits=0 session_visit_overflow=false session_invalidations=0 session_invalidation_overflow=false tracking_started_ms=1795857049320
[18:10:49] [Server thread/INFO] [LSS/]: Starting LSS LOD request processing service
│█[18:10:49] [Server thread/INFO] [LSS/]: LOD store active (driver=private/3.49.1.0). It stores served LOD bytes under <world>/lss-lod/ and, once fully warmed, occupies roughly as much space as the region files themselves. It is DERIVED data — deleting lss-lod/ is always safe. Set storage.lod_store.enabled to false and restart to disable; storage.lod_store.max_size_mib bounds its size after reload.
[18:10:49] [Server thread/INFO] [LSS/]: Effective config: useNbtTranscode=true, diskReaderThreads=3, useCompressedColumns=true, useBackgroundReadSplit=true, useSelectiveNbtParse=true, maxConcurrentDiskReads=2
[18:10:49] [LSS Store Backfill/INFO] [LSS/]: Store backfill: 68 region(s) to process, estimated ~39 MB of new deposits (uncapped)
│█[18:10:49] [Server thread/INFO] [LSS/]: Dirty content filter: seeded 49 already-loaded chunk(s)
│█[18:10:49] [Server thread/INFO] [minecraft/GameTestServer]: 32 tests are now running at position -13354753, -59, -13498993!
│█[18:10:50] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyEntityAdmission:0' (1 tests)...
│█[18:10:50] [Server thread/INFO] [minecraft/GameTestServer]: [                                ]
│█[18:10:50] [Server thread/INFO] [minecraft/GameTestServer]: [                                ]
│█[18:10:50] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyStorage:0' (10 tests)...
[18:10:50] [Server thread/INFO] [minecraft/GameTestServer]: [+                               ]
│█[18:10:50] [Server thread/INFO] [minecraft/GameTestServer]: [+                               ]
│█[18:10:50] [Server thread/ERROR] [minecraft/LogTestReporter]: entitystoragestorewaitsbehindindependentworkergate failed at -13354741, -60, -13498986! an IOWorker chunk-removal or shutdown lease is already active
│█[18:10:51] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyPoiMutation:0' (1 tests)...
│█[18:10:51] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++++X                     ]
[18:10:51] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyArchiveLifecycle:0' (1 tests)...
│█[18:10:51] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++++X+                    ]
│█[18:10:51] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 3 at (3.5, -60.0, -3.5)
│█│█[18:10:51] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
│█[18:10:51] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 4 at (-1.5, -60.0, -6.5)
[18:10:51] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
[18:10:51] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlySideStoreCombined:0' (1 tests)...
│█[18:10:51] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++++X++                   ]
│█[18:10:51] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyChunkMapMutation:0' (1 tests)...
[18:10:51] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++++X+++                  ]
│█[18:10:52] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++++X+++                  ]
│█[18:10:52] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'defaultBatch:0' (12 tests)...
│█[18:10:52] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++++X++++                 ]
[18:10:52] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 7 at (-4.5, -60.0, 3.5)
[18:10:52] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
[18:10:52] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v9999, capabilities=1)
[18:10:52] [Server thread/WARN] [LSS/]: Player test-mock-player has incompatible LSS protocol version 9999 (server: 20), skipping LOD distribution
│█│█[18:10:52] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 8 at (-1.5, -60.0, 1.5)
[18:10:52] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
[18:10:52] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v20, capabilities=0)
[18:10:52] [Server thread/INFO] [LSS/]: Player test-mock-player has no LOD consumer (caps=0), skipping LOD registration
[18:10:52] [Server thread/WARN] [LSS/]: Auxiliary snapshot eligibility inspection failed; normal LOD delivery continues without archiving
java.lang.IllegalStateException: synthetic metadata observer failure
        at TRANSFORMER/lsstest@1.0.0/dev.vox.lss.neoforge.gametest.LSSNeoGameTests.lambda$generationObserverFailurePreservesNormalResult$7(LSSNeoGameTests.java:399) ~[%23134!/:?] {re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.ChunkGenerationService.tick(ChunkGenerationService.java:249) ~[%23135!/:?] {re:classloading}
        at TRANSFORMER/lsstest@1.0.0/dev.vox.lss.neoforge.gametest.LSSNeoGameTests.generationObserverFailurePreservesNormalResult(LSSNeoGameTests.java:407) ~[%23134!/:?] {re:classloading}
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
│█[18:10:52] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++++X++++++++_++++        ]
│█│█│█│█[18:10:55] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 9 at (-9.5, -60.0, 8.5)
[18:10:55] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
[18:10:55] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v20, capabilities=1)
[18:10:55] [Server thread/INFO] [LSS/]: Player test-mock-player registered for LSS LOD request processing (caps=1)
[18:10:55] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlySideStoreLifecycle:0' (1 tests)...
│█[18:10:56] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++++X++++++++++++++++     ]
[18:10:56] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyEntityStored:0' (1 tests)...
│█[18:10:56] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++++X+++++++++++++++++    ]
[18:10:56] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyEntityMutation:0' (1 tests)...
[18:10:56] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++++X++++++++++++++++++   ]
[18:10:56] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyTicketMutation:0' (1 tests)...
│█[18:10:56] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++++X+++++++++++++++++++  ]
[18:10:56] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyBroadcast:0' (1 tests)...
[18:10:56] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++++X++++++++++++++++++++ ]
│█[18:10:56] [Server thread/INFO] [minecraft/GameTestServer]: [++++++++++X+++++++++++++++++++++]
[18:10:56] [Server thread/INFO] [minecraft/GameTestServer]: ========= 32 GAME TESTS COMPLETE IN 6.692 s ======================
[18:10:56] [Server thread/INFO] [minecraft/GameTestServer]: 1 required tests failed :(
[18:10:56] [Server thread/INFO] [minecraft/GameTestServer]:    - entitystoragestorewaitsbehindindependentworkergate
[18:10:56] [Server thread/INFO] [minecraft/GameTestServer]: ====================================================
[18:10:56] [Server thread/INFO] [LSS/]: Stopping LSS LOD generation admissions before final world save
[18:10:56] [Server thread/INFO] [minecraft/MinecraftServer]: Stopping server
[18:10:56] [Server thread/INFO] [minecraft/MinecraftServer]: Saving players
│█[18:10:56] [Server thread/INFO] [minecraft/ServerGamePacketListenerImpl]: test-mock-player lost connection: Server closed
[18:10:56] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player left the game
[18:10:56] [Server thread/INFO] [minecraft/ServerGamePacketListenerImpl]: test-mock-player lost connection: Server closed
[18:10:56] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player left the game
[18:10:56] [Server thread/INFO] [minecraft/ServerGamePacketListenerImpl]: test-mock-player lost connection: Server closed
[18:10:56] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player left the game
│█[18:10:56] [Server thread/INFO] [minecraft/MinecraftServer]: Saving worlds
│█[18:10:57] [Server thread/INFO] [minecraft/MinecraftServer]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:overworld
│█│█│█│█[18:11:00] [Server thread/INFO] [minecraft/MinecraftServer]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:the_end
[18:11:00] [Server thread/INFO] [minecraft/MinecraftServer]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:the_nether
[18:11:00] [Server thread/INFO] [minecraft/MinecraftServer]: ThreadedAnvilChunkStorage (world): All chunks are saved
[18:11:00] [Server thread/INFO] [minecraft/MinecraftServer]: ThreadedAnvilChunkStorage (DIM1): All chunks are saved
[18:11:00] [Server thread/INFO] [minecraft/MinecraftServer]: ThreadedAnvilChunkStorage (DIM-1): All chunks are saved
[18:11:00] [Server thread/INFO] [minecraft/MinecraftServer]: ThreadedAnvilChunkStorage: All dimensions are saved
[18:11:00] [Server thread/INFO] [LSS/]: Stopping LSS LOD request processing service
[18:11:00] [LSS Store Backfill/INFO] [LSS/]: Store backfill stopped: 1 regions, 48 deposited, 630 skipped, 0 errors, 1 pauses
[18:11:00] [Server thread/INFO] [minecraft/GameTestServer]: Game test server shutting down
│█
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

BUILD FAILED in 29s
24 actionable tasks: 1 executed, 23 up-to-date
