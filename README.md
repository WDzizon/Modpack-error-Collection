^Cwdzizon@DESKTOP-LS6DH9N:~/lod-server-support-lod-only$ cd ~/lod-server-support-lod-only &&
> git pull --ff-only origin feat/lod-only-preservation-1.21.1 &&
> ./gradlew :neoforge:test :neoforge:compileGametestJava :neoforge:runGameTestServer
remote: Enumerating objects: 38, done.
remote: Counting objects: 100% (38/38), done.
remote: Compressing objects: 100% (14/14), done.
remote: Total 23 (delta 6), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (23/23), 2.37 KiB | 201.00 KiB/s, done.
From https://github.com/WDzizon/lod-server-support-lod-only
 * branch                feat/lod-only-preservation-1.21.1 -> FETCH_HEAD
   1583e3094..142fc8b58  feat/lod-only-preservation-1.21.1 -> origin/feat/lod-only-preservation-1.21.1
Updating 1583e3094..142fc8b58
Fast-forward
 neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LodOnlyTwoPlayerConvergenceGameTest.java | 23 +++++++++++++----------
 neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeLodOnlyTwoPlayerConvergenceContractTest.java  |  5 +++--
 2 files changed, 16 insertions(+), 12 deletions(-)
│·······│·······│·······│·······│·······│·······│██▌····│██▌····│██▌····│██▌····│██▌····│█████··│█████··
> Configure project :fabric                                 > Evaluating settings         > Loading pr> :common > > :common > > :common                         > :fabric > :fabric
Fabric Loom: 1.17.13
│██████│████│█
> Configure project :sponge
SpongePowered Plugin 'GRADLE' Toolset Version '2.3.0'
Targeting Minecraft '1.21.1' on a 'SERVER' platform
│·······│████▎··│█████··│██████│████│████│████│████
> Task :neoforge:compileGametestJava                > :ne> IDLE
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:236: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
            var firstPlayer = helper.makeMockServerPlayerInLevel();
                                    ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:257: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
            var secondPlayer = helper.makeMockServerPlayerInLevel();
                                     ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:374: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
        var player = helper.makeMockServerPlayerInLevel();
                           ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:390: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
        var player = helper.makeMockServerPlayerInLevel();
                           ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:407: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
        var player = helper.makeMockServerPlayerInLevel();
                           ^
5 warnings

> Task :neoforge:runGameTestServer
WARN StatusConsoleListener Advanced terminal features are not available in this environment
[19:30:17] [main/INFO] [cp.mo.mo.Launcher/MODLAUNCHER]: ModLauncher running: args [--launchTarget, forgeserverdev, --gameDir, ., --fml.fmlVersion, 4.0.45, --fml.mcVersion, 1.21.1, --fml.neoForgeVersion, 21.1.267, --fml.neoFormVersion, 20240808.144430]
[19:30:17] [main/INFO] [cp.mo.mo.Launcher/MODLAUNCHER]: JVM identified as Ubuntu OpenJDK 64-Bit Server VM 21.0.13.1+2-1-24.04.1-Ubuntu
[19:30:17] [main/INFO] [cp.mo.mo.Launcher/MODLAUNCHER]: ModLauncher 11.0.5+main.901c6ea8 starting: java version 21.0.13.1 by Ubuntu; OS Linux arch amd64 version 6.18.40.1-microsoft-standard-WSL2
[19:30:17] [main/INFO] [ne.ne.fm.lo.ImmediateWindowHandler/]: ImmediateWindowProvider not loading because launch target is forgeserverdev
[19:30:17] [main/INFO] [mixin/]: SpongePowered MIXIN Subsystem Version=0.8.7 Source=union:/home/wdzizon/.gradle/caches/modules-2/files-2.1/net.fabricmc/sponge-mixin/0.16.4+mixin.0.8.7/26d01f0567ab46e9ca0d2ed89d0ecc11aadbd433/sponge-mixin-0.16.4+mixin.0.8.7.jar%2398!/ Service=ModLauncher Env=SERVER
[19:30:18] [main/INFO] [ne.ne.fm.lo.mo.lo.JarInJarDependencyLocator/]: Found 2 dependencies adding them to mods collection
[19:30:18] [main/INFO] [ne.ne.fm.lo.mo.ModDiscoverer/]:
     Mod List:
                Name Version (Mod Id)

                LOD Server Support 0.23.0 (lss)
                LSS NeoForge GameTests 1.0.0 (lsstest)
                Minecraft 1.21.1 (minecraft)
                NeoForge 21.1.267 (neoforge)
[19:30:19] [main/INFO] [mixin/]: Compatibility level set to JAVA_21
[19:30:19] [main/INFO] [cp.mo.mo.LaunchServiceHandler/MODLAUNCHER]: Launching target 'forgeserverdev' with arguments [--gameDir, .]
[19:30:20] [main/INFO] [MixinExtras|Service/]: Initializing MixinExtras via com.llamalad7.mixinextras.service.MixinExtrasServiceImpl(version=0.5.5).
[19:30:27] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, location] and [teleport, destination] with inputs: [0.1 -0.5 .9, 0 0 0]
[19:30:27] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, location] and [teleport, targets] with inputs: [0.1 -0.5 .9, 0 0 0]
[19:30:27] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, destination] and [teleport, targets] with inputs: [Player, 0123, @e, dd12be42-52a9-4a91-a8a1-11c01849e498]
[19:30:27] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, targets] and [teleport, destination] with inputs: [Player, 0123, dd12be42-52a9-4a91-a8a1-11c01849e498]
[19:30:27] [main/WARN] [minecraft/Commands]: Ambiguity between arguments [teleport, targets, location] and [teleport, targets, destination] with inputs: [0.1 -0.5 .9, 0 0 0]
[19:30:27] [modloading-worker-0/INFO] [ne.ne.ne.co.NeoForgeMod/NEOFORGE-MOD]: NeoForge mod loading, version 21.1.267, for MC 1.21.1
[19:30:27] [main/INFO] [mojang/YggdrasilAuthenticationService]: Environment: Environment[sessionHost=https://sessionserver.mojang.com, servicesHost=https://api.minecraftservices.com, name=PROD]
[19:30:27] [main/WARN] [minecraft/VanillaPackResourcesBuilder]: Assets URL 'union:/home/wdzizon/lod-server-support-lod-only/neoforge/build/moddev/artifacts/neoforge-21.1.267.jar%23132!/assets/.mcassetsroot' uses unexpected schema
[19:30:27] [main/WARN] [minecraft/VanillaPackResourcesBuilder]: Assets URL 'union:/home/wdzizon/lod-server-support-lod-only/neoforge/build/moddev/artifacts/neoforge-21.1.267.jar%23132!/data/.mcassetsroot' uses unexpected schema
[19:30:28] [main/INFO] [ne.ne.ne.ga.GameTestHooks/]: Enabled Gametest Namespaces: [lsstest]
[19:30:29] [main/INFO] [minecraft/RecipeManager]: Loaded 1291 recipes
[19:30:29] [main/INFO] [minecraft/AdvancementTree]: Loaded 1400 advancements
[19:30:30] [Server thread/INFO] [minecraft/MinecraftServer]: Preparing start region for dimension minecraft:overworld
[19:30:30] [worldgen/INFO] [minecraft/LoggerChunkProgressListener]: Preparing spawn area: 2%
[19:30:30] [Server thread/INFO] [minecraft/LoggerChunkProgressListener]: Time elapsed: 202 ms
[19:30:30] [Server thread/INFO] [minecraft/GameTestServer]: Started game test server
[19:30:30] [Server thread/INFO] [ne.ne.ne.se.pe.PermissionAPI/]: Successfully initialized permission handler neoforge:default_handler
[19:30:30] [Server thread/WARN] [LSS/]: LOD-only archive unavailable; historical player-visit state is uncertain and chunk deletion remains disabled | LOD-only recovery inspection: mode=filesystem-only auto_recovery=disabled directory=directory session_marker=regular(61B) invalidation_marker=missing archive_db=regular(28672B) wal=regular(20632B) shm=regular(32768B) journal=missing lock_file=regular(0B) operator_review=required
java.io.IOException: LOD-only archive has an unclean previous session marker; preserving the database and refusing to serve archived LOD
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.common.lodonly.LodOnlyArchiveStore.<init>(LodOnlyArchiveStore.java:326) ~[%23135!/:?] {re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.common.lodonly.LodOnlyArchiveStore.open(LodOnlyArchiveStore.java:279) ~[%23135!/:?] {re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.common.lodonly.LodOnlyArchiveStore.open(LodOnlyArchiveStore.java:275) ~[%23135!/:?] {re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.LSSServerNetworking.openLodOnlyArchive(LSSServerNetworking.java:72) ~[%23135!/:?] {re:mixin,re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.LSSServerNetworking.onServerStarted(LSSServerNetworking.java:214) ~[%23135!/:?] {re:mixin,re:classloading}
        at MC-BOOTSTRAP/net.neoforged.bus/net.neoforged.bus.ConsumerEventHandler.invoke(ConsumerEventHandler.java:27) ~[bus-8.0.5.jar%23110!/:?] {}
        at MC-BOOTSTRAP/net.neoforged.bus/net.neoforged.bus.EventBus.post(EventBus.java:360) ~[bus-8.0.5.jar%23110!/:?] {}
        at MC-BOOTSTRAP/net.neoforged.bus/net.neoforged.bus.EventBus.post(EventBus.java:328) ~[bus-8.0.5.jar%23110!/:?] {}
        at TRANSFORMER/neoforge@21.1.267/net.neoforged.neoforge.server.ServerLifecycleHooks.handleServerStarted(ServerLifecycleHooks.java:113) ~[neoforge-21.1.267.jar%23133!/:?] {re:classloading}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.MinecraftServer.runServer(MinecraftServer.java:674) ~[neoforge-21.1.267.jar%23132!/:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,pl:mixin:APP:lss.neoforge.mixins.json:ServerStopCompletionHook from mod lss,pl:mixin:A}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.MinecraftServer.lambda$spin$2(MinecraftServer.java:267) ~[neoforge-21.1.267.jar%23132!/:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,pl:mixin:APP:lss.neoforge.mixins.json:ServerStopCompletionHook from mod lss,pl:mixin:A}
        at java.base/java.lang.Thread.run(Thread.java:1583) [?:?] {}
[19:30:30] [Server thread/INFO] [LSS/]: Starting LSS LOD request processing service
[19:30:31] [Server thread/INFO] [LSS/]: LOD store active (driver=private/3.49.1.0). It stores served LOD bytes under <world>/lss-lod/ and, once fully warmed, occupies roughly as much space as the region files themselves. It is DERIVED data — deleting lss-lod/ is always safe. Set storage.lod_store.enabled to false and restart to disable; storage.lod_store.max_size_mib bounds its size after reload.
[19:30:31] [Server thread/INFO] [LSS/]: Effective config: useNbtTranscode=true, diskReaderThreads=3, useCompressedColumns=true, useBackgroundReadSplit=true, useSelectiveNbtParse=true, maxConcurrentDiskReads=2
[19:30:31] [LSS LOD Store SQLite/INFO] [LSS/]: LOD store sweep [minecraft:overworld]: 18 changed region(s), dropped 0 stale + 0 vanished-region row(s)
[19:30:31] [LSS Store Backfill/INFO] [LSS/]: Store backfill: 6 region(s) to process, estimated ~1 MB of new deposits (uncapped)
[19:30:31] [Server thread/INFO] [LSS/]: Dirty content filter: seeded 49 already-loaded chunk(s)
[19:30:31] [Server thread/INFO] [minecraft/GameTestServer]: 19 tests are now running at position -7530995, -59, -3797553!
[19:30:32] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyStorage:0' (6 tests)...
[19:30:32] [Server thread/INFO] [minecraft/GameTestServer]: [                   ]
[19:30:32] [Server thread/INFO] [minecraft/GameTestServer]: [                   ]
[19:30:32] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyArchiveLifecycle:0' (1 tests)...
[19:30:32] [Server thread/INFO] [minecraft/GameTestServer]: [++++++             ]
[19:30:32] [Server thread/ERROR] [minecraft/LogTestReporter]: playerwatchrecorderpersistsvisitandsuppressesarchivedlod failed at -7530959, -60, -3797553! the durable archive must be attached and healthy before a watch is recorded
[19:30:32] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'defaultBatch:0' (11 tests)...
[19:30:33] [Server thread/INFO] [minecraft/GameTestServer]: [++++++X            ]
[19:30:33] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 1 at (-7.5, -60.0, 7.5)
[19:30:33] [LSS Store Backfill/INFO] [LSS/]: Store backfill complete: 6 regions, 41 deposited, 661 skipped, 0 errors, 0 pauses
[19:30:33] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
[19:30:33] [Server thread/WARN] [LSS/]: LOD-only durable player-visit recording failed; visit history is untrusted and the affected world data must be preserved
java.lang.IllegalStateException: LOD-only durable visit archive is unavailable
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.ServerReceiverGlue.markPlayerWatched(ServerReceiverGlue.java:120) ~[%23135!/:?] {re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.LSSServerNetworking.onChunkWatch(LSSServerNetworking.java:205) ~[%23135!/:?] {re:mixin,re:classloading}
        at MC-BOOTSTRAP/net.neoforged.bus/net.neoforged.bus.ConsumerEventHandler.invoke(ConsumerEventHandler.java:27) ~[bus-8.0.5.jar%23110!/:?] {}
        at MC-BOOTSTRAP/net.neoforged.bus/net.neoforged.bus.EventBus.post(EventBus.java:360) ~[bus-8.0.5.jar%23110!/:?] {}
        at MC-BOOTSTRAP/net.neoforged.bus/net.neoforged.bus.EventBus.post(EventBus.java:328) ~[bus-8.0.5.jar%23110!/:?] {}
        at TRANSFORMER/neoforge@21.1.267/net.neoforged.neoforge.event.EventHooks.fireChunkWatch(EventHooks.java:806) ~[neoforge-21.1.267.jar%23133!/:?] {re:classloading}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.level.ChunkMap.markChunkPendingToSend(ChunkMap.java:826) ~[neoforge-21.1.267.jar%23132!/:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,pl:mixin:APP:lss.neoforge.mixins.json:AccessorChunkMapLifecycle from mod lss,pl:mixin:A}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.level.ChunkMap.markChunkPendingToSend(ChunkMap.java:820) ~[neoforge-21.1.267.jar%23132!/:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,pl:mixin:APP:lss.neoforge.mixins.json:AccessorChunkMapLifecycle from mod lss,pl:mixin:A}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.level.ChunkMap.lambda$applyChunkTrackingView$39(ChunkMap.java:1059) ~[neoforge-21.1.267.jar%23132!/:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,pl:mixin:APP:lss.neoforge.mixins.json:AccessorChunkMapLifecycle from mod lss,pl:mixin:A}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.level.ChunkTrackingView$Positioned.forEach(ChunkTrackingView.java:117) ~[neoforge-21.1.267.jar%23132!/:?] {re:classloading}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.level.ChunkTrackingView.difference(ChunkTrackingView.java:51) ~[neoforge-21.1.267.jar%23132!/:?] {re:classloading}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.level.ChunkMap.applyChunkTrackingView(ChunkMap.java:1058) ~[neoforge-21.1.267.jar%23132!/:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,pl:mixin:APP:lss.neoforge.mixins.json:AccessorChunkMapLifecycle from mod lss,pl:mixin:A}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.level.ChunkMap.updateChunkTracking(ChunkMap.java:1043) ~[neoforge-21.1.267.jar%23132!/:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,pl:mixin:APP:lss.neoforge.mixins.json:AccessorChunkMapLifecycle from mod lss,pl:mixin:A}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.level.ChunkMap.updatePlayerStatus(ChunkMap.java:980) ~[neoforge-21.1.267.jar%23132!/:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,pl:mixin:APP:lss.neoforge.mixins.json:AccessorChunkMapLifecycle from mod lss,pl:mixin:A}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.level.ChunkMap.addEntity(ChunkMap.java:1093) ~[neoforge-21.1.267.jar%23132!/:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,pl:mixin:APP:lss.neoforge.mixins.json:AccessorChunkMapLifecycle from mod lss,pl:mixin:A}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.level.ServerChunkCache.addEntity(ServerChunkCache.java:472) ~[neoforge-21.1.267.jar%23132!/:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,pl:mixin:APP:lss.neoforge.mixins.json:AccessorServerChunkCache from mod lss,pl:mixin:A}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.level.ServerLevel$EntityCallbacks.onTrackingStart(ServerLevel.java:1743) ~[neoforge-21.1.267.jar%23132!/:?] {re:classloading}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.level.ServerLevel$EntityCallbacks.onTrackingStart(ServerLevel.java:1726) ~[neoforge-21.1.267.jar%23132!/:?] {re:classloading}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.world.level.entity.PersistentEntitySectionManager.startTracking(PersistentEntitySectionManager.java:136) ~[neoforge-21.1.267.jar%23132!/:?] {re:classloading}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.world.level.entity.PersistentEntitySectionManager.addEntityWithoutEvent(PersistentEntitySectionManager.java:97) ~[neoforge-21.1.267.jar%23132!/:?] {re:classloading}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.world.level.entity.PersistentEntitySectionManager.addNewEntityWithoutEvent(PersistentEntitySectionManager.java:75) ~[neoforge-21.1.267.jar%23132!/:?] {re:classloading}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.level.ServerLevel.addPlayer(ServerLevel.java:926) ~[neoforge-21.1.267.jar%23132!/:?] {re:classloading,pl:accesstransformer:B,re:mixin,pl:accesstransformer:B}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.level.ServerLevel.addNewPlayer(ServerLevel.java:910) ~[neoforge-21.1.267.jar%23132!/:?] {re:classloading,pl:accesstransformer:B,re:mixin,pl:accesstransformer:B}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.players.PlayerList.placeNewPlayer(PlayerList.java:231) ~[neoforge-21.1.267.jar%23132!/:?] {re:classloading}
        at TRANSFORMER/minecraft@1.21.1/net.minecraft.gametest.framework.GameTestHelper.makeMockServerPlayerInLevel(GameTestHelper.java:308) ~[neoforge-21.1.267.jar%23132!/:?] {re:classloading,pl:accesstransformer:B}
        at TRANSFORMER/lsstest@1.0.0/dev.vox.lss.neoforge.gametest.LSSNeoGameTests.handshakeForeignVersionIsSilent(LSSNeoGameTests.java:390) ~[%23134!/:?] {re:classloading}
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
[19:30:33] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v9999, capabilities=1)
[19:30:33] [Server thread/WARN] [LSS/]: Player test-mock-player has incompatible LSS protocol version 9999 (server: 20), skipping LOD distribution
[19:30:33] [Server thread/INFO] [minecraft/GameTestServer]: [++++++X+           ]
[19:30:33] [Server thread/WARN] [LSS/]: Auxiliary snapshot eligibility inspection failed; normal LOD delivery continues without archiving
java.lang.IllegalStateException: synthetic metadata observer failure
        at TRANSFORMER/lsstest@1.0.0/dev.vox.lss.neoforge.gametest.LSSNeoGameTests.lambda$generationObserverFailurePreservesNormalResult$7(LSSNeoGameTests.java:351) ~[%23134!/:?] {re:classloading}
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.ChunkGenerationService.tick(ChunkGenerationService.java:249) ~[%23135!/:?] {re:classloading}
        at TRANSFORMER/lsstest@1.0.0/dev.vox.lss.neoforge.gametest.LSSNeoGameTests.generationObserverFailurePreservesNormalResult(LSSNeoGameTests.java:359) ~[%23134!/:?] {re:classloading}
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
[19:30:33] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 2 at (5.5, -60.0, -9.5)
[19:30:33] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
[19:30:33] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v20, capabilities=1)
[19:30:33] [Server thread/INFO] [LSS/]: Player test-mock-player registered for LSS LOD request processing (caps=1)
[19:30:34] [Server thread/INFO] [minecraft/PlayerList]: test-mock-player[embedded] logged in with entity id 3 at (0.5, -60.0, -5.5)
[19:30:34] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player joined the game
[19:30:34] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v20, capabilities=0)
[19:30:34] [Server thread/INFO] [LSS/]: Player test-mock-player has no LOD consumer (caps=0), skipping LOD registration
[19:30:34] [Server thread/ERROR] [minecraft/LogTestReporter]: durablelodonlyarchiveopensonserverstart failed at -7530953, -60, -3797546! the NeoForge ServerStartedEvent must open and attach the LOD-only archive
[19:30:34] [Server thread/INFO] [minecraft/GameTestServer]: [++++++X+++++_++X++ ]
[19:30:37] [Server thread/INFO] [minecraft/GameTestRunner]: Running test batch 'lodOnlyBroadcast:0' (1 tests)...
[19:30:37] [Server thread/INFO] [minecraft/GameTestServer]: [++++++X++++++++X++ ]
[19:30:37] [Server thread/INFO] [minecraft/GameTestServer]: [++++++X++++++++X+++]
[19:30:37] [Server thread/INFO] [minecraft/GameTestServer]: ========= 19 GAME TESTS COMPLETE IN 6.323 s ======================
[19:30:37] [Server thread/INFO] [minecraft/GameTestServer]: 2 required tests failed :(
[19:30:37] [Server thread/INFO] [minecraft/GameTestServer]:    - playerwatchrecorderpersistsvisitandsuppressesarchivedlod
[19:30:37] [Server thread/INFO] [minecraft/GameTestServer]:    - durablelodonlyarchiveopensonserverstart
[19:30:37] [Server thread/INFO] [minecraft/GameTestServer]: ====================================================
[19:30:37] [Server thread/INFO] [LSS/]: Stopping LSS LOD generation admissions before final world save
[19:30:37] [Server thread/INFO] [minecraft/MinecraftServer]: Stopping server
[19:30:37] [Server thread/INFO] [minecraft/MinecraftServer]: Saving players
[19:30:38] [Server thread/INFO] [minecraft/ServerGamePacketListenerImpl]: test-mock-player lost connection: Server closed
[19:30:38] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player left the game
[19:30:38] [Server thread/INFO] [minecraft/ServerGamePacketListenerImpl]: test-mock-player lost connection: Server closed
[19:30:38] [Server thread/INFO] [minecraft/MinecraftServer]: test-mock-player left the game
[19:30:38] [Server thread/INFO] [minecraft/MinecraftServer]: Saving worlds
[19:30:38] [Server thread/INFO] [minecraft/MinecraftServer]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:overworld
[19:30:42] [Server thread/INFO] [minecraft/MinecraftServer]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:the_nether
[19:30:42] [Server thread/INFO] [minecraft/MinecraftServer]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:the_end
[19:30:42] [Server thread/INFO] [minecraft/MinecraftServer]: ThreadedAnvilChunkStorage (world): All chunks are saved
[19:30:42] [Server thread/INFO] [minecraft/MinecraftServer]: ThreadedAnvilChunkStorage (DIM-1): All chunks are saved
[19:30:42] [Server thread/INFO] [minecraft/MinecraftServer]: ThreadedAnvilChunkStorage (DIM1): All chunks are saved
[19:30:42] [Server thread/INFO] [minecraft/MinecraftServer]: ThreadedAnvilChunkStorage: All dimensions are saved
[19:30:42] [Server thread/INFO] [LSS/]: Stopping LSS LOD request processing service
[19:30:42] [Server thread/INFO] [minecraft/GameTestServer]: Game test server shutting down

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

BUILD FAILED in 35s
16 actionable tasks: 4 executed, 12 up-to-date
