wdzizon@DESKTOP-LS6DH9N:~/lod-server-support-lod-only$ cd ~/lod-server-support-lod-only &&
> git pull --ff-only origin feat/lod-only-preservation-1.21.1 &&
> ./gradlew :common:test :neoforge:test :neoforge:compileGametestJava :neoforge:runGameTestServer :neoforge:build
remote: Enumerating objects: 68, done.
remote: Counting objects: 100% (68/68), done.
remote: Compressing objects: 100% (37/37), done.
remote: Total 46 (delta 19), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (46/46), 11.33 KiB | 331.00 KiB/s, done.
From https://github.com/WDzizon/lod-server-support-lod-only
 * branch                feat/lod-only-preservation-1.21.1 -> FETCH_HEAD
   537ecde9b..85f43a86f  feat/lod-only-preservation-1.21.1 -> origin/feat/lod-only-preservation-1.21.1
Updating 537ecde9b..85f43a86f
Fast-forward
 docs/planning/lod-only-preservation-plan.md                                                 | 157 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++--
 neoforge/src/gametest/java/dev/vox/lss/neoforge/gametest/LSSNeoGameTests.java               | 144 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 neoforge/src/main/java/dev/vox/lss/networking/server/NeoForgeChunkRecordRemovalAdapter.java | 181 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-----------------------------
 neoforge/src/main/java/dev/vox/lss/networking/server/NeoForgeChunkSideStoreCoordinator.java |  28 ++++++++++++++++++
 4 files changed, 463 insertions(+), 47 deletions(-)
│·······│██▌····│█████··│█████··│█████··│█████··│█████··│█████··
> Configure project :fabric> :common > :fabric > :fabric           > :fabric > :fabric > :fabric
Fabric Loom: 1.17.13
│██████│████│████│█
> Configure project :spongee
SpongePowered Plugin 'GRADLE' Toolset Version '2.3.0'
Targeting Minecraft '1.21.1' on a 'SERVER' platform
│████···│█████▋·│█████▋·│█████▋·│██████·
> Task :neoforge:compileJava FAILEDfor> :neofor> :neoforge:compileJava
/home/wdzizon/lod-server-support-lod-only/neoforge/src/main/java/dev/vox/lss/networking/server/NeoForgeChunkRecordRemovalAdapter.java:172: error: incompatible types: no instance(s) of type variable(s) U exist so that CompletionStage<U> conforms to CompletableFuture<RemovalReceipt>
                    .thenApply(readBack -> {
                              ^
  where U,T are type-variables:
    U extends Object declared in method <U>thenApply(Function<? super T,? extends U>)
    T extends Object declared in interface CompletionStage
1 error

[Incubating] Problems report is available at: file:///home/wdzizon/lod-server-support-lod-only/build/reports/problems/problems-report.html

FAILURE: Build failed with an exception.

* What went wrong:
Execution failed for task ':neoforge:compileJava' (registered by plugin class 'org.gradle.api.plugins.JavaBasePlugin').
> Compilation failed; see the compiler output below.
  /home/wdzizon/lod-server-support-lod-only/neoforge/src/main/java/dev/vox/lss/networking/server/NeoForgeChunkRecordRemovalAdapter.java:172: error: incompatible types: no instance(s) of type variable(s) U exist so that CompletionStage<U> conforms to CompletableFuture<RemovalReceipt>
                      .thenApply(readBack -> {
                                ^
    where U,T are type-variables:
      U extends Object declared in method <U>thenApply(Function<? super T,? extends U>)
      T extends Object declared in interface CompletionStage
  1 error

* Try:
> Check your code and dependencies to fix the compilation error(s)
> Run with --scan to get full insights from a Build Scan (powered by Develocity).

BUILD FAILED in 4s
13 actionable tasks: 1 executed, 12 up-to-date
