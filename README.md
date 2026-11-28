wdzizon@DESKTOP-LS6DH9N:~/lod-server-support-lod-only$ cd ~/lod-server-support-lod-only &&
> git pull --ff-only origin feat/lod-only-preservation-1.21.1 &&
> ./gradlew :common:test :neoforge:test :neoforge:compileGametestJava :neoforge:runGameTestServer :neoforge:build
remote: Enumerating objects: 128, done.
remote: Counting objects: 100% (128/128), done.
remote: Compressing objects: 100% (68/68), done.
remote: Total 102 (delta 38), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (102/102), 15.54 KiB | 1.11 MiB/s, done.
Resolving deltas: 100% (38/38), completed with 10 local objects.
From https://github.com/WDzizon/lod-server-support-lod-only
 * branch                feat/lod-only-preservation-1.21.1 -> FETCH_HEAD
   a0f9fa641..e8fc80528  feat/lod-only-preservation-1.21.1 -> origin/feat/lod-only-preservation-1.21.1
Updating a0f9fa641..e8fc80528
Fast-forward
 docs/planning/lod-only-preservation-plan.md                                 |  76 ++++++++-
 .../src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java    | 173 ++++++++++++++++----
 .../dev/vox/lss/networking/server/NeoForgeChunkSideStoreCoordinator.java    | 318 ++++++++++++++++++++++++++++++++++--
 .../dev/vox/lss/networking/server/NeoForgeEntityStorageAdmissionGate.java   |  43 +++++
 .../dev/vox/lss/neoforge/NeoForgeChunkSideStoreCoordinatorContractTest.java |  56 ++++++-
 5 files changed, 621 insertions(+), 45 deletions(-)
│█████··│█████··
> Configure project :fabricic
Fabric Loom: 1.17.13dependencies of :fabric:mappings
│██████│████│█│█
> Configure project :sponge
SpongePowered Plugin 'GRADLE' Toolset Version '2.3.0'
Targeting Minecraft '1.21.1' on a 'SERVER' platform
│██████·│██████·
> Task :neoforge:compileJava FAILED
/home/wdzizon/lod-server-support-lod-only/neoforge/src/main/java/dev/vox/lss/networking/server/NeoForgeChunkSideStoreCoordinator.java:181: error: method tryAcquireWorkers in class NeoForgeChunkSideStoreCoordinator cannot be applied to given types;
        return tryAcquireWorkers(level, position, null,
               ^
  required: ServerLevel,ChunkPos,EntityStorage,Lease,long,long,boolean
  found:    ServerLevel,ChunkPos,<null>,long,long,boolean
  reason: actual and formal argument lists differ in length
/home/wdzizon/lod-server-support-lod-only/neoforge/src/main/java/dev/vox/lss/networking/server/NeoForgeChunkSideStoreCoordinator.java:182: error: incompatible types: long cannot be converted to Lease
                NeoForgePoiMutationTracker.revision(poiManager, position),
                                                   ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/main/java/dev/vox/lss/networking/server/NeoForgeChunkSideStoreCoordinator.java:638: error: cannot find symbol
                                    failure = loadFailure;
                                              ^
  symbol:   variable loadFailure
  location: class Acquisition
/home/wdzizon/lod-server-support-lod-only/neoforge/src/main/java/dev/vox/lss/networking/server/NeoForgeChunkSideStoreCoordinator.java:639: error: cannot find symbol
                                } else if (loadFailure != null) {
                                           ^
  symbol:   variable loadFailure
  location: class Acquisition
/home/wdzizon/lod-server-support-lod-only/neoforge/src/main/java/dev/vox/lss/networking/server/NeoForgeChunkSideStoreCoordinator.java:640: error: cannot find symbol
                                    failure.addSuppressed(loadFailure);
                                                          ^
  symbol:   variable loadFailure
  location: class Acquisition
Note: Some messages have been simplified; recompile with -Xdiags:verbose to get full output
5 errors

[Incubating] Problems report is available at: file:///home/wdzizon/lod-server-support-lod-only/build/reports/problems/problems-report.html
│██████▍
FAILURE: Build failed with an exception.

* What went wrong:
Execution failed for task ':neoforge:compileJava' (registered by plugin class 'org.gradle.api.plugins.JavaBasePlugin').
> Compilation failed; see the compiler output below.
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/main/java/dev/vox/lss/networking/server/NeoForgeChunkSideStoreCoordinator.java:181: error: method tryAcquireWorkers in class NeoForgeChunkSideStoreCoordinator cannot be applied to given types;
          return tryAcquireWorkers(level, position, null,
                 ^
    required: ServerLevel,ChunkPos,EntityStorage,Lease,long,long,boolean
    found:    ServerLevel,ChunkPos,<null>,long,long,boolean
    reason: actual and formal argument lists differ in length
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/main/java/dev/vox/lss/networking/server/NeoForgeChunkSideStoreCoordinator.java:182: error: incompatible types: long cannot be converted to Lease
                  NeoForgePoiMutationTracker.revision(poiManager, position),
                                                     ^
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/main/java/dev/vox/lss/networking/server/NeoForgeChunkSideStoreCoordinator.java:638: error: cannot find symbol
                                      failure = loadFailure;
                                                ^
    symbol:   variable loadFailure
    location: class Acquisition
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/main/java/dev/vox/lss/networking/server/NeoForgeChunkSideStoreCoordinator.java:639: error: cannot find symbol
                                  } else if (loadFailure != null) {
                                             ^
    symbol:   variable loadFailure
    location: class Acquisition
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/main/java/dev/vox/lss/networking/server/NeoForgeChunkSideStoreCoordinator.java:640: error: cannot find symbol
                                      failure.addSuppressed(loadFailure);
                                                            ^
    symbol:   variable loadFailure
    location: class Acquisition
  Note: Some messages have been simplified; recompile with -Xdiags:verbose to get full output
  5 errors

* Try:
> Check your code and dependencies to fix the compilation error(s)
> Run with --scan to get full insights from a Build Scan (powered by Develocity).

BUILD FAILED in 4s
13 actionable tasks: 1 executed, 12 up-to-date
