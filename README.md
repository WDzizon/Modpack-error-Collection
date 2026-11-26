  [2611??026 13:50:18.694] [Server thread/INFO] [net.minecraft.server.dedicated.DedicatedServer/]: Done (1.907s)! For h
elp, type "help"
  [2611??026 13:50:18.732] [Server thread/INFO] [net.neoforged.neoforge.server.permission.PermissionAPI/]: Successfully
 initialized permission handler neoforge:default_handler
> [2611??026 13:50:18.765] [Server thread/WARN] [LSS/]: LOD-only archive unavailable; historical player-visit state is
uncertain and chunk deletion remains disabled | LOD-only recovery inspection: mode=filesystem-only auto_recovery=disabl
ed directory=directory session_marker=regular(63B) invalidation_marker=missing archive_db=regular(182325248B) wal=regul
ar(4165352B) shm=regular(32768B) journal=missing lock_file=regular(0B) operator_review=required
> java.io.IOException: LOD-only archive has an unclean previous session marker; preserving the database and refusing to
 serve archived LOD
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.common.lodonly.LodOnlyArchiveStore.<init>(LodOnlyArchiveStore.java:319) ~[lod-
server-support-neoforge.jar%23120!/:?]
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.common.lodonly.LodOnlyArchiveStore.open(LodOnlyArchiveStore.java:272) ~[lod-se
rver-support-neoforge.jar%23120!/:?]
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.common.lodonly.LodOnlyArchiveStore.open(LodOnlyArchiveStore.java:268) ~[lod-se
rver-support-neoforge.jar%23120!/:?]
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.LSSServerNetworking.openLodOnlyArchive(LSSServerNetworking.j
ava:72) ~[lod-server-support-neoforge.jar%23120!/:?]
  [2611??026 13:50:19.374] [Server thread/INFO] [LSS/]: Effective config: useNbtTranscode=true, diskReaderThreads=3, us
eCompressedColumns=true, useBackgroundReadSplit=true, useSelectiveNbtParse=true, maxConcurrentDiskReads=2
  [2611??026 13:50:19.585] [Server thread/INFO] [LSS/]: Dirty content filter: seeded 49 already-loaded chunk(s)
> [2611??026 13:50:24.345] [LSS LOD Store SQLite/INFO] [LSS/]: LOD store sweep [minecraft:overworld]: 26 changed region
(s), dropped 5196 stale + 0 vanished-region row(s)
  [2611??026 13:50:24.357] [LSS Store Backfill/INFO] [LSS/]: Store backfill: 15 region(s) to process, estimated ~33 MB
of new deposits (uncapped)
  [2611??026 13:50:35.535] [LSS Store Backfill/INFO] [LSS/]: Store backfill complete: 15 regions, 2151 deposited, 3517
skipped, 0 errors, 0 pauses
  [2611??026 13:50:42.645] [User Authenticator #1/INFO] [net.minecraft.server.network.ServerLoginPacketListenerImpl/]:
UUID of player WDzizon is ea04c93a-d122-4b7b-baee-1c53d5ae535e
  [2611??026 13:50:44.035] [Server thread/INFO] [net.minecraft.server.players.PlayerList/]: WDzizon[/[::1]:7737] logged
 in with entity id 5 at (9403.770578746604, 75.0, -757.349223386137)
  [2611??026 13:50:44.137] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: WDzizon joined the game
> [2611??026 13:50:44.440] [Server thread/WARN] [LSS/]: LOD-only durable player-visit recording failed; visit history i
s untrusted and the affected world data must be preserved
  java.lang.IllegalStateException: LOD-only durable visit archive is unavailable
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.ServerReceiverGlue.markPlayerWatched(ServerReceiverGlue.java
:120) ~[lod-server-support-neoforge.jar%23120!/:?]
        at TRANSFORMER/lss@0.23.0/dev.vox.lss.networking.server.LSSServerNetworking.onChunkWatch(LSSServerNetworking.java:18
2) ~[lod-server-support-neoforge.jar%23120!/:?]
        at MC-BOOTSTRAP/net.neoforged.bus/net.neoforged.bus.ConsumerEventHandler.invoke(ConsumerEventHandler.java:27) ~[bus-
8.0.5.jar%2362!/:?]
  [2611??026 13:52:05.424] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Bandwidth: 891.7 KB/s / 75.0 M
B/s global (48.9 MB total, 8.5 MB wire, cols zstd=1519 raw=0)
  [2611??026 13:52:05.424] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]:   WDzizon: sq=0/1024, psync=98
, pgen=0, sent=1519 (48.9 MB), rate=14/s, obuf=0 B/93.6 KB, pingf=1.00, yielded=0, paced=13
> [2611??026 13:52:05.436] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: LOD-only preservation: inspect
ed=757 candidates_at_generation=0 snapshot_candidates_at_generation=0 protected_area=0 player_watched_before_generation
=5 uncertain_player_access=539 structure_starts=9 structure_references=204 uncertain=0 watch_index=count=1554,supported
=true,overflow=false,archive=unavailable,visit_write_failed=true,history=positive-only,scope=session-only structure_ins
pection_failed=false deletion=DISABLED | LOD-only archive: state=unavailable attached=false durable_visit_write_failed=
true | LOD-only recovery inspection: mode=filesystem-only auto_recovery=disabled directory=directory session_marker=reg
ular(63B) invalidation_marker=missing archive_db=regular(182325248B) wal=regular(4165352B) shm=regular(32768B) journal=
missing lock_file=regular(0B) operator_review=required | LOD-only snapshot writes: attempts=0 committed=0 protected_noo
p=0 failures=0
  [2611??026 13:52:05.845] [LSS Processing Thread/WARN] [LSS/]: Disk reads are concurrency-gated under sustained load (
read_gate=2/2, park full): the request router is deferring cold-region reads to the next client declaration (running to
tal: gate_stops= in /lsslod diag). This is the gate working; raise storage.disk.max_concurrent_reads in lss-server-conf
ig.yaml and reload if server CPU headroom allows and you want faster cold backfill. (Logged once per session.)
  [2611??026 13:54:20.160] [LSS Disk Reader #1/WARN] [LSS/]: Disk read timed out (>10s) at 535, -109 ??triaged as not-f
ound (counted disk.errors; self-heals by re-declaration on gen-enabled servers)
  [2611??026 13:54:30.591] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Stopping the server
  [2611??026 13:54:30.592] [Server thread/INFO] [LSS/]: Preparing LSS LOD generation tickets for final world save

========== debug-3.log.gz ==========
  [2611월2026 13:25:26.567] [Server thread/DEBUG] [net.neoforged.neoforge.server.LanguageHook/]: Loaded 4 language file
s for en_us
  [2611월2026 13:25:26.579] [Server thread/INFO] [net.neoforged.neoforge.server.permission.PermissionAPI/]: Successfull
y initialized permission handler neoforge:default_handler
> [2611월2026 13:25:27.363] [Server thread/INFO] [LSS/]: LOD-only durable archive ready: LOD-only archive: state=ready
schema=2 queue=0/4096 visit_history=positive-only absence=unknown invalidations_pending=0 invalidation_jobs=0/0/0 inval
idation_batches=0 archive_write_batches=0 invalidation_active=false invalidation_last_started_age_ms=-1 invalidation_la
st_completed_age_ms=-1 egress_invalidation_blocked=false egress_visit_publication_blocked=false archive_untrusted=false
 session_visits=0 session_visit_overflow=false session_invalidations=0 session_invalidation_overflow=false tracking_sta
rted_ms=1795596825561
  [2611월2026 13:25:27.364] [Server thread/INFO] [LSS/]: Starting LSS LOD request processing service
  [2611월2026 13:25:27.417] [Server thread/INFO] [LSS/]: Loaded 19546 timestamp cache entries from world\data\lss-times
tamps.bin
  [2611월2026 13:25:28.003] [Server thread/INFO] [LSS/]: LOD store active (driver=private/3.49.1.0). It stores served L
OD bytes under <world>/lss-lod/ and, once fully warmed, occupies roughly as much space as the region files themselves.
It is DERIVED data — deleting lss-lod/ is always safe. Set storage.lod_store.enabled to false and restart to disable; s
torage.lod_store.max_size_mib bounds its size after reload.
  [2611월2026 13:25:28.011] [Server thread/INFO] [LSS/]: Effective config: useNbtTranscode=true, diskReaderThreads=3, u
seCompressedColumns=true, useBackgroundReadSplit=true, useSelectiveNbtParse=true, maxConcurrentDiskReads=2
  [2611월2026 13:25:28.198] [Server thread/INFO] [LSS/]: Dirty content filter: seeded 49 already-loaded chunk(s)
> [2611월2026 13:25:29.957] [LSS LOD Store SQLite/INFO] [LSS/]: LOD store sweep [minecraft:overworld]: 13 changed regio
n(s), dropped 1030 stale + 0 vanished-region row(s)
  [2611월2026 13:25:29.966] [LSS Store Backfill/INFO] [LSS/]: Store backfill: 0 region(s) to process, estimated ~0 MB o
f new deposits (uncapped)
  [2611월2026 13:25:29.970] [LSS Store Backfill/INFO] [LSS/]: Store backfill complete: 0 regions, 0 deposited, 0 skippe
d, 0 errors, 0 pauses
  [2611월2026 13:25:33.152] [Server thread/DEBUG] [LSS/]: sent=0/tick, disk=0/0, utd=0, bw=0 B/75.0 MB
  [2611월2026 13:25:38.150] [Server thread/DEBUG] [LSS/]: sent=0/tick, disk=0/0, utd=0, bw=0 B/75.0 MB
  [2611월2026 13:29:23.493] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: Bandwidth: 757.0 KB/s / 75.0
MB/s global (77.9 MB total, 13.1 MB wire, cols zstd=2320 raw=0)
  [2611월2026 13:29:23.494] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]:   WDzizon: sq=0/1024, psync=9
8, pgen=40, sent=2320 (77.9 MB), rate=10/s, obuf=1.3 KB/64.3 KB, pingf=1.00, yielded=0, paced=14
> [2611월2026 13:29:23.508] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: LOD-only preservation: inspec
ted=1063 candidates_at_generation=0 snapshot_candidates_at_generation=795 protected_area=0 player_watched_before_genera
tion=0 uncertain_player_access=795 structure_starts=2 structure_references=266 uncertain=0 watch_index=count=1486,suppo
rted=true,overflow=false,archive=ready,visit_write_failed=false,history=positive-only,scope=session-only structure_insp
ection_failed=false deletion=DISABLED | LOD-only archive: state=ready schema=2 queue=0/4096 visit_history=positive-only
 absence=unknown invalidations_pending=0 invalidation_jobs=2222/2222/0 invalidation_batches=262 archive_write_batches=4
00 invalidation_active=false invalidation_last_started_age_ms=304 invalidation_last_completed_age_ms=119 egress_invalid
ation_blocked=false egress_visit_publication_blocked=false archive_untrusted=false session_visits=1486 session_visit_ov
erflow=false session_invalidations=1398 session_invalidation_overflow=false tracking_started_ms=1795596825561 durable_v
isit_write_failed=false | LOD-only snapshot writes: attempts=795 committed=329 protected_noop=466 failures=0
> [2611월2026 13:29:23.518] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: LOD-only archive reads: reque
sts=1963 started=1963 hits=0 misses=1963 failures=0 queue_rejected=0 shutdown_rejected=0 hit_bytes=0 may_send_denied=0
egress_permits=0 permit_releases=0 | archive_lookup_reasons: requests=1963 selected_rows=0 global_blocked=32 session_vi
sit_blocked=55 session_invalidation_blocked=99 row_missing=1776 row_invalidated=1 durable_visited_row=0 unexpected_filt
ered=0 post_select_blocked=0 | archive_lookup_dimensions: [minecraft:overworld{requests=1963,selected=0,missing=1776,in
validated=1,durable_visited=0,global_blocked=32,session_visit_blocked=55,session_invalidation_blocked=99,post_select_bl
ocked=0}]
  [2611월2026 13:29:23.628] [Server thread/INFO] [net.minecraft.server.MinecraftServer/]: LOD-only archive rows: total=
4026 valid=3153 invalidated=873 valid_unvisited=3153 valid_with_visit_marker=0 durable_visited_total=3595 | archive_row
_dimensions: [minecraft:overworld{total=4026,valid=3153,invalidated=873,valid_unvisited=3153,valid_with_visit_marker=0,
durable_visited_total=3595}]
  [2611월2026 13:29:25.007] [Server thread/DEBUG] [LSS/]: sent=0/tick, disk=0/0, utd=0, bw=342.1 KB/75.0 MB
  [2611월2026 13:29:25.007] [Server thread/DEBUG] [LSS/]:   WDzizon: sq=0, syncSlots=98/200, genSlots=0/40
  [2611월2026 13:29:27.009] [LSS-TimestampSave/DEBUG] [LSS/]: Saved 20599 timestamp cache entries to world\data\lss-tim
estamps.bin
