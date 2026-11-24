[24Nov2026 14:20:29.626] [main/INFO] [cpw.mods.modlauncher.Launcher/MODLAUNCHER]: ModLauncher running: args [--launchTarget, forgeserverdev, --gameDir, ., --fml.fmlVersion, 4.0.43, --fml.mcVersion, 1.21.1, --fml.neoForgeVersion, 21.1.248, --fml.neoFormVersion, 20240808.144430]
[24Nov2026 14:20:29.628] [main/INFO] [cpw.mods.modlauncher.Launcher/MODLAUNCHER]: JVM identified as Ubuntu OpenJDK 64-Bit Server VM 21.0.13.1+2-1-24.04.1-Ubuntu
[24Nov2026 14:20:29.631] [main/INFO] [cpw.mods.modlauncher.Launcher/MODLAUNCHER]: ModLauncher 11.0.5+main.901c6ea8 starting: java version 21.0.13.1 by Ubuntu; OS Linux arch amd64 version 6.18.40.1-microsoft-standard-WSL2
[24Nov2026 14:20:29.787] [main/INFO] [net.neoforged.fml.loading.ImmediateWindowHandler/]: ImmediateWindowProvider not loading because launch target is forgeserverdev
[24Nov2026 14:20:29.846] [main/INFO] [mixin/]: SpongePowered MIXIN Subsystem Version=0.8.7 Source=union:/home/wdzizon/.gradle/caches/modules-2/files-2.1/net.fabricmc/sponge-mixin/0.15.2+mixin.0.8.7/2af2f021d8e02a0220dc27a7a72b4666d66d44ca/sponge-mixin-0.15.2+mixin.0.8.7.jar%2398!/ Service=ModLauncher Env=SERVER
[24Nov2026 14:20:30.163] [main/INFO] [net.neoforged.fml.loading.moddiscovery.locators.JarInJarDependencyLocator/]: Found 2 dependencies adding them to mods collection
[24Nov2026 14:20:30.165] [main/INFO] [net.neoforged.fml.loading.moddiscovery.ModDiscoverer/]: 
     Mod List:
		Name Version (Mod Id)

		LOD Server Support 0.23.0 (lss)
		LSS NeoForge GameTests 1.0.0 (lsstest)
		Minecraft 1.21.1 (minecraft)
		NeoForge 21.1.248 (neoforge)
[24Nov2026 14:20:30.862] [main/INFO] [mixin/]: Compatibility level set to JAVA_21
[24Nov2026 14:20:30.868] [main/INFO] [cpw.mods.modlauncher.LaunchServiceHandler/MODLAUNCHER]: Launching target 'forgeserverdev' with arguments [--gameDir, .]
[24Nov2026 14:20:31.824] [main/INFO] [MixinExtras|Service/]: Initializing MixinExtras via com.llamalad7.mixinextras.service.MixinExtrasServiceImpl(version=0.5.3).
[24Nov2026 14:20:37.376] [main/WARN] [net.minecraft.commands.Commands/]: Ambiguity between arguments [teleport, location] and [teleport, destination] with inputs: [0.1 -0.5 .9, 0 0 0]
[24Nov2026 14:20:37.379] [main/WARN] [net.minecraft.commands.Commands/]: Ambiguity between arguments [teleport, location] and [teleport, targets] with inputs: [0.1 -0.5 .9, 0 0 0]
[24Nov2026 14:20:37.383] [main/WARN] [net.minecraft.commands.Commands/]: Ambiguity between arguments [teleport, destination] and [teleport, targets] with inputs: [Player, 0123, @e, dd12be42-52a9-4a91-a8a1-11c01849e498]
[24Nov2026 14:20:37.384] [main/WARN] [net.minecraft.commands.Commands/]: Ambiguity between arguments [teleport, targets] and [teleport, destination] with inputs: [Player, 0123, dd12be42-52a9-4a91-a8a1-11c01849e498]
[24Nov2026 14:20:37.385] [main/WARN] [net.minecraft.commands.Commands/]: Ambiguity between arguments [teleport, targets, location] and [teleport, targets, destination] with inputs: [0.1 -0.5 .9, 0 0 0]
[24Nov2026 14:20:37.448] [modloading-worker-0/INFO] [net.neoforged.neoforge.common.NeoForgeMod/NEOFORGE-MOD]: NeoForge mod loading, version 21.1.248, for MC 1.21.1
[24Nov2026 14:20:37.823] [main/INFO] [com.mojang.authlib.yggdrasil.YggdrasilAuthenticationService/]: Environment: Environment[sessionHost=https://sessionserver.mojang.com, servicesHost=https://api.minecraftservices.com, name=PROD]
[24Nov2026 14:20:37.911] [main/WARN] [net.minecraft.server.packs.VanillaPackResourcesBuilder/]: Assets URL 'union:/home/wdzizon/lod-server-support-lod-only/neoforge/build/moddev/artifacts/neoforge-21.1.248.jar%23132!/assets/.mcassetsroot' uses unexpected schema
[24Nov2026 14:20:37.912] [main/WARN] [net.minecraft.server.packs.VanillaPackResourcesBuilder/]: Assets URL 'union:/home/wdzizon/lod-server-support-lod-only/neoforge/build/moddev/artifacts/neoforge-21.1.248.jar%23132!/data/.mcassetsroot' uses unexpected schema
[24Nov2026 14:20:37.920] [main/INFO] [net.neoforged.neoforge.gametest.GameTestHooks/]: Enabled Gametest Namespaces: [lsstest]
[24Nov2026 14:20:38.958] [main/INFO] [net.minecraft.world.item.crafting.RecipeManager/]: Loaded 1291 recipes
[24Nov2026 14:20:39.147] [main/INFO] [net.minecraft.advancements.AdvancementTree/]: Loaded 1400 advancements
[24Nov2026 14:20:40.122] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Preparing start region for dimension minecraft:overworld
[24Nov2026 14:20:40.194] [worldgen/INFO] [net.minecraft.server.level.progress.LoggerChunkProgressListener/]: Preparing spawn area: 2%
[24Nov2026 14:20:40.292] [Server thread/INFO] [net.minecraft.server.level.progress.LoggerChunkProgressListener/]: Time elapsed: 170 ms
[24Nov2026 14:20:40.305] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: Started game test server
[24Nov2026 14:20:40.327] [Server thread/INFO] [net.neoforged.neoforge.server.permission.PermissionAPI/]: Successfully initialized permission handler neoforge:default_handler
[24Nov2026 14:20:40.699] [Server thread/INFO] [LSS/]: LOD-only durable archive ready: LOD-only archive: state=ready schema=2 queue=0/4096 visit_history=positive-only absence=unknown invalidations_pending=0 egress_invalidation_blocked=false egress_visit_publication_blocked=false archive_untrusted=false session_visits=0 session_visit_overflow=false session_invalidations=0 session_invalidation_overflow=false tracking_started_ms=1795496799715
[24Nov2026 14:20:40.700] [Server thread/INFO] [LSS/]: Starting LSS LOD request processing service
[24Nov2026 14:20:40.925] [Server thread/INFO] [LSS/]: LOD store active (driver=private/3.49.1.0). It stores served LOD bytes under <world>/lss-lod/ and, once fully warmed, occupies roughly as much space as the region files themselves. It is DERIVED data — deleting lss-lod/ is always safe. Set storage.lod_store.enabled to false and restart to disable; storage.lod_store.max_size_mib bounds its size after reload.
[24Nov2026 14:20:40.931] [Server thread/INFO] [LSS/]: Effective config: useNbtTranscode=true, diskReaderThreads=3, useCompressedColumns=true, useBackgroundReadSplit=true, useSelectiveNbtParse=true, maxConcurrentDiskReads=2
[24Nov2026 14:20:40.934] [LSS LOD Store SQLite/INFO] [LSS/]: LOD store sweep [minecraft:overworld]: 4 changed region(s), dropped 66 stale + 0 vanished-region row(s)
[24Nov2026 14:20:40.940] [LSS Store Backfill/INFO] [LSS/]: Store backfill: 15 region(s) to process, estimated ~8 MB of new deposits (uncapped)
[24Nov2026 14:20:41.075] [Server thread/INFO] [LSS/]: Dirty content filter: seeded 49 already-loaded chunk(s)
[24Nov2026 14:20:41.160] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: 12 tests are now running at position -3971915, -59, -6181840!
[24Nov2026 14:20:41.650] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestRunner/]: Running test batch 'lodOnlyArchiveLifecycle:0' (1 tests)...
[24Nov2026 14:20:41.790] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [            ]
[24Nov2026 14:20:41.817] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [            ]
[24Nov2026 14:20:41.835] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [            ]
[24Nov2026 14:20:41.857] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [            ]
[24Nov2026 14:20:41.879] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [            ]
[24Nov2026 14:20:41.899] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [            ]
[24Nov2026 14:20:41.920] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [            ]
[24Nov2026 14:20:41.937] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [            ]
[24Nov2026 14:20:41.950] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [            ]
[24Nov2026 14:20:41.962] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [            ]
[24Nov2026 14:20:41.976] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [            ]
[24Nov2026 14:20:41.990] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [            ]
[24Nov2026 14:20:42.004] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [            ]
[24Nov2026 14:20:42.017] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [            ]
[24Nov2026 14:20:42.028] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [            ]
[24Nov2026 14:20:42.362] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [            ]
[24Nov2026 14:20:42.442] [Server thread/ERROR] [net.minecraft.gametest.framework.LogTestReporter/]: playerwatchrecorderpersistsvisitandsuppressesarchivedlod failed at -3971915, -60, -6181840! the test archive row must be visible before the watch signal
[24Nov2026 14:20:42.494] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestRunner/]: Running test batch 'defaultBatch:0' (11 tests)...
[24Nov2026 14:20:42.505] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [X           ]
[24Nov2026 14:20:42.778] [Server thread/INFO] [net.minecraft.server.players.PlayerList/]: test-mock-player[embedded] logged in with entity id 1 at (3.5, -60.0, -8.5)
[24Nov2026 14:20:42.967] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: test-mock-player joined the game
[24Nov2026 14:20:42.987] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v9999, capabilities=1)
[24Nov2026 14:20:42.989] [Server thread/WARN] [LSS/]: Player test-mock-player has incompatible LSS protocol version 9999 (server: 20), skipping LOD distribution
[24Nov2026 14:20:43.053] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [X+      ++  ]
[24Nov2026 14:20:43.065] [Server thread/WARN] [LSS/]: Auxiliary snapshot eligibility inspection failed; normal LOD delivery continues without archiving
java.lang.IllegalStateException: synthetic metadata observer failure
	at TRANSFORMER/lsstest@1.0.0/dev.vox.lss.neoforge.gametest.LSSNeoGameTests.lambda$generationObserverFailurePreservesNormalResult$7(LSSNeoGameTests.java:302) ~[%23134!/:?]
	at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.ChunkGenerationService.tick(ChunkGenerationService.java:245) ~[%23135!/:?]
	at TRANSFORMER/lsstest@1.0.0/dev.vox.lss.neoforge.gametest.LSSNeoGameTests.generationObserverFailurePreservesNormalResult(LSSNeoGameTests.java:310) ~[%23134!/:?]
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
[24Nov2026 14:20:43.079] [Server thread/INFO] [net.minecraft.server.players.PlayerList/]: test-mock-player[embedded] logged in with entity id 2 at (-3.5, -60.0, -2.5)
[24Nov2026 14:20:43.082] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: test-mock-player joined the game
[24Nov2026 14:20:43.088] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v20, capabilities=0)
[24Nov2026 14:20:43.090] [Server thread/INFO] [LSS/]: Player test-mock-player has no LOD consumer (caps=0), skipping LOD registration
[24Nov2026 14:20:43.322] [Server thread/INFO] [net.minecraft.server.players.PlayerList/]: test-mock-player[embedded] logged in with entity id 3 at (-6.5, -60.0, -8.5)
[24Nov2026 14:20:43.326] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: test-mock-player joined the game
[24Nov2026 14:20:43.329] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v20, capabilities=1)
[24Nov2026 14:20:43.337] [Server thread/INFO] [LSS/]: Player test-mock-player registered for LSS LOD request processing (caps=1)
[24Nov2026 14:20:46.658] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [X+++++++++++]
[24Nov2026 14:20:46.660] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: ========= 12 GAME TESTS COMPLETE IN 5.498 s ======================
[24Nov2026 14:20:46.661] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: 1 required tests failed :(
[24Nov2026 14:20:46.661] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]:    - playerwatchrecorderpersistsvisitandsuppressesarchivedlod
[24Nov2026 14:20:46.662] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: ====================================================
[24Nov2026 14:20:46.675] [Server thread/INFO] [LSS/]: Preparing LSS LOD generation tickets for final world save
[24Nov2026 14:20:46.677] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping server
[24Nov2026 14:20:46.677] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving players
[24Nov2026 14:20:46.721] [Server thread/INFO] [net.minecraft.server.network.ServerGamePacketListenerImpl/]: test-mock-player lost connection: Server closed
[24Nov2026 14:20:46.721] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: test-mock-player left the game
[24Nov2026 14:20:46.734] [Server thread/INFO] [net.minecraft.server.network.ServerGamePacketListenerImpl/]: test-mock-player lost connection: Server closed
[24Nov2026 14:20:46.735] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: test-mock-player left the game
[24Nov2026 14:20:46.744] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving worlds
[24Nov2026 14:20:47.091] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:overworld
[24Nov2026 14:20:51.193] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:the_nether
[24Nov2026 14:20:51.203] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:the_end
[24Nov2026 14:20:51.227] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (world): All chunks are saved
[24Nov2026 14:20:51.228] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM-1): All chunks are saved
[24Nov2026 14:20:51.228] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM1): All chunks are saved
[24Nov2026 14:20:51.228] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage: All dimensions are saved
[24Nov2026 14:20:51.271] [Server thread/INFO] [LSS/]: Stopping LSS LOD request processing service
[24Nov2026 14:20:51.273] [LSS Store Backfill/INFO] [LSS/]: Store backfill stopped (shutdown): 3 regions, 51 deposited, 928 skipped, 0 errors
[24Nov2026 14:20:51.291] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: Game test server shutting down
