wdzizon@DESKTOP-LS6DH9N:~/lod-server-support-lod-only$ cd ~/lod-server-support-lod-only &&
> git pull --ff-only origin feat/lod-only-preservation-1.21.1 &&
> ./gradlew :common:test :neoforge:test :neoforge:compileGametestJava :neoforge:runGameTestServer :neoforge:build
remote: Enumerating objects: 113, done.
remote: Counting objects: 100% (113/113), done.
remote: Compressing objects: 100% (54/54), done.
remote: Total 86 (delta 23), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (86/86), 13.50 KiB | 314.00 KiB/s, done.
From https://github.com/WDzizon/lod-server-support-lod-only
 * branch                feat/lod-only-preservation-1.21.1 -> FETCH_HEAD
   cd783f2ec..063557dae  feat/lod-only-preservation-1.21.1 -> origin/feat/lod-only-preservation-1.21.1
Updating cd783f2ec..063557dae
Fast-forward
 docs/planning/lod-only-preservation-plan.md                                 |  53 +++++++++++++
 .../src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java    | 128 +++++++++++++++++++++++++++++++
 .../java/dev/vox/lss/mixin/DistanceManagerTicketMutationTrackerMixin.java   | 106 ++++++++++++++++++++++++++
 .../dev/vox/lss/networking/server/NeoForgeChunkSideStoreCoordinator.java    |  54 ++++++++++++-
 .../lss/networking/server/NeoForgeDistanceManagerTicketMutationTracker.java | 148 ++++++++++++++++++++++++++++++++++++
 neoforge/src/main/resources/lss.neoforge.mixins.json                        |   1 +
 .../vox/lss/neoforge/NeoForgeDistanceManagerTicketMutationContractTest.java |  55 ++++++++++++++
 7 files changed, 543 insertions(+), 2 deletions(-)
 create mode 100644 neoforge/src/main/java/dev/vox/lss/mixin/DistanceManagerTicketMutationTrackerMixin.java
 create mode 100644 neoforge/src/main/java/dev/vox/lss/networking/server/NeoForgeDistanceManagerTicketMutationTracker.java
 create mode 100644 neoforge/src/test/java/dev/vox/lss/neoforge/NeoForgeDistanceManagerTicketMutationContractTest.java
│█████··
> Configure project :fabric
Fabric Loom: 1.17.13
│██████│████│█
> Configure project :sponge
SpongePowered Plugin 'GRADLE' Toolset Version '2.3.0'
Targeting Minecraft '1.21.1' on a 'SERVER' platform
│███
> Task :neoforge:test FAILED

NeoForgeDistanceManagerTicketMutationContractTest > coordinatorRechecksTargetRelevantTicketHistoryBeforeAndAtCommitSeal() FAILED
    org.opentest4j.AssertionFailedError at NeoForgeDistanceManagerTicketMutationContractTest.java:48

72 tests completed, 1 failed

FAILURE: Build failed with an exception.

* What went wrong:
Execution failed for task ':neoforge:test'.
> There were failing tests. See the report at: file:///home/wdzizon/lod-server-support-lod-only/neoforge/build/reports/tests/test/index.html

* Try:
> Run with --scan to get full insights from a Build Scan (powered by Develocity).

BUILD FAILED in 5s
18 actionable tasks: 5 executed, 13 up-to-date
