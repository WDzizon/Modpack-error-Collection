[24Nov2026 23:15:56.858] [main/INFO] [cpw.mods.modlauncher.Launcher/MODLAUNCHER]: ModLauncher running: args [--launchTarget, forgeserverdev, --gameDir, ., --fml.fmlVersion, 4.0.45, --fml.mcVersion, 1.21.1, --fml.neoForgeVersion, 21.1.267, --fml.neoFormVersion, 20240808.144430]
[24Nov2026 23:15:56.862] [main/INFO] [cpw.mods.modlauncher.Launcher/MODLAUNCHER]: JVM identified as Ubuntu OpenJDK 64-Bit Server VM 21.0.13.1+2-1-24.04.1-Ubuntu
[24Nov2026 23:15:56.864] [main/INFO] [cpw.mods.modlauncher.Launcher/MODLAUNCHER]: ModLauncher 11.0.5+main.901c6ea8 starting: java version 21.0.13.1 by Ubuntu; OS Linux arch amd64 version 6.18.40.1-microsoft-standard-WSL2
[24Nov2026 23:15:56.991] [main/INFO] [net.neoforged.fml.loading.ImmediateWindowHandler/]: ImmediateWindowProvider not loading because launch target is forgeserverdev
[24Nov2026 23:15:57.042] [main/INFO] [mixin/]: SpongePowered MIXIN Subsystem Version=0.8.7 Source=union:/home/wdzizon/.gradle/caches/modules-2/files-2.1/net.fabricmc/sponge-mixin/0.16.4+mixin.0.8.7/26d01f0567ab46e9ca0d2ed89d0ecc11aadbd433/sponge-mixin-0.16.4+mixin.0.8.7.jar%2398!/ Service=ModLauncher Env=SERVER
[24Nov2026 23:15:57.375] [main/INFO] [net.neoforged.fml.loading.moddiscovery.locators.JarInJarDependencyLocator/]: Found 2 dependencies adding them to mods collection
[24Nov2026 23:15:57.377] [main/INFO] [net.neoforged.fml.loading.moddiscovery.ModDiscoverer/]: 
     Mod List:
		Name Version (Mod Id)

		LOD Server Support 0.23.0 (lss)
		LSS NeoForge GameTests 1.0.0 (lsstest)
		Minecraft 1.21.1 (minecraft)
		NeoForge 21.1.267 (neoforge)
[24Nov2026 23:15:58.203] [main/INFO] [mixin/]: Compatibility level set to JAVA_21
[24Nov2026 23:15:58.210] [main/INFO] [cpw.mods.modlauncher.LaunchServiceHandler/MODLAUNCHER]: Launching target 'forgeserverdev' with arguments [--gameDir, .]
[24Nov2026 23:15:59.249] [main/INFO] [MixinExtras|Service/]: Initializing MixinExtras via com.llamalad7.mixinextras.service.MixinExtrasServiceImpl(version=0.5.5).
[24Nov2026 23:16:03.821] [main/WARN] [net.minecraft.commands.Commands/]: Ambiguity between arguments [teleport, location] and [teleport, destination] with inputs: [0.1 -0.5 .9, 0 0 0]
[24Nov2026 23:16:03.823] [main/WARN] [net.minecraft.commands.Commands/]: Ambiguity between arguments [teleport, location] and [teleport, targets] with inputs: [0.1 -0.5 .9, 0 0 0]
[24Nov2026 23:16:03.826] [main/WARN] [net.minecraft.commands.Commands/]: Ambiguity between arguments [teleport, destination] and [teleport, targets] with inputs: [Player, 0123, @e, dd12be42-52a9-4a91-a8a1-11c01849e498]
[24Nov2026 23:16:03.828] [main/WARN] [net.minecraft.commands.Commands/]: Ambiguity between arguments [teleport, targets] and [teleport, destination] with inputs: [Player, 0123, dd12be42-52a9-4a91-a8a1-11c01849e498]
[24Nov2026 23:16:03.829] [main/WARN] [net.minecraft.commands.Commands/]: Ambiguity between arguments [teleport, targets, location] and [teleport, targets, destination] with inputs: [0.1 -0.5 .9, 0 0 0]
[24Nov2026 23:16:03.884] [modloading-worker-0/INFO] [net.neoforged.neoforge.common.NeoForgeMod/NEOFORGE-MOD]: NeoForge mod loading, version 21.1.267, for MC 1.21.1
[24Nov2026 23:16:04.212] [main/INFO] [com.mojang.authlib.yggdrasil.YggdrasilAuthenticationService/]: Environment: Environment[sessionHost=https://sessionserver.mojang.com, servicesHost=https://api.minecraftservices.com, name=PROD]
[24Nov2026 23:16:04.297] [main/WARN] [net.minecraft.server.packs.VanillaPackResourcesBuilder/]: Assets URL 'union:/home/wdzizon/lod-server-archive-read-hooks-review/neoforge/build/moddev/artifacts/neoforge-21.1.267.jar%23132!/assets/.mcassetsroot' uses unexpected schema
[24Nov2026 23:16:04.298] [main/WARN] [net.minecraft.server.packs.VanillaPackResourcesBuilder/]: Assets URL 'union:/home/wdzizon/lod-server-archive-read-hooks-review/neoforge/build/moddev/artifacts/neoforge-21.1.267.jar%23132!/data/.mcassetsroot' uses unexpected schema
[24Nov2026 23:16:04.304] [main/INFO] [net.neoforged.neoforge.gametest.GameTestHooks/]: Enabled Gametest Namespaces: [lsstest]
[24Nov2026 23:16:05.185] [main/INFO] [net.minecraft.world.item.crafting.RecipeManager/]: Loaded 1291 recipes
[24Nov2026 23:16:05.370] [main/INFO] [net.minecraft.advancements.AdvancementTree/]: Loaded 1400 advancements
[24Nov2026 23:16:06.254] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Preparing start region for dimension minecraft:overworld
[24Nov2026 23:16:06.307] [worldgen/INFO] [net.minecraft.server.level.progress.LoggerChunkProgressListener/]: Preparing spawn area: 2%
[24Nov2026 23:16:06.411] [Server thread/INFO] [net.minecraft.server.level.progress.LoggerChunkProgressListener/]: Time elapsed: 157 ms
[24Nov2026 23:16:06.424] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: Started game test server
[24Nov2026 23:16:06.454] [Server thread/INFO] [net.neoforged.neoforge.server.permission.PermissionAPI/]: Successfully initialized permission handler neoforge:default_handler
[24Nov2026 23:16:06.719] [Server thread/INFO] [LSS/]: LOD-only durable archive ready: LOD-only archive: state=ready schema=2 queue=0/4096 visit_history=positive-only absence=unknown invalidations_pending=0 egress_invalidation_blocked=false egress_visit_publication_blocked=false archive_untrusted=false session_visits=0 session_visit_overflow=false session_invalidations=0 session_invalidation_overflow=false tracking_started_ms=1795521277431
[24Nov2026 23:16:06.719] [Server thread/INFO] [LSS/]: Starting LSS LOD request processing service
[24Nov2026 23:16:06.939] [Server thread/INFO] [LSS/]: LOD store active (driver=private/3.49.1.0). It stores served LOD bytes under <world>/lss-lod/ and, once fully warmed, occupies roughly as much space as the region files themselves. It is DERIVED data — deleting lss-lod/ is always safe. Set storage.lod_store.enabled to false and restart to disable; storage.lod_store.max_size_mib bounds its size after reload.
[24Nov2026 23:16:06.945] [Server thread/INFO] [LSS/]: Effective config: useNbtTranscode=true, diskReaderThreads=3, useCompressedColumns=true, useBackgroundReadSplit=true, useSelectiveNbtParse=true, maxConcurrentDiskReads=2
[24Nov2026 23:16:06.946] [LSS LOD Store SQLite/INFO] [LSS/]: LOD store sweep [minecraft:overworld]: 4 changed region(s), dropped 24 stale + 0 vanished-region row(s)
[24Nov2026 23:16:06.952] [LSS Store Backfill/INFO] [LSS/]: Store backfill: 16 region(s) to process, estimated ~9 MB of new deposits (uncapped)
[24Nov2026 23:16:07.073] [Server thread/INFO] [LSS/]: Dirty content filter: seeded 49 already-loaded chunk(s)
[24Nov2026 23:16:07.137] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: 12 tests are now running at position 3975807, -59, -13052337!
[24Nov2026 23:16:07.572] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestRunner/]: Running test batch 'lodOnlyArchiveLifecycle:0' (1 tests)...
[24Nov2026 23:16:07.662] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [            ]
[24Nov2026 23:16:07.727] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [            ]
[24Nov2026 23:16:07.752] [Server thread/ERROR] [net.minecraft.gametest.framework.LogTestReporter/]: playerwatchrecorderpersistsvisitandsuppressesarchivedlod failed at 3975807, -60, -13052337! test LOD snapshot must be committed before the player watch
[24Nov2026 23:16:07.809] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestRunner/]: Running test batch 'defaultBatch:0' (11 tests)...
[24Nov2026 23:16:07.847] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [X           ]
[24Nov2026 23:16:07.997] [Server thread/INFO] [net.minecraft.server.players.PlayerList/]: test-mock-player[embedded] logged in with entity id 1 at (5.5, -60.0, 0.5)
[24Nov2026 23:16:08.140] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: test-mock-player joined the game
[24Nov2026 23:16:08.159] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v9999, capabilities=1)
[24Nov2026 23:16:08.161] [Server thread/WARN] [LSS/]: Player test-mock-player has incompatible LSS protocol version 9999 (server: 20), skipping LOD distribution
[24Nov2026 23:16:08.207] [Server thread/WARN] [LSS/]: Auxiliary snapshot eligibility inspection failed; normal LOD delivery continues without archiving
java.lang.IllegalStateException: synthetic metadata observer failure
	at TRANSFORMER/lsstest@1.0.0/dev.vox.lss.neoforge.gametest.LSSNeoGameTests.lambda$generationObserverFailurePreservesNormalResult$7(LSSNeoGameTests.java:308) ~[%23134!/:?]
	at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.ChunkGenerationService.tick(ChunkGenerationService.java:245) ~[%23135!/:?]
	at TRANSFORMER/lsstest@1.0.0/dev.vox.lss.neoforge.gametest.LSSNeoGameTests.generationObserverFailurePreservesNormalResult(LSSNeoGameTests.java:316) ~[%23134!/:?]
	at java.base/jdk.internal.reflect.DirectMethodHandleAccessor.invoke(DirectMethodHandleAccessor.java:103) ~[?:?]
	at java.base/java.lang.reflect.Method.invoke(Method.java:580) ~[?:?]
	at TRANSFORMER/minecraft@1.21.1/net.minecraft.gametest.framework.GameTestRegistry.lambda$turnMethodIntoConsumer$5(GameTestRegistry.java:157) ~[neoforge-21.1.267.jar%23132!/:?]
	at TRANSFORMER/minecraft@1.21.1/net.minecraft.gametest.framework.TestFunction.run(TestFunction.java:40) ~[neoforge-21.1.267.jar%23132!/:?]
	at TRANSFORMER/minecraft@1.21.1/net.minecraft.gametest.framework.GameTestInfo.startTest(GameTestInfo.java:162) ~[neoforge-21.1.267.jar%23132!/:?]
	at TRANSFORMER/minecraft@1.21.1/net.minecraft.gametest.framework.GameTestInfo.tickInternal(GameTestInfo.java:124) ~[neoforge-21.1.267.jar%23132!/:?]
	at TRANSFORMER/minecraft@1.21.1/net.minecraft.gametest.framework.GameTestInfo.tick(GameTestInfo.java:107) ~[neoforge-21.1.267.jar%23132!/:?]
	at TRANSFORMER/minecraft@1.21.1/net.minecraft.gametest.framework.GameTestTicker.lambda$tick$0(GameTestTicker.java:39) ~[neoforge-21.1.267.jar%23132!/:?]
	at java.base/java.util.concurrent.CopyOnWriteArrayList.forEach(CopyOnWriteArrayList.java:891) ~[?:?]
	at TRANSFORMER/minecraft@1.21.1/net.minecraft.gametest.framework.GameTestTicker.tick(GameTestTicker.java:39) ~[neoforge-21.1.267.jar%23132!/:?]
	at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.MinecraftServer.tickChildren(MinecraftServer.java:1055) ~[neoforge-21.1.267.jar%23132!/:?]
	at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.MinecraftServer.tickServer(MinecraftServer.java:917) ~[neoforge-21.1.267.jar%23132!/:?]
	at TRANSFORMER/minecraft@1.21.1/net.minecraft.gametest.framework.GameTestServer.tickServer(GameTestServer.java:168) ~[neoforge-21.1.267.jar%23132!/:?]
	at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.MinecraftServer.runServer(MinecraftServer.java:707) ~[neoforge-21.1.267.jar%23132!/:?]
	at TRANSFORMER/minecraft@1.21.1/net.minecraft.server.MinecraftServer.lambda$spin$2(MinecraftServer.java:267) ~[neoforge-21.1.267.jar%23132!/:?]
	at java.base/java.lang.Thread.run(Thread.java:1583) [?:?]
[24Nov2026 23:16:08.219] [Server thread/INFO] [net.minecraft.server.players.PlayerList/]: test-mock-player[embedded] logged in with entity id 2 at (5.5, -60.0, -3.5)
[24Nov2026 23:16:08.221] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: test-mock-player joined the game
[24Nov2026 23:16:08.226] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v20, capabilities=0)
[24Nov2026 23:16:08.228] [Server thread/INFO] [LSS/]: Player test-mock-player has no LOD consumer (caps=0), skipping LOD registration
[24Nov2026 23:16:08.245] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [X+++++      ]
[24Nov2026 23:16:08.465] [Server thread/INFO] [net.minecraft.server.players.PlayerList/]: test-mock-player[embedded] logged in with entity id 3 at (5.5, -60.0, 10.5)
[24Nov2026 23:16:08.467] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: test-mock-player joined the game
[24Nov2026 23:16:08.470] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v20, capabilities=1)
[24Nov2026 23:16:08.476] [Server thread/INFO] [LSS/]: Player test-mock-player registered for LSS LOD request processing (caps=1)
[24Nov2026 23:16:11.488] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [X+++++++++_+]
[24Nov2026 23:16:11.510] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [X+++++++++++]
[24Nov2026 23:16:11.513] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: ========= 12 GAME TESTS COMPLETE IN 4.374 s ======================
[24Nov2026 23:16:11.514] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: 1 required tests failed :(
[24Nov2026 23:16:11.514] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]:    - playerwatchrecorderpersistsvisitandsuppressesarchivedlod
[24Nov2026 23:16:11.515] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: ====================================================
[24Nov2026 23:16:11.520] [Server thread/INFO] [LSS/]: Preparing LSS LOD generation tickets for final world save
[24Nov2026 23:16:11.522] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping server
[24Nov2026 23:16:11.523] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving players
[24Nov2026 23:16:11.568] [Server thread/INFO] [net.minecraft.server.network.ServerGamePacketListenerImpl/]: test-mock-player lost connection: Server closed
[24Nov2026 23:16:11.568] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: test-mock-player left the game
[24Nov2026 23:16:11.581] [Server thread/INFO] [net.minecraft.server.network.ServerGamePacketListenerImpl/]: test-mock-player lost connection: Server closed
[24Nov2026 23:16:11.581] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: test-mock-player left the game
[24Nov2026 23:16:11.590] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving worlds
[24Nov2026 23:16:11.948] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:overworld
[24Nov2026 23:16:15.836] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:the_end
[24Nov2026 23:16:15.842] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:the_nether
[24Nov2026 23:16:15.861] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (world): All chunks are saved
[24Nov2026 23:16:15.862] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM1): All chunks are saved
[24Nov2026 23:16:15.862] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM-1): All chunks are saved
[24Nov2026 23:16:15.862] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage: All dimensions are saved
[24Nov2026 23:16:15.904] [Server thread/INFO] [LSS/]: Stopping LSS LOD request processing service
[24Nov2026 23:16:15.907] [LSS Store Backfill/INFO] [LSS/]: Store backfill stopped (shutdown): 4 regions, 1 deposited, 640 skipped, 0 errors
[24Nov2026 23:16:15.920] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: Game test server shutting down
