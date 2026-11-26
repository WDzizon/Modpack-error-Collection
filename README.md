========== latest.log ==========

  [2611??026 13:52:05.436] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: LOD-only preservation: inspected=757 candidates_at_generation=0 snapshot_candidates_at_generation=0 protected_area=0 player_watched_before_generation=5 uncertain_player_acces
s=539 structure_starts=9 structure_references=204 uncertain=0 watch_index=count=1554,supported=true,overflow=false,archive=unavailable,visit_write_failed=true,history=positive-only,scope=session-only structure_inspection_failed=false deletion=DISABLED | LOD-only
archive: state=unavailable attached=false durable_visit_write_failed=true | LOD-only recovery inspection: mode=filesystem-only auto_recovery=disabled directory=directory session_marker=regular(63B) invalidation_marker=missing archive_db=regular(182325248B) wal=re
gular(4165352B) shm=regular(32768B) journal=missing lock_file=regular(0B) operator_review=required | LOD-only snapshot writes: attempts=0 committed=0 protected_noop=0 failures=0
  [2611??026 13:52:05.845] [LSS Processing Thread/WARN] [LSS/]: Disk reads are concurrency-gated under sustained load (read_gate=2/2, park full): the request router is deferring cold-region reads to the next client declaration (running total: gate_stops= in /lssl
od diag). This is the gate working; raise storage.disk.max_concurrent_reads in lss-server-config.yaml and reload if server CPU headroom allows and you want faster cold backfill. (Logged once per session.)
  [2611??026 13:54:20.160] [LSS Disk Reader #1/WARN] [LSS/]: Disk read timed out (>10s) at 535, -109 ??triaged as not-found (counted disk.errors; self-heals by re-declaration on gen-enabled servers)
> [2611??026 13:54:30.591] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping the server
> [2611??026 13:54:30.592] [Server thread/INFO] [LSS/]: Preparing LSS LOD generation tickets for final world save
  [2611??026 13:54:30.594] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping server
  [2611??026 13:54:30.595] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving players
  [2611??026 13:54:30.930] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving worlds
  [2611??026 13:54:31.845] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:overworld
  [2611??026 13:54:50.270] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:the_end
  [2611??026 13:54:50.303] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:the_nether
  [2611??026 13:54:50.365] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM1): All chunks are saved
  [2611??026 13:54:50.365] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM-1): All chunks are saved
  [2611??026 13:54:50.366] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage: All dimensions are saved
> [2611??026 13:54:52.698] [Server thread/INFO] [LSS/]: Stopping LSS LOD request processing service

========== debug-3.log.gz ==========
  [2611월2026 13:44:37.663] [LSS Processing Thread/DEBUG] [LSS/]: Disk saturated/gated result dropped silently (superseded) for ea04c93a-d122-4b7b-baee-1c53d5ae535e: chunk [594, -97]
  [2611월2026 13:44:40.184] [Server thread/DEBUG] [LSS/]: sent=0/tick, disk=0/0, utd=0, bw=301.7 KB/75.0 MB
  [2611월2026 13:44:40.184] [Server thread/DEBUG] [LSS/]:   WDzizon: sq=0, syncSlots=42/200, genSlots=40/40
> [2611월2026 13:44:42.260] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: [WDzizon: Stopping the server]
> [2611월2026 13:44:42.262] [Server thread/INFO] [LSS/]: Preparing LSS LOD generation tickets for final world save
  [2611월2026 13:44:42.265] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping server
  [2611월2026 13:44:42.269] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving players
  [2611월2026 13:44:42.431] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving worlds


========== 2026-11-26-3.log.gz ==========
  [2611월2026 13:42:18.029] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: [WDzizon: Set the weather to clear]
  [2611월2026 13:43:10.319] [LSS Disk Reader #2/WARN] [LSS/]: Disk read timed out (>10s) at 539, -61 — triaged as not-found (counted disk.errors; self-heals by re-declaration on gen-enabled servers) (+5 more since last report)
  [2611월2026 13:44:12.124] [LSS Disk Reader #1/WARN] [LSS/]: Disk read timed out (>10s) at 637, -93 — triaged as not-found (counted disk.errors; self-heals by re-declaration on gen-enabled servers) (+8 more since last report)
> [2611월2026 13:44:42.260] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: [WDzizon: Stopping the server]
> [2611월2026 13:44:42.262] [Server thread/INFO] [LSS/]: Preparing LSS LOD generation tickets for final world save
  [2611월2026 13:44:42.265] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping server
  [2611월2026 13:44:42.269] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving players
  [2611월2026 13:44:42.431] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving worlds


========== debug-4.log.gz ==========
  [2611월2026 13:22:03.639] [Server thread/DEBUG] [LSS/]:   WDzizon: sq=0, syncSlots=98/200, genSlots=0/40
  [2611월2026 13:22:08.642] [Server thread/DEBUG] [LSS/]: sent=0/tick, disk=0/0, utd=0, bw=193.0 KB/75.0 MB
  [2611월2026 13:22:08.642] [Server thread/DEBUG] [LSS/]:   WDzizon: sq=0, syncSlots=98/200, genSlots=0/40
> [2611월2026 13:22:11.218] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping the server
> [2611월2026 13:22:11.220] [Server thread/INFO] [LSS/]: Preparing LSS LOD generation tickets for final world save
  [2611월2026 13:22:11.222] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping server
  [2611월2026 13:22:11.223] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving players
  [2611월2026 13:22:11.479] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving worlds
  [2611월2026 13:22:11.587] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:overworld
  [2611월2026 13:22:13.432] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:the_end
  [2611월2026 13:22:13.465] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:the_nether
  [2611월2026 13:22:13.518] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM1): All chunks are saved
  [2611월2026 13:22:13.519] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM-1): All chunks are saved
  [2611월2026 13:22:13.520] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage: All dimensions are saved
> [2611월2026 13:22:14.360] [Server thread/INFO] [LSS/]: Stopping LSS LOD request processing service
  [2611월2026 13:22:14.369] [LSS-TimestampSave/DEBUG] [LSS/]: Saved 19546 timestamp cache entries to world\data\lss-timestamps.bin
  [2611월2026 13:22:14.742] [Server thread/DEBUG] [net.neoforged.fml.config.ConfigTracker/CONFIG]: Unloading configs type SERVER


========== 2026-11-26-2.log.gz ==========
  [2611월2026 13:19:02.813] [LSS Processing Thread/WARN] [LSS/]: Disk reads are concurrency-gated under sustained load (read_gate=2/2, park full): the request router is deferring cold-region reads to the next client declaration (running total: gate_stops= in /lss
lod diag). This is the gate working; raise storage.disk.max_concurrent_reads in lss-server-config.yaml and reload if server CPU headroom allows and you want faster cold backfill. (Logged once per session.)
  [2611월2026 13:20:00.762] [LSS Disk Reader #1/WARN] [LSS/]: Disk read timed out (>10s) at 591, 25 — triaged as not-found (counted disk.errors; self-heals by re-declaration on gen-enabled servers)
  [2611월2026 13:21:20.308] [LSS Disk Reader #2/WARN] [LSS/]: Disk read timed out (>10s) at 594, -9 — triaged as not-found (counted disk.errors; self-heals by re-declaration on gen-enabled servers) (+5 more since last report)
> [2611월2026 13:22:11.218] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping the server
> [2611월2026 13:22:11.220] [Server thread/INFO] [LSS/]: Preparing LSS LOD generation tickets for final world save
  [2611월2026 13:22:11.222] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping server
  [2611월2026 13:22:11.223] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving players
  [2611월2026 13:22:11.479] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving worlds
  [2611월2026 13:22:11.587] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:overworld
  [2611월2026 13:22:13.432] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:the_end
  [2611월2026 13:22:13.465] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:the_nether
  [2611월2026 13:22:13.518] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM1): All chunks are saved
  [2611월2026 13:22:13.519] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM-1): All chunks are saved
  [2611월2026 13:22:13.520] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage: All dimensions are saved
> [2611월2026 13:22:14.360] [Server thread/INFO] [LSS/]: Stopping LSS LOD request processing service


========== debug-5.log.gz ==========
  [2611월2026 12:54:12.488] [LSS-TimestampSave/DEBUG] [LSS/]: Saved 18248 timestamp cache entries to world\data\lss-timestamps.bin
  [2611월2026 12:54:15.617] [Server thread/DEBUG] [LSS/]: sent=0/tick, disk=0/0, utd=0, bw=306.3 KB/75.0 MB
  [2611월2026 12:54:15.618] [Server thread/DEBUG] [LSS/]:   WDzizon: sq=0, syncSlots=4/200, genSlots=40/40
> [2611월2026 12:54:17.784] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping the server
> [2611월2026 12:54:17.819] [Server thread/INFO] [LSS/]: Preparing LSS LOD generation tickets for final world save
  [2611월2026 12:54:17.820] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping server
  [2611월2026 12:54:17.822] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving players
  [2611월2026 12:54:17.968] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving worlds
  [2611월2026 12:54:18.380] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:overworld
  [2611월2026 12:54:24.604] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:the_end
  [2611월2026 12:54:24.637] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:the_nether
  [2611월2026 12:54:24.690] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM1): All chunks are saved
  [2611월2026 12:54:24.691] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM-1): All chunks are saved
  [2611월2026 12:54:24.692] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage: All dimensions are saved
> [2611월2026 12:54:25.548] [Server thread/INFO] [LSS/]: Stopping LSS LOD request processing service
  [2611월2026 12:54:25.553] [LSS-TimestampSave/DEBUG] [LSS/]: Saved 18304 timestamp cache entries to world\data\lss-timestamps.bin
  [2611월2026 12:54:26.043] [Server thread/DEBUG] [net.neoforged.fml.config.ConfigTracker/CONFIG]: Unloading configs type SERVER


========== 2026-11-26-1.log.gz ==========
  [2611월2026 12:53:34.508] [LSS LOD Store SQLite/INFO] [LSS/]: LOD store sweep [minecraft:overworld]: 14 changed region(s), dropped 814 stale + 0 vanished-region row(s)
  [2611월2026 12:53:34.657] [LSS Store Backfill/INFO] [LSS/]: Store backfill: 0 region(s) to process, estimated ~0 MB of new deposits (uncapped)
  [2611월2026 12:53:34.689] [LSS Store Backfill/INFO] [LSS/]: Store backfill complete: 0 regions, 0 deposited, 0 skipped, 0 errors, 0 pauses
> [2611월2026 12:54:17.784] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping the server
> [2611월2026 12:54:17.819] [Server thread/INFO] [LSS/]: Preparing LSS LOD generation tickets for final world save
  [2611월2026 12:54:17.820] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping server
  [2611월2026 12:54:17.822] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving players
  [2611월2026 12:54:17.968] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving worlds
  [2611월2026 12:54:18.380] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:overworld
  [2611월2026 12:54:24.604] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:the_end
  [2611월2026 12:54:24.637] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:the_nether
  [2611월2026 12:54:24.690] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM1): All chunks are saved
  [2611월2026 12:54:24.691] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM-1): All chunks are saved
  [2611월2026 12:54:24.692] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage: All dimensions are saved
> [2611월2026 12:54:25.548] [Server thread/INFO] [LSS/]: Stopping LSS LOD request processing service


========== 2026-11-25-6.log.gz ==========
  [2511월2026 23:38:12.824] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: LOD-only archive reads: requests=102 started=7 hits=0 misses=5 failures=0 queue_rejected=64 shutdown_rejected=0 hit_bytes=0 may_send_denied=0 egress_permits=0 permit_release
s=0 | archive_lookup_reasons: requests=7 selected_rows=0 global_blocked=4 session_visit_blocked=1 session_invalidation_blocked=0 row_missing=0 row_invalidated=0 durable_visited_row=0 unexpected_filtered=0 post_select_blocked=0 | archive_lookup_dimensions: [minecr
aft:overworld{requests=7,selected=0,missing=0,invalidated=0,durable_visited=0,global_blocked=4,session_visit_blocked=1,session_invalidation_blocked=0,post_select_blocked=0}]
  [2511월2026 23:38:17.775] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: LOD-only archive rows: total=2886 valid=2269 invalidated=617 valid_unvisited=2269 valid_with_visit_marker=0 durable_visited_total=2468 | archive_row_dimensions: [minecraft:o
verworld{total=2886,valid=2269,invalidated=617,valid_unvisited=2269,valid_with_visit_marker=0,durable_visited_total=2468}]
  [2511월2026 23:39:06.721] [LSS Disk Reader #1/WARN] [LSS/]: Disk read timed out (>10s) at 577, 31 — triaged as not-found (counted disk.errors; self-heals by re-declaration on gen-enabled servers) (+7 more since last report)
> [2511월2026 23:40:01.792] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping the server
> [2511월2026 23:40:01.837] [Server thread/INFO] [LSS/]: Preparing LSS LOD generation tickets for final world save
  [2511월2026 23:40:01.837] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping server
  [2511월2026 23:40:01.839] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving players
  [2511월2026 23:40:02.038] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving worlds
  [2511월2026 23:40:02.327] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:overworld
  [2511월2026 23:40:08.050] [LSS Disk Reader #2/WARN] [LSS/]: Disk read timed out (>10s) at 583, 44 — triaged as not-found (counted disk.errors; self-heals by re-declaration on gen-enabled servers) (+3 more since last report)
  [2511월2026 23:40:13.297] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:the_end
  [2511월2026 23:40:13.376] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM1): All chunks are saved
  [2511월2026 23:40:13.377] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM-1): All chunks are saved
  [2511월2026 23:40:13.379] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage: All dimensions are saved
> [2511월2026 23:40:14.318] [Server thread/INFO] [LSS/]: Stopping LSS LOD request processing service


========== 2026-11-25-5.log.gz ==========
  [2511월2026 23:35:37.787] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: notepad "D:\���¿�\����\����ũ����Ʈ\����\1.21.1 vss modifying test\run.bat"<--[HERE]
  [2511월2026 23:35:42.886] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Unknown or incomplete command, see below for error
  [2511월2026 23:35:42.886] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: stio<--[HERE]
> [2511월2026 23:35:43.892] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping the server
> [2511월2026 23:35:43.935] [Server thread/INFO] [LSS/]: Preparing LSS LOD generation tickets for final world save
  [2511월2026 23:35:43.936] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping server
  [2511월2026 23:35:43.937] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving players
  [2511월2026 23:35:43.939] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving worlds
  [2511월2026 23:35:43.969] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:overworld
  [2511월2026 23:35:44.152] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:the_end
  [2511월2026 23:35:44.186] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:the_nether
  [2511월2026 23:35:44.239] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM1): All chunks are saved
  [2511월2026 23:35:44.242] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM-1): All chunks are saved
  [2511월2026 23:35:44.243] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage: All dimensions are saved
> [2511월2026 23:35:44.339] [Server thread/INFO] [LSS/]: Stopping LSS LOD request processing service


========== 2026-11-25-4.log.gz ==========
  [2511월2026 23:22:23.364] [LSS LOD Store SQLite/INFO] [LSS/]: LOD store sweep [minecraft:overworld]: 21 changed region(s), dropped 2034 stale + 0 vanished-region row(s)
  [2511월2026 23:22:23.373] [LSS Store Backfill/INFO] [LSS/]: Store backfill: 11 region(s) to process, estimated ~1 MB of new deposits (uncapped)
  [2511월2026 23:22:24.382] [LSS Store Backfill/INFO] [LSS/]: Store backfill complete: 11 regions, 0 deposited, 518 skipped, 0 errors, 0 pauses
> [2511월2026 23:25:34.113] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping the server
> [2511월2026 23:25:34.156] [Server thread/INFO] [LSS/]: Preparing LSS LOD generation tickets for final world save
  [2511월2026 23:25:34.158] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping server
  [2511월2026 23:25:34.159] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving players
  [2511월2026 23:25:34.159] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving worlds
  [2511월2026 23:25:34.186] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:overworld
  [2511월2026 23:25:34.380] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:the_end
  [2511월2026 23:25:34.414] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:the_nether
  [2511월2026 23:25:34.467] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM1): All chunks are saved
  [2511월2026 23:25:34.470] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM-1): All chunks are saved
  [2511월2026 23:25:34.471] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage: All dimensions are saved
> [2511월2026 23:25:34.549] [Server thread/INFO] [LSS/]: Stopping LSS LOD request processing service


========== 2026-11-25-3.log.gz ==========
  [2511월2026 23:04:43.874] [LSS Disk Reader #3/WARN] [LSS/]: Disk read timed out (>10s) at 468, 61 — triaged as not-found (counted disk.errors; self-heals by re-declaration on gen-enabled servers) (+9 more since last report)
  [2511월2026 23:05:59.209] [LSS Disk Reader #3/WARN] [LSS/]: Disk read timed out (>10s) at 498, -53 — triaged as not-found (counted disk.errors; self-heals by re-declaration on gen-enabled servers) (+9 more since last report)
  [2511월2026 23:07:00.510] [LSS Disk Reader #1/WARN] [LSS/]: Disk read timed out (>10s) at 450, -39 — triaged as not-found (counted disk.errors; self-heals by re-declaration on gen-enabled servers) (+7 more since last report)
> [2511월2026 23:07:22.356] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping the server
> [2511월2026 23:07:22.402] [Server thread/INFO] [LSS/]: Preparing LSS LOD generation tickets for final world save
  [2511월2026 23:07:22.402] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping server
  [2511월2026 23:07:22.405] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving players
  [2511월2026 23:07:22.562] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving worlds
  [2511월2026 23:07:22.665] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:overworld
  [2511월2026 23:07:52.455] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:the_end
  [2511월2026 23:07:52.488] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:the_nether
  [2511월2026 23:07:52.543] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM1): All chunks are saved
  [2511월2026 23:07:52.544] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM-1): All chunks are saved
  [2511월2026 23:07:52.544] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage: All dimensions are saved
> [2511월2026 23:07:54.724] [Server thread/INFO] [LSS/]: Stopping LSS LOD request processing service


========== 2026-11-25-2.log.gz ==========
  [2511월2026 19:11:40.377] [LSS Disk Reader #1/WARN] [LSS/]: Disk read timed out (>10s) at 529, 54 — triaged as not-found (counted disk.errors; self-heals by re-declaration on gen-enabled servers) (+5 more since last report)
  [2511월2026 19:12:36.877] [Server thread/INFO] [net.minecraft.server.network.ServerGamePacketListenerImpl/]: WDzizon lost connection: Disconnected
  [2511월2026 19:12:36.878] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: WDzizon left the game
> [2511월2026 19:12:43.417] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping the server
> [2511월2026 19:12:43.467] [Server thread/INFO] [LSS/]: Preparing LSS LOD generation tickets for final world save
  [2511월2026 19:12:43.467] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping server
  [2511월2026 19:12:43.468] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving players
  [2511월2026 19:12:43.468] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving worlds
  [2511월2026 19:12:43.477] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:overworld
  [2511월2026 19:12:44.192] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:the_end
  [2511월2026 19:12:44.226] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:the_nether
  [2511월2026 19:12:44.287] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM1): All chunks are saved
  [2511월2026 19:12:44.287] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM-1): All chunks are saved
  [2511월2026 19:12:44.287] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage: All dimensions are saved
> [2511월2026 19:12:45.853] [Server thread/INFO] [LSS/]: Stopping LSS LOD request processing service


========== 2026-11-25-1.log.gz ==========
  [2511월2026 18:46:19.741] [LSS Disk Reader #2/WARN] [LSS/]: Disk read timed out (>10s) at 443, 53 — triaged as not-found (counted disk.errors; self-heals by re-declaration on gen-enabled servers) (+4 more since last report)
  [2511월2026 18:47:02.792] [Server thread/INFO] [net.minecraft.server.network.ServerGamePacketListenerImpl/]: WDzizon lost connection: Disconnected
  [2511월2026 18:47:02.793] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: WDzizon left the game
> [2511월2026 18:52:38.841] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping the server
> [2511월2026 18:52:38.890] [Server thread/INFO] [LSS/]: Preparing LSS LOD generation tickets for final world save
  [2511월2026 18:52:38.891] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping server
  [2511월2026 18:52:38.892] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving players
  [2511월2026 18:52:38.892] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving worlds
  [2511월2026 18:52:38.901] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:overworld
  [2511월2026 18:52:39.298] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:the_nether
  [2511월2026 18:52:39.332] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:the_end
  [2511월2026 18:52:39.393] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM-1): All chunks are saved
  [2511월2026 18:52:39.393] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM1): All chunks are saved
  [2511월2026 18:52:39.393] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage: All dimensions are saved
> [2511월2026 18:52:40.567] [Server thread/INFO] [LSS/]: Stopping LSS LOD request processing service


========== 2026-11-24-4.log.gz ==========
  [2411월2026 15:50:26.570] [LSS Disk Reader #1/WARN] [LSS/]: Disk read timed out (>10s) at 1819, 1906 — triaged as not-found (counted disk.errors; self-heals by re-declaration on gen-enabled servers) (+8 more since last report)
  [2411월2026 15:51:35.552] [LSS Disk Reader #1/WARN] [LSS/]: Disk read timed out (>10s) at 1930, 1904 — triaged as not-found (counted disk.errors; self-heals by re-declaration on gen-enabled servers) (+7 more since last report)
  [2411월2026 15:53:10.315] [LSS Disk Reader #1/WARN] [LSS/]: Disk read timed out (>10s) at 1821, 1932 — triaged as not-found (counted disk.errors; self-heals by re-declaration on gen-enabled servers) (+7 more since last report)
> [2411월2026 15:53:20.759] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: [WDzizon: Stopping the server]
> [2411월2026 15:53:20.806] [Server thread/INFO] [LSS/]: Preparing LSS LOD generation tickets for final world save
  [2411월2026 15:53:20.808] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping server
  [2411월2026 15:53:20.810] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving players
  [2411월2026 15:53:21.054] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving worlds


========== 2026-11-24-3.log.gz ==========
  [2411월2026 15:21:20.517] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: LOD-only preservation: inspected=935 candidates_at_generation=0 snapshot_candidates_at_generation=121 protected_area=684 player_watched_before_generation=0 uncertain_player_
access=121 structure_starts=1 structure_references=129 uncertain=0 watch_index=count=906,supported=true,overflow=false,archive=ready,visit_write_failed=false,history=positive-only,scope=session-only structure_inspection_failed=false deletion=DISABLED | LOD-only a
rchive: state=ready schema=2 queue=732/4096 visit_history=positive-only absence=unknown invalidations_pending=525 egress_invalidation_blocked=true egress_visit_publication_blocked=false archive_untrusted=false session_visits=906 session_visit_overflow=false sessi
on_invalidations=1454 session_invalidation_overflow=false tracking_started_ms=1795501102485 durable_visit_write_failed=false | LOD-only snapshot writes: attempts=121 committed=121 protected_noop=0 failures=0
  [2411월2026 15:21:37.218] [LSS Processing Thread/WARN] [LSS/]: Disk reads are concurrency-gated under sustained load (read_gate=2/2, park full): the request router is deferring cold-region reads to the next client declaration (running total: gate_stops= in /lss
lod diag). This is the gate working; raise storage.disk.max_concurrent_reads in lss-server-config.yaml and reload if server CPU headroom allows and you want faster cold backfill. (Logged once per session.)
  [2411월2026 15:23:27.809] [Server thread/WARN] [net.minecraft.server.MinecraftServer/]: Can't keep up! Is the server overloaded? Running 2106ms or 42 ticks behind
> [2411월2026 15:25:58.970] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: [WDzizon: Stopping the server]
> [2411월2026 15:25:59.004] [Server thread/INFO] [LSS/]: Preparing LSS LOD generation tickets for final world save
  [2411월2026 15:25:59.005] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping server
  [2411월2026 15:25:59.010] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving players
  [2411월2026 15:25:59.106] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving worlds
  [2411월2026 15:26:01.734] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:overworld
  [2411월2026 15:26:08.772] [LSS Disk Reader #2/WARN] [LSS/]: Disk read timed out (>10s) at 1879, 1848 — triaged as not-found (counted disk.errors; self-heals by re-declaration on gen-enabled servers) (+10 more since last report)
  [2411월2026 15:26:35.406] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Saving chunks for level 'ServerLevel[world]'/minecraft:the_nether
  [2411월2026 15:26:35.552] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM-1): All chunks are saved
  [2411월2026 15:26:35.553] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage (DIM1): All chunks are saved
  [2411월2026 15:26:35.554] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: ThreadedAnvilChunkStorage: All dimensions are saved
> [2411월2026 15:26:38.166] [Server thread/INFO] [LSS/]: Stopping LSS LOD request processing service
