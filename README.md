PS D:\정승원\게임\마인크래프트\모드\lod-server-support-support-mc1.21.1> .\gradlew :common:test --tests "dev.vox.lss.common.BrandTest" --rerun-tasks --no-parallel                                           

> Configure project :fabric
Fabric Loom: 1.17.13

> Configure project :sponge
SpongePowered Plugin 'GRADLE' Toolset Version '2.3.0'
Targeting Minecraft '1.21.1' on a 'SERVER' platform

> Task :common:compileJava
Note: D:\?뺤듅??寃뚯엫\留덉씤?щ옒?꾪듃\紐⑤뱶\lod-server-support-support-mc1.21.1\common\src\main\java\dev\vox\lss\common\config\LegacySettingsMigration.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
[
> Task :common:compileTestJava
Note: D:\?뺤듅??寃뚯엫\留덉씤?щ옒?꾪듃\紐⑤뱶\lod-server-support-support-mc1.21.1\common\src\test\java\dev\vox\lss\common\wire\IdentityCodecTest.java uses unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
[
> Task :common:test FAILED

[Incubating] Problems report is available at: file:///D:/%EC%A0%95%EC%8A%B9%EC%9B%90/%EA%B2%8C%EC%9E%84/%EB%A7%88%EC%9D%B8%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B8/%EB%AA%A8%EB%93%9C/lod-server-support-support-mc1.21.1/build/reports/problems/problems-report.html

FAILURE: Build failed with an exception.

* What went wrong:
Execution failed for task ':common:test' (registered by plugin 'org.gradle.jvm-test-suite').
> Test process encountered an unexpected problem.
   > Could not execute test class 'dev.vox.lss.common.BrandTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.BrandTest

* Try:
> Check common problems https://docs.gradle.org/9.5.1/userguide/java_testing.html#sec:java_testing_troubleshooting.
> Run with --stacktrace option to get the stack trace.
> Run with --info or --debug option to get more log output.
> Run with --scan to get full insights from a Build Scan (powered by Develocity).
> Get more help at https://help.gradle.org.

Deprecated Gradle features were used in this build, making it incompatible with Gradle 10.

You can use '--warning-mode all' to show the individual deprecation warnings and determine if they come from your own scripts or plugins.

For more on this, please refer to https://docs.gradle.org/9.5.1/userguide/command_line_interface.html#sec:command_line_warnings in the Gradle documentation.

BUILD FAILED in 11s
11 actionable tasks: 11 executed
