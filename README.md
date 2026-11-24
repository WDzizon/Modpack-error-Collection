[24Nov2026 14:12:51.328] [main/INFO] [cpw.mods.modlauncher.Launcher/MODLAUNCHER]: ModLauncher running: args [--launchTarget, forgeserverdev, --gameDir, ., --fml.fmlVersion, 4.0.43, --fml.mcVersion, 1.21.1, --fml.neoForgeVersion, 21.1.248, --fml.neoFormVersion, 20240808.144430]
[24Nov2026 14:12:51.331] [main/INFO] [cpw.mods.modlauncher.Launcher/MODLAUNCHER]: JVM identified as Ubuntu OpenJDK 64-Bit Server VM 21.0.13.1+2-1-24.04.1-Ubuntu
[24Nov2026 14:12:51.335] [main/INFO] [cpw.mods.modlauncher.Launcher/MODLAUNCHER]: ModLauncher 11.0.5+main.901c6ea8 starting: java version 21.0.13.1 by Ubuntu; OS Linux arch amd64 version 6.18.40.1-microsoft-standard-WSL2
[24Nov2026 14:12:51.561] [main/INFO] [net.neoforged.fml.loading.ImmediateWindowHandler/]: ImmediateWindowProvider not loading because launch target is forgeserverdev
[24Nov2026 14:12:51.656] [main/INFO] [mixin/]: SpongePowered MIXIN Subsystem Version=0.8.7 Source=union:/home/wdzizon/.gradle/caches/modules-2/files-2.1/net.fabricmc/sponge-mixin/0.15.2+mixin.0.8.7/2af2f021d8e02a0220dc27a7a72b4666d66d44ca/sponge-mixin-0.15.2+mixin.0.8.7.jar%2398!/ Service=ModLauncher Env=SERVER
[24Nov2026 14:12:52.082] [main/INFO] [net.neoforged.fml.loading.moddiscovery.locators.JarInJarDependencyLocator/]: Found 2 dependencies adding them to mods collection
[24Nov2026 14:12:52.085] [main/INFO] [net.neoforged.fml.loading.moddiscovery.ModDiscoverer/]: 
     Mod List:
		Name Version (Mod Id)

		LOD Server Support 0.23.0 (lss)
		LSS NeoForge GameTests 1.0.0 (lsstest)
		Minecraft 1.21.1 (minecraft)
		NeoForge 21.1.248 (neoforge)
[24Nov2026 14:12:52.921] [main/INFO] [mixin/]: Compatibility level set to JAVA_21
[24Nov2026 14:12:52.928] [main/INFO] [cpw.mods.modlauncher.LaunchServiceHandler/MODLAUNCHER]: Launching target 'forgeserverdev' with arguments [--gameDir, .]
[24Nov2026 14:12:54.103] [main/INFO] [MixinExtras|Service/]: Initializing MixinExtras via com.llamalad7.mixinextras.service.MixinExtrasServiceImpl(version=0.5.3).
[24Nov2026 14:13:01.198] [main/WARN] [net.minecraft.commands.Commands/]: Ambiguity between arguments [teleport, location] and [teleport, destination] with inputs: [0.1 -0.5 .9, 0 0 0]
[24Nov2026 14:13:01.202] [main/WARN] [net.minecraft.commands.Commands/]: Ambiguity between arguments [teleport, location] and [teleport, targets] with inputs: [0.1 -0.5 .9, 0 0 0]
[24Nov2026 14:13:01.208] [main/WARN] [net.minecraft.commands.Commands/]: Ambiguity between arguments [teleport, destination] and [teleport, targets] with inputs: [Player, 0123, @e, dd12be42-52a9-4a91-a8a1-11c01849e498]
[24Nov2026 14:13:01.212] [main/WARN] [net.minecraft.commands.Commands/]: Ambiguity between arguments [teleport, targets] and [teleport, destination] with inputs: [Player, 0123, dd12be42-52a9-4a91-a8a1-11c01849e498]
[24Nov2026 14:13:01.216] [main/WARN] [net.minecraft.commands.Commands/]: Ambiguity between arguments [teleport, targets, location] and [teleport, targets, destination] with inputs: [0.1 -0.5 .9, 0 0 0]
[24Nov2026 14:13:01.291] [modloading-worker-0/INFO] [net.neoforged.neoforge.common.NeoForgeMod/NEOFORGE-MOD]: NeoForge mod loading, version 21.1.248, for MC 1.21.1
[24Nov2026 14:13:01.711] [main/INFO] [com.mojang.authlib.yggdrasil.YggdrasilAuthenticationService/]: Environment: Environment[sessionHost=https://sessionserver.mojang.com, servicesHost=https://api.minecraftservices.com, name=PROD]
[24Nov2026 14:13:01.808] [main/WARN] [net.minecraft.server.packs.VanillaPackResourcesBuilder/]: Assets URL 'union:/home/wdzizon/lod-server-support-lod-only/neoforge/build/moddev/artifacts/neoforge-21.1.248.jar%23132!/assets/.mcassetsroot' uses unexpected schema
[24Nov2026 14:13:01.809] [main/WARN] [net.minecraft.server.packs.VanillaPackResourcesBuilder/]: Assets URL 'union:/home/wdzizon/lod-server-support-lod-only/neoforge/build/moddev/artifacts/neoforge-21.1.248.jar%23132!/data/.mcassetsroot' uses unexpected schema
[24Nov2026 14:13:01.817] [main/INFO] [net.neoforged.neoforge.gametest.GameTestHooks/]: Enabled Gametest Namespaces: [lsstest]
[24Nov2026 14:13:02.983] [main/INFO] [net.minecraft.world.item.crafting.RecipeManager/]: Loaded 1291 recipes
[24Nov2026 14:13:03.214] [main/INFO] [net.minecraft.advancements.AdvancementTree/]: Loaded 1400 advancements
[24Nov2026 14:13:04.274] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Preparing start region for dimension minecraft:overworld
[24Nov2026 14:13:04.353] [worldgen/INFO] [net.minecraft.server.level.progress.LoggerChunkProgressListener/]: Preparing spawn area: 2%
[24Nov2026 14:13:04.468] [Server thread/INFO] [net.minecraft.server.level.progress.LoggerChunkProgressListener/]: Time elapsed: 194 ms
[24Nov2026 14:13:04.482] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: Started game test server
[24Nov2026 14:13:04.506] [Server thread/INFO] [net.neoforged.neoforge.server.permission.PermissionAPI/]: Successfully initialized permission handler neoforge:default_handler
[24Nov2026 14:13:04.831] [Server thread/INFO] [LSS/]: LOD-only durable archive ready: LOD-only archive: state=ready schema=2 queue=0/4096 visit_history=positive-only absence=unknown invalidations_pending=0 egress_invalidation_blocked=false egress_visit_publication_blocked=false archive_untrusted=false session_visits=0 session_visit_overflow=false session_invalidations=0 session_invalidation_overflow=false tracking_started_ms=1795496799715
[24Nov2026 14:13:04.832] [Server thread/INFO] [LSS/]: Starting LSS LOD request processing service
[24Nov2026 14:13:05.052] [Server thread/INFO] [LSS/]: LOD store active (driver=private/3.49.1.0). It stores served LOD bytes under <world>/lss-lod/ and, once fully warmed, occupies roughly as much space as the region files themselves. It is DERIVED data — deleting lss-lod/ is always safe. Set storage.lod_store.enabled to false and restart to disable; storage.lod_store.max_size_mib bounds its size after reload.
[24Nov2026 14:13:05.057] [Server thread/INFO] [LSS/]: Effective config: useNbtTranscode=true, diskReaderThreads=3, useCompressedColumns=true, useBackgroundReadSplit=true, useSelectiveNbtParse=true, maxConcurrentDiskReads=2
[24Nov2026 14:13:05.061] [LSS Store Backfill/INFO] [LSS/]: Store backfill: 12 region(s) to process, estimated ~6 MB of new deposits (uncapped)
[24Nov2026 14:13:05.197] [Server thread/INFO] [LSS/]: Dirty content filter: seeded 49 already-loaded chunk(s)
[24Nov2026 14:13:05.275] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: 12 tests are now running at position -478326, -59, -4735456!
[24Nov2026 14:13:05.831] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestRunner/]: Running test batch 'lodOnlyArchiveLifecycle:0' (1 tests)...
[24Nov2026 14:13:05.951] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [            ]
[24Nov2026 14:13:06.286] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [            ]
[24Nov2026 14:13:06.332] [Server thread/ERROR] [net.minecraft.gametest.framework.LogTestReporter/]: playerwatchrecorderpersistsvisitandsuppressesarchivedlod failed at -478326, -60, -4735456! the test archive row must be visible before the watch signal
[24Nov2026 14:13:06.404] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestRunner/]: Running test batch 'defaultBatch:0' (11 tests)...
[24Nov2026 14:13:06.433] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [X           ]
[24Nov2026 14:13:06.648] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [X       +   ]
[24Nov2026 14:13:06.793] [Server thread/INFO] [net.minecraft.server.players.PlayerList/]: test-mock-player[embedded] logged in with entity id 1 at (0.5, -60.0, 8.5)
[24Nov2026 14:13:07.004] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: test-mock-player joined the game
[24Nov2026 14:13:07.028] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v9999, capabilities=1)
[24Nov2026 14:13:07.032] [Server thread/WARN] [LSS/]: Player test-mock-player has incompatible LSS protocol version 9999 (server: 20), skipping LOD distribution
[24Nov2026 14:13:07.038] [Server thread/WARN] [LSS/]: Auxiliary snapshot eligibility inspection failed; normal LOD delivery continues without archiving
java.lang.IllegalStateException: synthetic metadata observer failure
	at TRANSFORMER/lsstest@1.0.0/dev.vox.lss.neoforge.gametest.LSSNeoGameTests.lambda$generationObserverFailurePreservesNormalResult$7(LSSNeoGameTests.java:288) ~[%23134!/:?]
	at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.ChunkGenerationService.tick(ChunkGenerationService.java:245) ~[%23135!/:?]
	at TRANSFORMER/lsstest@1.0.0/dev.vox.lss.neoforge.gametest.LSSNeoGameTests.generationObserverFailurePreservesNormalResult(LSSNeoGameTests.java:296) ~[%23134!/:?]
	at java.base/jdk.internal.reflect.DirectMethodHandleAccessor.invoke(DirectMethodHandleAccessor.java:103) ~[?:?]
	at java.base/java.lang.reflect.Method.invoke(Method.java:580) ~[?:?]
	at TRANSFORMER/minecraft@1.21.1/net.minecraft.gametest.framework.GameTestRegistry.lambda$turnMethodIntoConsumer$5(GameTestRegistry.java:157) ~[neoforge-21.1.248.jar%23132!/:?]
	at TRANSFORMER/minecraft@1.21.1/net.minecraft.gametest.framework.TestFunction.run(TestFunction.java:40) ~[neoforge-21.1.248.jar%23132!/:?]
	at TRANSFORMER/minecraft@1.21.1/net.minecraft.gametest.framework.GameTestInfo.startTest(GameTestInfo.java:162) ~[neoforge-21.1.248.jar%23132!/:?]
	at TRANSFORMER/minecraft@1.21.1/net.minecraft.gametest.framework.GameTestInfo.tickInternal(GameTestInfo.java:124) ~[neoforge-21.1.248.jar%23132!/:?]
	at TRANSFORMER/minecraft@1.21.1/net.minecraft.gametest.framework.GameTestInfo.tick(GameTestInfo.java:107) ~[neoforge-21.1.248.jar%23132!/:?]
	at TRANSFORMER/minecraft@1.21.1/net.minecraft.gametest.framework.GameTestTicker.lambda$tick$0(GameTestTicker.java:39) ~[neoforge-21.1.248.jar%23132!/:?]
	at java.base/java.util.concurrent.CopyOnWriteArrayList.forEach(CopyOnWriteArrayList.java:891) ~[?:?]
	at TRANSFORMER/minecraft@1.21.1/net.minecraft.gametest.framework.GameTestTicker.tick(GameTestTicker.java:39) ~[neoforge-21.1.248.jar%23132!/:?]
	at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.MinecraftServer.tickChildren(MinecraftServer.java:1055) ~[neoforge-21.1.248.jar%23132!/:?]
	at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.MinecraftServer.tickServer(MinecraftServer.java:917) ~[neoforge-21.1.248.jar%23132!/:?]
	at TRANSFORMER/minecraft@1.21.1/net.minecraft.gametest.framework.GameTestServer.tickServer(GameTestServer.java:168) ~[neoforge-21.1.248.jar%23132!/:?]
	at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.MinecraftServer.runServer(MinecraftServer.java:707) ~[neoforge-21.1.248.jar%23132!/:?]
	at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.MinecraftServer.lambda$spin$2(MinecraftServer.java:267) ~[neoforge-21.1.248.jar%23132!/:?]
	at java.base/java.lang.Thread.run(Thread.java:1583) [?:?]
[24Nov2026 14:13:07.320] [Server thread/INFO] [net.minecraft.server.players.PlayerList/]: test-mock-player[embedded] logged in with entity id 2 at (-1.5, -60.0, -8.5)
[24Nov2026 14:13:07.324] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: test-mock-player joined the game
[24Nov2026 14:13:07.327] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v20, capabilities=1)
[24Nov2026 14:13:07.334] [Server thread/INFO] [LSS/]: Player test-mock-player registered for LSS LOD request processing (caps=1)
[24Nov2026 14:13:07.407] [Server thread/INFO] [net.minecraft.server.players.PlayerList/]: test-mock-player[embedded] logged in with entity id 3 at (-9.5, -60.0, 4.5)
[24Nov2026 14:13:07.409] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: test-mock-player joined the game
[24Nov2026 14:13:07.415] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v20, capabilities=0)
[24Nov2026 14:13:07.416] [Server thread/INFO] [LSS/]: Player test-mock-player has no LOD consumer (caps=0), skipping LOD registration
[24Nov2026 14:13:07.452] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [X+++++++++_+]
[24Nov2026 14:13:11.099] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [X+++++++++++]
[24Nov2026 14:13:11.101] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: ========= 12 GAME TESTS COMPLETE IN 5.824 s ======================
[24Nov2026 14:13:11.102] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: 1 required tests failed :(
[24Nov2026 14:13:11.102] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]:    - playerwatchrecorderpersistsvisitandsuppressesarchivedlod
[24Nov2026 14:13:11.103] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: ====================================================
[24Nov2026 14:13:11.109] [Server thread/INFO] [LSS/]: Preparing LSS LOD generation tickets for final world save
[24Nov2026 14:13:11.111] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping server
[24Nov2026 14:13:11.111] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving players
[24Nov2026 14:13:11.157] [Server thread/INFO] [net.minecraft.server.network.ServerGamePacketListenerImpl/]: test-mock-player lost connection: Server closed
[24Nov2026 14:13:11.157] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: test-mock-player left the game
[24Nov2026 14:13:11.176] [Server thread/INFO] [net.minecraft.server.network.ServerGamePacketListenerImpl/]: test-mock-player lost connection: Server closed
[24Nov2026 14:13:11.177] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: test-mock-player left the game
[24Nov2026 14:13:11.188] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving worlds
[24Nov2026 14:13:11.755] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:overworld
[24Nov2026 14:13:17.884] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:the_nether
[24Nov2026 14:13:17.892] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:the_end
[24Nov2026 14:13:17.923] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (world): All chunks are saved
[24Nov2026 14:13:17.923] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM-1): All chunks are saved
[24Nov2026 14:13:17.923] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM1): All chunks are saved
[24Nov2026 14:13:17.924] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage: All dimensions are saved
[24Nov2026 14:13:18.042] [Server thread/INFO] [LSS/]: Stopping LSS LOD request processing service
[24Nov2026 14:13:18.045] [LSS Store Backfill/INFO] [LSS/]: Store backfill stopped (shutdown): 3 regions, 90 deposited, 852 skipped, 0 errors
[24Nov2026 14:13:18.066] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: Game test server shutting down
