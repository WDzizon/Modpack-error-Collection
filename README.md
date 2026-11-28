wdzizon@DESKTOP-LS6DH9N:~/lod-server-support-lod-only$ cd ~/lod-server-support-lod-only &&
> git pull --ff-only origin feat/lod-only-preservation-1.21.1 &&
> ./gradlew :common:test :neoforge:test :neoforge:compileGametestJava :neoforge:runGameTestServer :neoforge:build
remote: Enumerating objects: 31, done.
remote: Counting objects: 100% (31/31), done.
remote: Compressing objects: 100% (15/15), done.
remote: Total 17 (delta 9), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (17/17), 2.20 KiB | 173.00 KiB/s, done.
From https://github.com/WDzizon/lod-server-support-lod-only
 * branch                feat/lod-only-preservation-1.21.1 -> FETCH_HEAD
   85f43a86f..e66a0c9a9  feat/lod-only-preservation-1.21.1 -> origin/feat/lod-only-preservation-1.21.1
Updating 85f43a86f..e66a0c9a9
Fast-forward
 docs/planning/lod-only-preservation-plan.md                                                 | 43 +++++++++++++++++++++++++++++++++++++++++++
 neoforge/src/main/java/dev/vox/lss/networking/server/NeoForgeChunkRecordRemovalAdapter.java |  2 +-
 2 files changed, 44 insertions(+), 1 deletion(-)
│·······│█████··│█████··│█████··│█████··│█████··│█████··
> Configure project :fabric:fabric > :fabric           > :fabric > :fabric
Fabric Loom: 1.17.13
│████│█
> Configure project :sponge
SpongePowered Plugin 'GRADLE' Toolset Version '2.3.0'
Targeting Minecraft '1.21.1' on a 'SERVER' platform
│████···│█████▋·│██████·│██████·│██████│█████│███│███
> Task :neoforge:test FAILED

NeoForgeIOWorkerNullStoreContractTest > executableProbeUsesOnlyAnIsolatedTemporaryStorageDirectory() FAILED
    org.opentest4j.AssertionFailedError at NeoForgeIOWorkerNullStoreContractTest.java:51

74 tests completed, 1 failed

FAILURE: Build failed with an exception.

* What went wrong:
Execution failed for task ':neoforge:test'.
> There were failing tests. See the report at: file:///home/wdzizon/lod-server-support-lod-only/neoforge/build/reports/tests/test/index.html

* Try:
> Run with --scan to get full insights from a Build Scan (powered by Develocity).

BUILD FAILED in 5s
18 actionable tasks: 3 executed, 15 up-to-date
