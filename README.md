wdzizon@DESKTOP-LS6DH9N:~/lod-server-support-lod-only$ cd ~/lod-server-support-lod-only &&
> git pull --ff-only origin feat/lod-only-preservation-1.21.1 &&
> ./gradlew :common:test :neoforge:test :neoforge:compileGametestJava :neoforge:runGameTestServer :neoforge:build
remote: Enumerating objects: 55, done.
remote: Counting objects: 100% (55/55), done.
remote: Compressing objects: 100% (26/26), done.
remote: Total 41 (delta 10), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (41/41), 6.22 KiB | 212.00 KiB/s, done.
From https://github.com/WDzizon/lod-server-support-lod-only
 * branch                feat/lod-only-preservation-1.21.1 -> FETCH_HEAD
   a112ce856..c8adcf352  feat/lod-only-preservation-1.21.1 -> origin/feat/lod-only-preservation-1.21.1
Updating a112ce856..c8adcf352
Fast-forward
 docs/planning/lod-only-preservation-plan.md                                   |  58 +++++++++++++++++++++++++++++
 neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java | 261 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++------------------------------------
 2 files changed, 246 insertions(+), 73 deletions(-)
│█████··│█████··│█████··│█████··│█████··│█████··
> Configure project :fabric             > :fabric > :fabric > :fabric
Fabric Loom: 1.17.13
│██████│████│█
> Configure project :sponge
SpongePowered Plugin 'GRADLE' Toolset Version '2.3.0'
Targeting Minecraft '1.21.1' on a 'SERVER' platform
│██·····│█████▎·│█████▋·│█████│███│███
> Task :neoforge:compileGametestJava FAILED:neoforge:compileGametestJava
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:284: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
            var firstPlayer = helper.makeMockServerPlayerInLevel();
                                    ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:305: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
            var secondPlayer = helper.makeMockServerPlayerInLevel();
                                     ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:422: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
        var player = helper.makeMockServerPlayerInLevel();
                           ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:438: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
        var player = helper.makeMockServerPlayerInLevel();
                           ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:455: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
        var player = helper.makeMockServerPlayerInLevel();
                           ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:2185: error: incompatible types: possible lossy conversion from long to int
                    removalStartedAtTick.compareAndSet(-1, helper.getTick());
                                                                         ^
/home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:2199: error: incompatible types: possible lossy conversion from long to int
            int elapsedSinceRemovalStart = helper.getTick() - removalStartedAtTick.get();
                                                            ^
Note: Some messages have been simplified; recompile with -Xdiags:verbose to get full output
2 errors
5 warnings

[Incubating] Problems report is available at: file:///home/wdzizon/lod-server-support-lod-only/build/reports/problems/problems-report.html

FAILURE: Build failed with an exception.

* What went wrong:
Execution failed for task ':neoforge:compileGametestJava' (registered by plugin class 'org.gradle.api.plugins.JavaBasePlugin').
> Compilation failed; see the compiler output below.
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:2185: error: incompatible types: possible lossy conversion from long to int
                      removalStartedAtTick.compareAndSet(-1, helper.getTick());
                                                                           ^
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:2199: error: incompatible types: possible lossy conversion from long to int
              int elapsedSinceRemovalStart = helper.getTick() - removalStartedAtTick.get();
                                                              ^
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:284: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
              var firstPlayer = helper.makeMockServerPlayerInLevel();
                                      ^
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:305: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
              var secondPlayer = helper.makeMockServerPlayerInLevel();
                                       ^
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:422: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
          var player = helper.makeMockServerPlayerInLevel();
                             ^
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:438: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
          var player = helper.makeMockServerPlayerInLevel();
                             ^
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java:455: warning: [removal] makeMockServerPlayerInLevel() in GameTestHelper has been deprecated and marked for removal
          var player = helper.makeMockServerPlayerInLevel();
                             ^
  Note: Some messages have been simplified; recompile with -Xdiags:verbose to get full output
  2 errors
  5 warnings

* Try:
> Check your code and dependencies to fix the compilation error(s)
> Run with --scan to get full insights from a Build Scan (powered by Develocity).

BUILD FAILED in 4s
19 actionable tasks: 1 executed, 18 up-to-date
