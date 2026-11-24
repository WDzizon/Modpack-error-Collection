[25Nov2026 02:50:17.214] [main/INFO] [cpw.mods.modlauncher.Launcher/MODLAUNCHER]: ModLauncher running: args [--launchTarget, forgeserverdev, --gameDir, ., --fml.fmlVersion, 4.0.45, --fml.mcVersion, 1.21.1, --fml.neoForgeVersion, 21.1.267, --fml.neoFormVersion, 20240808.144430]
[25Nov2026 02:50:17.219] [main/INFO] [cpw.mods.modlauncher.Launcher/MODLAUNCHER]: JVM identified as Ubuntu OpenJDK 64-Bit Server VM 21.0.13.1+2-1-24.04.1-Ubuntu
[25Nov2026 02:50:17.221] [main/INFO] [cpw.mods.modlauncher.Launcher/MODLAUNCHER]: ModLauncher 11.0.5+main.901c6ea8 starting: java version 21.0.13.1 by Ubuntu; OS Linux arch amd64 version 6.18.40.1-microsoft-standard-WSL2
[25Nov2026 02:50:17.350] [main/INFO] [net.neoforged.fml.loading.ImmediateWindowHandler/]: ImmediateWindowProvider not loading because launch target is forgeserverdev
[25Nov2026 02:50:17.410] [main/INFO] [mixin/]: SpongePowered MIXIN Subsystem Version=0.8.7 Source=union:/home/wdzizon/.gradle/caches/modules-2/files-2.1/net.fabricmc/sponge-mixin/0.16.4+mixin.0.8.7/26d01f0567ab46e9ca0d2ed89d0ecc11aadbd433/sponge-mixin-0.16.4+mixin.0.8.7.jar%2398!/ Service=ModLauncher Env=SERVER
[25Nov2026 02:50:17.924] [main/INFO] [net.neoforged.fml.loading.moddiscovery.locators.JarInJarDependencyLocator/]: Found 2 dependencies adding them to mods collection
[25Nov2026 02:50:17.926] [main/INFO] [net.neoforged.fml.loading.moddiscovery.ModDiscoverer/]: 
     Mod List:
		Name Version (Mod Id)

		LOD Server Support 0.23.0 (lss)
		LSS NeoForge GameTests 1.0.0 (lsstest)
		Minecraft 1.21.1 (minecraft)
		NeoForge 21.1.267 (neoforge)
[25Nov2026 02:50:18.745] [main/INFO] [mixin/]: Compatibility level set to JAVA_21
[25Nov2026 02:50:18.754] [main/INFO] [cpw.mods.modlauncher.LaunchServiceHandler/MODLAUNCHER]: Launching target 'forgeserverdev' with arguments [--gameDir, .]
[25Nov2026 02:50:20.249] [main/INFO] [MixinExtras|Service/]: Initializing MixinExtras via com.llamalad7.mixinextras.service.MixinExtrasServiceImpl(version=0.5.5).
[25Nov2026 02:50:27.268] [main/WARN] [net.minecraft.commands.Commands/]: Ambiguity between arguments [teleport, location] and [teleport, destination] with inputs: [0.1 -0.5 .9, 0 0 0]
[25Nov2026 02:50:27.271] [main/WARN] [net.minecraft.commands.Commands/]: Ambiguity between arguments [teleport, location] and [teleport, targets] with inputs: [0.1 -0.5 .9, 0 0 0]
[25Nov2026 02:50:27.276] [main/WARN] [net.minecraft.commands.Commands/]: Ambiguity between arguments [teleport, destination] and [teleport, targets] with inputs: [Player, 0123, @e, dd12be42-52a9-4a91-a8a1-11c01849e498]
[25Nov2026 02:50:27.278] [main/WARN] [net.minecraft.commands.Commands/]: Ambiguity between arguments [teleport, targets] and [teleport, destination] with inputs: [Player, 0123, dd12be42-52a9-4a91-a8a1-11c01849e498]
[25Nov2026 02:50:27.281] [main/WARN] [net.minecraft.commands.Commands/]: Ambiguity between arguments [teleport, targets, location] and [teleport, targets, destination] with inputs: [0.1 -0.5 .9, 0 0 0]
[25Nov2026 02:50:27.372] [modloading-worker-0/INFO] [net.neoforged.neoforge.common.NeoForgeMod/NEOFORGE-MOD]: NeoForge mod loading, version 21.1.267, for MC 1.21.1
[25Nov2026 02:50:27.687] [modloading-sync-worker/WARN] [net.neoforged.fml.config.ConfigTracker/CONFIG]: Configuration file /home/wdzizon/lod-server-support-lod-only/neoforge/run/config/neoforge-common.toml is not correct. Correcting
[25Nov2026 02:50:27.835] [main/INFO] [com.mojang.authlib.yggdrasil.YggdrasilAuthenticationService/]: Environment: Environment[sessionHost=https://sessionserver.mojang.com, servicesHost=https://api.minecraftservices.com, name=PROD]
[25Nov2026 02:50:27.952] [main/WARN] [net.neoforged.neoforge.common.CommonHooks/WP]: The following mods have version differences that were not resolved:
neoforge (version 21.1.248 -> 21.1.267)
Things may not work well.
[25Nov2026 02:50:27.971] [main/WARN] [net.minecraft.server.packs.VanillaPackResourcesBuilder/]: Assets URL 'union:/home/wdzizon/lod-server-support-lod-only/neoforge/build/moddev/artifacts/neoforge-21.1.267.jar%23132!/assets/.mcassetsroot' uses unexpected schema
[25Nov2026 02:50:27.972] [main/WARN] [net.minecraft.server.packs.VanillaPackResourcesBuilder/]: Assets URL 'union:/home/wdzizon/lod-server-support-lod-only/neoforge/build/moddev/artifacts/neoforge-21.1.267.jar%23132!/data/.mcassetsroot' uses unexpected schema
[25Nov2026 02:50:27.982] [main/INFO] [net.neoforged.neoforge.gametest.GameTestHooks/]: Enabled Gametest Namespaces: [lsstest]
[25Nov2026 02:50:29.312] [main/INFO] [net.minecraft.world.item.crafting.RecipeManager/]: Loaded 1291 recipes
[25Nov2026 02:50:29.574] [main/INFO] [net.minecraft.advancements.AdvancementTree/]: Loaded 1400 advancements
[25Nov2026 02:50:30.722] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Preparing start region for dimension minecraft:overworld
[25Nov2026 02:50:30.804] [worldgen/INFO] [net.minecraft.server.level.progress.LoggerChunkProgressListener/]: Preparing spawn area: 2%
[25Nov2026 02:50:30.948] [Server thread/INFO] [net.minecraft.server.level.progress.LoggerChunkProgressListener/]: Time elapsed: 224 ms
[25Nov2026 02:50:30.966] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: Started game test server
[25Nov2026 02:50:30.989] [Server thread/INFO] [net.neoforged.neoforge.server.permission.PermissionAPI/]: Successfully initialized permission handler neoforge:default_handler
[25Nov2026 02:50:31.352] [Server thread/INFO] [LSS/]: LOD-only durable archive ready: LOD-only archive: state=ready schema=2 queue=0/4096 visit_history=positive-only absence=unknown invalidations_pending=0 egress_invalidation_blocked=false egress_visit_publication_blocked=false archive_untrusted=false session_visits=0 session_visit_overflow=false session_invalidations=0 session_invalidation_overflow=false tracking_started_ms=1795496799715
[25Nov2026 02:50:31.353] [Server thread/INFO] [LSS/]: Starting LSS LOD request processing service
[25Nov2026 02:50:31.580] [Server thread/INFO] [LSS/]: LOD store active (driver=private/3.49.1.0). It stores served LOD bytes under <world>/lss-lod/ and, once fully warmed, occupies roughly as much space as the region files themselves. It is DERIVED data — deleting lss-lod/ is always safe. Set storage.lod_store.enabled to false and restart to disable; storage.lod_store.max_size_mib bounds its size after reload.
[25Nov2026 02:50:31.587] [Server thread/INFO] [LSS/]: Effective config: useNbtTranscode=true, diskReaderThreads=3, useCompressedColumns=true, useBackgroundReadSplit=true, useSelectiveNbtParse=true, maxConcurrentDiskReads=2
[25Nov2026 02:50:31.590] [LSS LOD Store SQLite/INFO] [LSS/]: LOD store sweep [minecraft:overworld]: 2 changed region(s), dropped 0 stale + 0 vanished-region row(s)
[25Nov2026 02:50:31.601] [LSS Store Backfill/INFO] [LSS/]: Store backfill: 30 region(s) to process, estimated ~17 MB of new deposits (uncapped)
[25Nov2026 02:50:31.797] [Server thread/INFO] [LSS/]: Dirty content filter: seeded 49 already-loaded chunk(s)
[25Nov2026 02:50:31.886] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: 12 tests are now running at position -3844522, -59, 14408324!
[25Nov2026 02:50:32.425] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestRunner/]: Running test batch 'lodOnlyArchiveLifecycle:0' (1 tests)...
[25Nov2026 02:50:32.611] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [            ]
[25Nov2026 02:50:32.650] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [            ]
[25Nov2026 02:50:32.722] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [            ]
[25Nov2026 02:50:32.936] [Server thread/INFO] [net.minecraft.server.players.PlayerList/]: test-mock-player[embedded] logged in with entity id 1 at (9.5, -60.0, -1.5)
[25Nov2026 02:50:33.206] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: test-mock-player joined the game
[25Nov2026 02:50:33.248] [Server thread/INFO] [net.minecraft.server.players.PlayerList/]: test-mock-player[embedded] logged in with entity id 2 at (-9.5, -60.0, -0.5)
[25Nov2026 02:50:33.254] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: test-mock-player joined the game
[25Nov2026 02:50:33.363] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestRunner/]: Running test batch 'defaultBatch:0' (11 tests)...
[25Nov2026 02:50:33.499] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [+           ]
[25Nov2026 02:50:33.579] [Server thread/INFO] [net.minecraft.server.players.PlayerList/]: test-mock-player[embedded] logged in with entity id 3 at (-0.5, -60.0, -4.5)
[25Nov2026 02:50:33.583] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: test-mock-player joined the game
[25Nov2026 02:50:33.594] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v9999, capabilities=1)
[25Nov2026 02:50:33.599] [Server thread/WARN] [LSS/]: Player test-mock-player has incompatible LSS protocol version 9999 (server: 20), skipping LOD distribution
[25Nov2026 02:50:33.647] [Server thread/WARN] [LSS/]: Auxiliary snapshot eligibility inspection failed; normal LOD delivery continues without archiving
java.lang.IllegalStateException: synthetic metadata observer failure
	at TRANSFORMER/lsstest@1.0.0/dev.vox.lss.neoforge.gametest.LSSNeoGameTests.lambda$generationObserverFailurePreservesNormalResult$7(LSSNeoGameTests.java:338) ~[%23134!/:?]
	at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.ChunkGenerationService.tick(ChunkGenerationService.java:245) ~[%23135!/:?]
	at TRANSFORMER/lsstest@1.0.0/dev.vox.lss.neoforge.gametest.LSSNeoGameTests.generationObserverFailurePreservesNormalResult(LSSNeoGameTests.java:346) ~[%23134!/:?]
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
[25Nov2026 02:50:33.679] [Server thread/INFO] [net.minecraft.server.players.PlayerList/]: test-mock-player[embedded] logged in with entity id 4 at (9.5, -60.0, 4.5)
[25Nov2026 02:50:33.683] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: test-mock-player joined the game
[25Nov2026 02:50:33.687] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v20, capabilities=0)
[25Nov2026 02:50:33.690] [Server thread/INFO] [LSS/]: Player test-mock-player has no LOD consumer (caps=0), skipping LOD registration
[25Nov2026 02:50:33.929] [Server thread/INFO] [net.minecraft.server.players.PlayerList/]: test-mock-player[embedded] logged in with entity id 5 at (-3.5, -60.0, -5.5)
[25Nov2026 02:50:33.933] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: test-mock-player joined the game
[25Nov2026 02:50:33.938] [Server thread/INFO] [LSS/]: LSS handshake received from test-mock-player (protocol v20, capabilities=1)
[25Nov2026 02:50:33.946] [Server thread/INFO] [LSS/]: Player test-mock-player registered for LSS LOD request processing (caps=1)
[25Nov2026 02:50:34.026] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [++++++++++_+]
[25Nov2026 02:50:36.388] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: [++++++++++++]
[25Nov2026 02:50:36.391] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: ========= 12 GAME TESTS COMPLETE IN 5.527 s ======================
[25Nov2026 02:50:36.392] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: All 12 required tests passed :)
[25Nov2026 02:50:36.393] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: ====================================================
[25Nov2026 02:50:36.413] [Server thread/INFO] [LSS/]: Preparing LSS LOD generation tickets for final world save
[25Nov2026 02:50:36.416] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping server
[25Nov2026 02:50:36.416] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving players
[25Nov2026 02:50:36.489] [Server thread/INFO] [net.minecraft.server.network.ServerGamePacketListenerImpl/]: test-mock-player lost connection: Server closed
[25Nov2026 02:50:36.490] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: test-mock-player left the game
[25Nov2026 02:50:36.510] [Server thread/INFO] [net.minecraft.server.network.ServerGamePacketListenerImpl/]: test-mock-player lost connection: Server closed
[25Nov2026 02:50:36.510] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: test-mock-player left the game
[25Nov2026 02:50:36.522] [Server thread/INFO] [net.minecraft.server.network.ServerGamePacketListenerImpl/]: test-mock-player lost connection: Server closed
[25Nov2026 02:50:36.522] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: test-mock-player left the game
[25Nov2026 02:50:36.533] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving worlds
[25Nov2026 02:50:36.983] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:overworld
[25Nov2026 02:50:40.944] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:the_end
[25Nov2026 02:50:40.951] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[Test Level]'/minecraft:the_nether
[25Nov2026 02:50:40.986] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (world): All chunks are saved
[25Nov2026 02:50:40.986] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM1): All chunks are saved
[25Nov2026 02:50:40.986] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM-1): All chunks are saved
[25Nov2026 02:50:40.986] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage: All dimensions are saved
[25Nov2026 02:50:41.037] [Server thread/INFO] [LSS/]: Stopping LSS LOD request processing service
[25Nov2026 02:50:41.039] [LSS Store Backfill/INFO] [LSS/]: Store backfill stopped (shutdown): 1 regions, 40 deposited, 722 skipped, 0 errors
[25Nov2026 02:50:41.058] [Server thread/INFO] [net.minecraft.gametest.framework.GameTestServer/]: Game test server shutting down
