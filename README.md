> Configure project :fabric
Fabric Loom: 1.17.13

> Configure project :sponge
SpongePowered Plugin 'GRADLE' Toolset Version '2.3.0'
Targeting Minecraft '1.21.1' on a 'SERVER' platform

> Task :paper:compileJava
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.

> Task :common:compileTestJava
Note: D:\?뺤듅??寃뚯엫\留덉씤?щ옒?꾪듃\紐⑤뱶\lod-server-support-support-mc1.21.1\common\src\test\java\dev\vox\lss\common\wire\IdentityCodecTest.java uses unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
[
> Task :neoforge:test FAILED
> Task :common:test FAILED

[Incubating] Problems report is available at: file:///D:/%EC%A0%95%EC%8A%B9%EC%9B%90/%EA%B2%8C%EC%9E%84/%EB%A7%88%EC%9D%B8%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B8/%EB%AA%A8%EB%93%9C/lod-server-support-support-mc1.21.1/build/reports/problems/problems-report.html

FAILURE: Build completed with 2 failures.

1: Task failed with an exception.
-----------
* What went wrong:
Execution failed for task ':neoforge:test' (registered by plugin 'org.gradle.jvm-test-suite').
> Test process encountered an unexpected problem.
   > Could not execute test class 'dev.vox.lss.neoforge.ClassfileSurface$Member'.
      > java.lang.ClassNotFoundException: dev.vox.lss.neoforge.ClassfileSurface$Member
   > Could not execute test class 'dev.vox.lss.neoforge.ClassfileSurface$Surface'.
      > java.lang.ClassNotFoundException: dev.vox.lss.neoforge.ClassfileSurface$Surface
   > Could not execute test class 'dev.vox.lss.neoforge.ClassfileSurface'.
      > java.lang.ClassNotFoundException: dev.vox.lss.neoforge.ClassfileSurface
   > Could not execute test class 'dev.vox.lss.neoforge.LSSNeoPermissionsContractTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.neoforge.LSSNeoPermissionsContractTest
   > Could not execute test class 'dev.vox.lss.neoforge.NeoForgeFarPlaneHookContractTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.neoforge.NeoForgeFarPlaneHookContractTest
   > Could not execute test class 'dev.vox.lss.neoforge.NeoForgeLoaderSeamContractTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.neoforge.NeoForgeLoaderSeamContractTest
   > Could not execute test class 'dev.vox.lss.neoforge.NeoForgeModuleContractTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.neoforge.NeoForgeModuleContractTest
   > Could not execute test class 'dev.vox.lss.neoforge.SodiumConfigApiContractTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.neoforge.SodiumConfigApiContractTest
   > Could not execute test class 'dev.vox.lss.neoforge.SodiumNeoGoldenParityTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.neoforge.SodiumNeoGoldenParityTest

* Try:
> Check common problems https://docs.gradle.org/9.5.1/userguide/java_testing.html#sec:java_testing_troubleshooting.
> Run with --stacktrace option to get the stack trace.
> Run with --info or --debug option to get more log output.
> Run with --scan to get full insights from a Build Scan (powered by Develocity).
> Get more help at https://help.gradle.org.
==============================================================================

2: Task failed with an exception.
-----------
* What went wrong:
Execution failed for task ':common:test' (registered by plugin 'org.gradle.jvm-test-suite').
> Test process encountered an unexpected problem.
   > Could not execute test class 'dev.vox.lss.common.BrandTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.BrandTest
   > Could not execute test class 'dev.vox.lss.common.BuildInfoTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.BuildInfoTest
   > Could not execute test class 'dev.vox.lss.common.ConfigBrandCandidatesTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.ConfigBrandCandidatesTest
   > Could not execute test class 'dev.vox.lss.common.DiagnosticsFormatterTest$StubState'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.DiagnosticsFormatterTest$StubState
   > Could not execute test class 'dev.vox.lss.common.DiagnosticsFormatterTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.DiagnosticsFormatterTest
   > Could not execute test class 'dev.vox.lss.common.ExtraCommandRootGuardTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.ExtraCommandRootGuardTest
   > Could not execute test class 'dev.vox.lss.common.FaultCountersTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.FaultCountersTest
   > Could not execute test class 'dev.vox.lss.common.LogThrottleTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.LogThrottleTest
   > Could not execute test class 'dev.vox.lss.common.MapPolicyGateTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.MapPolicyGateTest
   > Could not execute test class 'dev.vox.lss.common.MinecraftVersionRuleTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.MinecraftVersionRuleTest
   > Could not execute test class 'dev.vox.lss.common.ServiceGateStateTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.ServiceGateStateTest
   > Could not execute test class 'dev.vox.lss.common.SessionOffReasonTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.SessionOffReasonTest
   > Could not execute test class 'dev.vox.lss.common.SharedBandwidthLimiterReconfigureTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.SharedBandwidthLimiterReconfigureTest
   > Could not execute test class 'dev.vox.lss.common.WantSetBudgetInvariantTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.WantSetBudgetInvariantTest
   > Could not execute test class 'dev.vox.lss.common.XrayMaskPolicyTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.XrayMaskPolicyTest
   > Could not execute test class 'dev.vox.lss.common.compat.V16CompatManagerTest$TestState'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.compat.V16CompatManagerTest$TestState
   > Could not execute test class 'dev.vox.lss.common.compat.V16CompatManagerTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.compat.V16CompatManagerTest
   > Could not execute test class 'dev.vox.lss.common.compat.ViaProbeRefusalLineTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.compat.ViaProbeRefusalLineTest
   > Could not execute test class 'dev.vox.lss.common.compat.WireDialectTrackerTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.compat.WireDialectTrackerTest
   > Could not execute test class 'dev.vox.lss.common.config.DhDefaultDowngradeTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.config.DhDefaultDowngradeTest
   > Could not execute test class 'dev.vox.lss.common.config.FarPlaneSettingsTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.config.FarPlaneSettingsTest
   > Could not execute test class 'dev.vox.lss.common.config.FarPlayerHidePermissionSettingsTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.config.FarPlayerHidePermissionSettingsTest
   > Could not execute test class 'dev.vox.lss.common.config.FarPlayerRequiredModeSettingsTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.config.FarPlayerRequiredModeSettingsTest
   > Could not execute test class 'dev.vox.lss.common.config.LegacySettingsMigrationTest$LegacyFields'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.config.LegacySettingsMigrationTest$LegacyFields
   > Could not execute test class 'dev.vox.lss.common.config.LegacySettingsMigrationTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.config.LegacySettingsMigrationTest
   > Could not execute test class 'dev.vox.lss.common.config.LodDistanceOffTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.config.LodDistanceOffTest
   > Could not execute test class 'dev.vox.lss.common.config.MapIngestionSettingsTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.config.MapIngestionSettingsTest
   > Could not execute test class 'dev.vox.lss.common.config.MapPolicySettingsTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.config.MapPolicySettingsTest
   > Could not execute test class 'dev.vox.lss.common.config.SettingMetadataTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.config.SettingMetadataTest
   > Could not execute test class 'dev.vox.lss.common.config.SettingsCliTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.config.SettingsCliTest
   > Could not execute test class 'dev.vox.lss.common.config.SettingsDiagnosticsTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.config.SettingsDiagnosticsTest
   > Could not execute test class 'dev.vox.lss.common.config.SettingsHandleTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.config.SettingsHandleTest
   > Could not execute test class 'dev.vox.lss.common.config.SettingsProblemAnnouncerTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.config.SettingsProblemAnnouncerTest
   > Could not execute test class 'dev.vox.lss.common.config.SettingsProblemStartupTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.config.SettingsProblemStartupTest
   > Could not execute test class 'dev.vox.lss.common.config.SettingsProblemsTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.config.SettingsProblemsTest
   > Could not execute test class 'dev.vox.lss.common.config.SettingsReloadTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.config.SettingsReloadTest
   > Could not execute test class 'dev.vox.lss.common.config.SettingsSidecarStoreTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.config.SettingsSidecarStoreTest
   > Could not execute test class 'dev.vox.lss.common.config.SettingsStoreTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.config.SettingsStoreTest
   > Could not execute test class 'dev.vox.lss.common.config.ShowPermissionRefusalSettingsTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.config.ShowPermissionRefusalSettingsTest
   > Could not execute test class 'dev.vox.lss.common.config.YamlSettingsCodecTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.config.YamlSettingsCodecTest
   > Could not execute test class 'dev.vox.lss.common.dh.DhAssemblyTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.dh.DhAssemblyTest
   > Could not execute test class 'dev.vox.lss.common.dh.DhBandwidthRampTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.dh.DhBandwidthRampTest
   > Could not execute test class 'dev.vox.lss.common.dh.DhCaptureIntegrityTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.dh.DhCaptureIntegrityTest
   > Could not execute test class 'dev.vox.lss.common.dh.DhConnectionStateTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.dh.DhConnectionStateTest
   > Could not execute test class 'dev.vox.lss.common.dh.DhPositionHashTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.dh.DhPositionHashTest
   > Could not execute test class 'dev.vox.lss.common.dh.DhProtocolCodecTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.dh.DhProtocolCodecTest
   > Could not execute test class 'dev.vox.lss.common.dh.DhProtocolDiscoveryTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.dh.DhProtocolDiscoveryTest
   > Could not execute test class 'dev.vox.lss.common.dh.DhReceiptStoreTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.dh.DhReceiptStoreTest
   > Could not execute test class 'dev.vox.lss.common.dh.DhSessionPolicyTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.dh.DhSessionPolicyTest
   > Could not execute test class 'dev.vox.lss.common.dh.DhSkyLightBakeTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.dh.DhSkyLightBakeTest
   > Could not execute test class 'dev.vox.lss.common.dh.DhTerrainDecoderTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.dh.DhTerrainDecoderTest
   > Could not execute test class 'dev.vox.lss.common.dh.DhTerrainFixtures$Body'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.dh.DhTerrainFixtures$Body
   > Could not execute test class 'dev.vox.lss.common.dh.DhTerrainFixtures'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.dh.DhTerrainFixtures
   > Could not execute test class 'dev.vox.lss.common.diagnostics.ClientNoticeBookTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.diagnostics.ClientNoticeBookTest
   > Could not execute test class 'dev.vox.lss.common.diagnostics.ClientNoticePolicyTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.diagnostics.ClientNoticePolicyTest
   > Could not execute test class 'dev.vox.lss.common.diagnostics.ClientReloadTextTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.diagnostics.ClientReloadTextTest
   > Could not execute test class 'dev.vox.lss.common.diagnostics.ClientSettingsStatusTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.diagnostics.ClientSettingsStatusTest
   > Could not execute test class 'dev.vox.lss.common.diagnostics.ClientStatusTextTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.diagnostics.ClientStatusTextTest
   > Could not execute test class 'dev.vox.lss.common.diagnostics.ClientVerdictTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.diagnostics.ClientVerdictTest
   > Could not execute test class 'dev.vox.lss.common.diagnostics.DiagnosticExportTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.diagnostics.DiagnosticExportTest
   > Could not execute test class 'dev.vox.lss.common.diagnostics.DiagnosticPrivacyTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.diagnostics.DiagnosticPrivacyTest
   > Could not execute test class 'dev.vox.lss.common.diagnostics.ScreenEscapeReleaseTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.diagnostics.ScreenEscapeReleaseTest
   > Could not execute test class 'dev.vox.lss.common.diagnostics.ServerExportJobTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.diagnostics.ServerExportJobTest
   > Could not execute test class 'dev.vox.lss.common.diagnostics.ServerStatusSnapshotTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.diagnostics.ServerStatusSnapshotTest
   > Could not execute test class 'dev.vox.lss.common.diagnostics.StatusCacheTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.diagnostics.StatusCacheTest
   > Could not execute test class 'dev.vox.lss.common.diagnostics.StatusStateTest$1Case'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.diagnostics.StatusStateTest$1Case
   > Could not execute test class 'dev.vox.lss.common.diagnostics.StatusStateTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.diagnostics.StatusStateTest
   > Could not execute test class 'dev.vox.lss.common.farplayers.FarPlanePolicyTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.farplayers.FarPlanePolicyTest
   > Could not execute test class 'dev.vox.lss.common.farplayers.FarPlayerBroadcastServiceTest$Sent'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.farplayers.FarPlayerBroadcastServiceTest$Sent
   > Could not execute test class 'dev.vox.lss.common.farplayers.FarPlayerBroadcastServiceTest$Told'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.farplayers.FarPlayerBroadcastServiceTest$Told
   > Could not execute test class 'dev.vox.lss.common.farplayers.FarPlayerBroadcastServiceTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.farplayers.FarPlayerBroadcastServiceTest
   > Could not execute test class 'dev.vox.lss.common.farplayers.FarPlayerChatLineLangTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.farplayers.FarPlayerChatLineLangTest
   > Could not execute test class 'dev.vox.lss.common.farplayers.FarPlayerClientTrackerTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.farplayers.FarPlayerClientTrackerTest
   > Could not execute test class 'dev.vox.lss.common.farplayers.FarPlayerIdentityBindingTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.farplayers.FarPlayerIdentityBindingTest
   > Could not execute test class 'dev.vox.lss.common.farplayers.FarPlayerModeTransitionTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.farplayers.FarPlayerModeTransitionTest
   > Could not execute test class 'dev.vox.lss.common.farplayers.FarPlayerMotionTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.farplayers.FarPlayerMotionTest
   > Could not execute test class 'dev.vox.lss.common.farplayers.FarPlayerWireTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.farplayers.FarPlayerWireTest
   > Could not execute test class 'dev.vox.lss.common.processing.AbstractChunkDiskReaderTest$GateStubStore'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.AbstractChunkDiskReaderTest$GateStubStore
   > Could not execute test class 'dev.vox.lss.common.processing.AbstractChunkDiskReaderTest$TestDiskReader'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.AbstractChunkDiskReaderTest$TestDiskReader
   > Could not execute test class 'dev.vox.lss.common.processing.AbstractChunkDiskReaderTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.AbstractChunkDiskReaderTest
   > Could not execute test class 'dev.vox.lss.common.processing.AdaptiveReadThrottleTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.AdaptiveReadThrottleTest
   > Could not execute test class 'dev.vox.lss.common.processing.BacklogReplaceTest$1StraddleState'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.BacklogReplaceTest$1StraddleState
   > Could not execute test class 'dev.vox.lss.common.processing.BacklogReplaceTest$1WindowState'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.BacklogReplaceTest$1WindowState
   > Could not execute test class 'dev.vox.lss.common.processing.BacklogReplaceTest$TestState'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.BacklogReplaceTest$TestState
   > Could not execute test class 'dev.vox.lss.common.processing.BacklogReplaceTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.BacklogReplaceTest
   > Could not execute test class 'dev.vox.lss.common.processing.ChannelPressureSnapshotTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.ChannelPressureSnapshotTest
   > Could not execute test class 'dev.vox.lss.common.processing.ColumnBytesTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.ColumnBytesTest
   > Could not execute test class 'dev.vox.lss.common.processing.CorrectiveSendAccountingTest$State'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.CorrectiveSendAccountingTest$State
   > Could not execute test class 'dev.vox.lss.common.processing.CorrectiveSendAccountingTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.CorrectiveSendAccountingTest
   > Could not execute test class 'dev.vox.lss.common.processing.DedupFanoutTest$GatedDiskReader'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.DedupFanoutTest$GatedDiskReader
   > Could not execute test class 'dev.vox.lss.common.processing.DedupFanoutTest$Response'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.DedupFanoutTest$Response
   > Could not execute test class 'dev.vox.lss.common.processing.DedupFanoutTest$TestProcessor$Delivery'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.DedupFanoutTest$TestProcessor$Delivery
   > Could not execute test class 'dev.vox.lss.common.processing.DedupFanoutTest$TestProcessor'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.DedupFanoutTest$TestProcessor
   > Could not execute test class 'dev.vox.lss.common.processing.DedupFanoutTest$TestState'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.DedupFanoutTest$TestState
   > Could not execute test class 'dev.vox.lss.common.processing.DedupFanoutTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.DedupFanoutTest
   > Could not execute test class 'dev.vox.lss.common.processing.DiagnosticsCountersTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.DiagnosticsCountersTest
   > Could not execute test class 'dev.vox.lss.common.processing.DirtyEventMailboxTest$StubDiskReader'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.DirtyEventMailboxTest$StubDiskReader
   > Could not execute test class 'dev.vox.lss.common.processing.DirtyEventMailboxTest$TestProcessor'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.DirtyEventMailboxTest$TestProcessor
   > Could not execute test class 'dev.vox.lss.common.processing.DirtyEventMailboxTest$TestState'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.DirtyEventMailboxTest$TestState
   > Could not execute test class 'dev.vox.lss.common.processing.DirtyEventMailboxTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.DirtyEventMailboxTest
   > Could not execute test class 'dev.vox.lss.common.processing.DiskReadDoneSweepTest$StubDiskReader'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.DiskReadDoneSweepTest$StubDiskReader
   > Could not execute test class 'dev.vox.lss.common.processing.DiskReadDoneSweepTest$TestProcessor'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.DiskReadDoneSweepTest$TestProcessor
   > Could not execute test class 'dev.vox.lss.common.processing.DiskReadDoneSweepTest$TestState'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.DiskReadDoneSweepTest$TestState
   > Could not execute test class 'dev.vox.lss.common.processing.DiskReadDoneSweepTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.DiskReadDoneSweepTest
   > Could not execute test class 'dev.vox.lss.common.processing.DiskReadGateTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.DiskReadGateTest
   > Could not execute test class 'dev.vox.lss.common.processing.DiskReaderStoreRungTest$StubStore'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.DiskReaderStoreRungTest$StubStore
   > Could not execute test class 'dev.vox.lss.common.processing.DiskReaderStoreRungTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.DiskReaderStoreRungTest
   > Could not execute test class 'dev.vox.lss.common.processing.FlushSendQueueTest$TestState'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.FlushSendQueueTest$TestState
   > Could not execute test class 'dev.vox.lss.common.processing.FlushSendQueueTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.FlushSendQueueTest
   > Could not execute test class 'dev.vox.lss.common.processing.GateRetentionRoutingTest$StubDiskReader'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.GateRetentionRoutingTest$StubDiskReader
   > Could not execute test class 'dev.vox.lss.common.processing.GateRetentionRoutingTest$TestProcessor'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.GateRetentionRoutingTest$TestProcessor
   > Could not execute test class 'dev.vox.lss.common.processing.GateRetentionRoutingTest$TestState'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.GateRetentionRoutingTest$TestState
   > Could not execute test class 'dev.vox.lss.common.processing.GateRetentionRoutingTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.GateRetentionRoutingTest
   > Could not execute test class 'dev.vox.lss.common.processing.GenerationSessionOwnershipTest$Processor'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.GenerationSessionOwnershipTest$Processor
   > Could not execute test class 'dev.vox.lss.common.processing.GenerationSessionOwnershipTest$Reader'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.GenerationSessionOwnershipTest$Reader
   > Could not execute test class 'dev.vox.lss.common.processing.GenerationSessionOwnershipTest$State'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.GenerationSessionOwnershipTest$State
   > Could not execute test class 'dev.vox.lss.common.processing.GenerationSessionOwnershipTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.GenerationSessionOwnershipTest
   > Could not execute test class 'dev.vox.lss.common.processing.IncomingRequestRouterTest$CapturedPayload'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.IncomingRequestRouterTest$CapturedPayload
   > Could not execute test class 'dev.vox.lss.common.processing.IncomingRequestRouterTest$CapturedSubmit'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.IncomingRequestRouterTest$CapturedSubmit
   > Could not execute test class 'dev.vox.lss.common.processing.IncomingRequestRouterTest$Delivered'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.IncomingRequestRouterTest$Delivered
   > Could not execute test class 'dev.vox.lss.common.processing.IncomingRequestRouterTest$NoHeadroomDiskReader'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.IncomingRequestRouterTest$NoHeadroomDiskReader
   > Could not execute test class 'dev.vox.lss.common.processing.IncomingRequestRouterTest$StubDiskReader'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.IncomingRequestRouterTest$StubDiskReader
   > Could not execute test class 'dev.vox.lss.common.processing.IncomingRequestRouterTest$TestProcessor'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.IncomingRequestRouterTest$TestProcessor
   > Could not execute test class 'dev.vox.lss.common.processing.IncomingRequestRouterTest$TestState'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.IncomingRequestRouterTest$TestState
   > Could not execute test class 'dev.vox.lss.common.processing.IncomingRequestRouterTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.IncomingRequestRouterTest
   > Could not execute test class 'dev.vox.lss.common.processing.LoadedProbeGuardTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.LoadedProbeGuardTest
   > Could not execute test class 'dev.vox.lss.common.processing.OffThreadProcessorDiskResultTest$Response'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.OffThreadProcessorDiskResultTest$Response
   > Could not execute test class 'dev.vox.lss.common.processing.OffThreadProcessorDiskResultTest$Rig'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.OffThreadProcessorDiskResultTest$Rig
   > Could not execute test class 'dev.vox.lss.common.processing.OffThreadProcessorDiskResultTest$StubDiskReader'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.OffThreadProcessorDiskResultTest$StubDiskReader
   > Could not execute test class 'dev.vox.lss.common.processing.OffThreadProcessorDiskResultTest$TestProcessor$DiskSubmit'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.OffThreadProcessorDiskResultTest$TestProcessor$DiskSubmit
   > Could not execute test class 'dev.vox.lss.common.processing.OffThreadProcessorDiskResultTest$TestProcessor$EnqueuedColumn'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.OffThreadProcessorDiskResultTest$TestProcessor$EnqueuedColumn
   > Could not execute test class 'dev.vox.lss.common.processing.OffThreadProcessorDiskResultTest$TestProcessor'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.OffThreadProcessorDiskResultTest$TestProcessor
   > Could not execute test class 'dev.vox.lss.common.processing.OffThreadProcessorDiskResultTest$TestState'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.OffThreadProcessorDiskResultTest$TestState
   > Could not execute test class 'dev.vox.lss.common.processing.OffThreadProcessorDiskResultTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.OffThreadProcessorDiskResultTest
   > Could not execute test class 'dev.vox.lss.common.processing.OffThreadProcessorLifecycleTest$Response'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.OffThreadProcessorLifecycleTest$Response
   > Could not execute test class 'dev.vox.lss.common.processing.OffThreadProcessorLifecycleTest$StubDiskReader'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.OffThreadProcessorLifecycleTest$StubDiskReader
   > Could not execute test class 'dev.vox.lss.common.processing.OffThreadProcessorLifecycleTest$TestProcessor$EnqueuedColumn'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.OffThreadProcessorLifecycleTest$TestProcessor$EnqueuedColumn
   > Could not execute test class 'dev.vox.lss.common.processing.OffThreadProcessorLifecycleTest$TestProcessor'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.OffThreadProcessorLifecycleTest$TestProcessor
   > Could not execute test class 'dev.vox.lss.common.processing.OffThreadProcessorLifecycleTest$TestState'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.OffThreadProcessorLifecycleTest$TestState
   > Could not execute test class 'dev.vox.lss.common.processing.OffThreadProcessorLifecycleTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.OffThreadProcessorLifecycleTest
   > Could not execute test class 'dev.vox.lss.common.processing.OffThreadProcessorMailboxTest$StubDiskReader'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.OffThreadProcessorMailboxTest$StubDiskReader
   > Could not execute test class 'dev.vox.lss.common.processing.OffThreadProcessorMailboxTest$TestProcessor'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.OffThreadProcessorMailboxTest$TestProcessor
   > Could not execute test class 'dev.vox.lss.common.processing.OffThreadProcessorMailboxTest$TestState'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.OffThreadProcessorMailboxTest$TestState
   > Could not execute test class 'dev.vox.lss.common.processing.OffThreadProcessorMailboxTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.OffThreadProcessorMailboxTest
   > Could not execute test class 'dev.vox.lss.common.processing.OffThreadProcessorStoreTest$RecordingStore$Dep'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.OffThreadProcessorStoreTest$RecordingStore$Dep
   > Could not execute test class 'dev.vox.lss.common.processing.OffThreadProcessorStoreTest$RecordingStore'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.OffThreadProcessorStoreTest$RecordingStore
   > Could not execute test class 'dev.vox.lss.common.processing.OffThreadProcessorStoreTest$Rig'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.OffThreadProcessorStoreTest$Rig
   > Could not execute test class 'dev.vox.lss.common.processing.OffThreadProcessorStoreTest$StubDiskReader'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.OffThreadProcessorStoreTest$StubDiskReader
   > Could not execute test class 'dev.vox.lss.common.processing.OffThreadProcessorStoreTest$TestProcessor$EnqueuedColumn'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.OffThreadProcessorStoreTest$TestProcessor$EnqueuedColumn
   > Could not execute test class 'dev.vox.lss.common.processing.OffThreadProcessorStoreTest$TestProcessor'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.OffThreadProcessorStoreTest$TestProcessor
   > Could not execute test class 'dev.vox.lss.common.processing.OffThreadProcessorStoreTest$TestState'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.OffThreadProcessorStoreTest$TestState
   > Could not execute test class 'dev.vox.lss.common.processing.OffThreadProcessorStoreTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.OffThreadProcessorStoreTest
   > Could not execute test class 'dev.vox.lss.common.processing.PairedIngressLifecycleTest$State'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.PairedIngressLifecycleTest$State
   > Could not execute test class 'dev.vox.lss.common.processing.PairedIngressLifecycleTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.PairedIngressLifecycleTest
   > Could not execute test class 'dev.vox.lss.common.processing.PairedProbeRoutingTest$Delivery'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.PairedProbeRoutingTest$Delivery
   > Could not execute test class 'dev.vox.lss.common.processing.PairedProbeRoutingTest$Processor'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.PairedProbeRoutingTest$Processor
   > Could not execute test class 'dev.vox.lss.common.processing.PairedProbeRoutingTest$Reader'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.PairedProbeRoutingTest$Reader
   > Could not execute test class 'dev.vox.lss.common.processing.PairedProbeRoutingTest$Rig'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.PairedProbeRoutingTest$Rig
   > Could not execute test class 'dev.vox.lss.common.processing.PairedProbeRoutingTest$State'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.PairedProbeRoutingTest$State
   > Could not execute test class 'dev.vox.lss.common.processing.PairedProbeRoutingTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.PairedProbeRoutingTest
   > Could not execute test class 'dev.vox.lss.common.processing.PingBackstopTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.PingBackstopTest
   > Could not execute test class 'dev.vox.lss.common.processing.ReadFreshnessRungTest$RecordingStore'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.ReadFreshnessRungTest$RecordingStore
   > Could not execute test class 'dev.vox.lss.common.processing.ReadFreshnessRungTest$Response'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.ReadFreshnessRungTest$Response
   > Could not execute test class 'dev.vox.lss.common.processing.ReadFreshnessRungTest$Rig'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.ReadFreshnessRungTest$Rig
   > Could not execute test class 'dev.vox.lss.common.processing.ReadFreshnessRungTest$StubDiskReader'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.ReadFreshnessRungTest$StubDiskReader
   > Could not execute test class 'dev.vox.lss.common.processing.ReadFreshnessRungTest$TestDiskReader'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.ReadFreshnessRungTest$TestDiskReader
   > Could not execute test class 'dev.vox.lss.common.processing.ReadFreshnessRungTest$TestProcessor$EnqueuedColumn'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.ReadFreshnessRungTest$TestProcessor$EnqueuedColumn
   > Could not execute test class 'dev.vox.lss.common.processing.ReadFreshnessRungTest$TestProcessor'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.ReadFreshnessRungTest$TestProcessor
   > Could not execute test class 'dev.vox.lss.common.processing.ReadFreshnessRungTest$TestState'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.ReadFreshnessRungTest$TestState
   > Could not execute test class 'dev.vox.lss.common.processing.ReadFreshnessRungTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.ReadFreshnessRungTest
   > Could not execute test class 'dev.vox.lss.common.processing.RequestSessionOwnershipTest$1ParkReader'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.RequestSessionOwnershipTest$1ParkReader
   > Could not execute test class 'dev.vox.lss.common.processing.RequestSessionOwnershipTest$1TerminalReader'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.RequestSessionOwnershipTest$1TerminalReader
   > Could not execute test class 'dev.vox.lss.common.processing.RequestSessionOwnershipTest$Processor'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.RequestSessionOwnershipTest$Processor
   > Could not execute test class 'dev.vox.lss.common.processing.RequestSessionOwnershipTest$Reader'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.RequestSessionOwnershipTest$Reader
   > Could not execute test class 'dev.vox.lss.common.processing.RequestSessionOwnershipTest$State'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.RequestSessionOwnershipTest$State
   > Could not execute test class 'dev.vox.lss.common.processing.RequestSessionOwnershipTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.RequestSessionOwnershipTest
   > Could not execute test class 'dev.vox.lss.common.processing.RouteRotationFairnessTest$StubDiskReader'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.RouteRotationFairnessTest$StubDiskReader
   > Could not execute test class 'dev.vox.lss.common.processing.RouteRotationFairnessTest$TestProcessor'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.RouteRotationFairnessTest$TestProcessor
   > Could not execute test class 'dev.vox.lss.common.processing.RouteRotationFairnessTest$TestState'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.RouteRotationFairnessTest$TestState
   > Could not execute test class 'dev.vox.lss.common.processing.RouteRotationFairnessTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.RouteRotationFairnessTest
   > Could not execute test class 'dev.vox.lss.common.processing.SendActionIdentityTest$Delivered'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.SendActionIdentityTest$Delivered
   > Could not execute test class 'dev.vox.lss.common.processing.SendActionIdentityTest$TestProcessor'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.SendActionIdentityTest$TestProcessor
   > Could not execute test class 'dev.vox.lss.common.processing.SendActionIdentityTest$TestState'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.SendActionIdentityTest$TestState
   > Could not execute test class 'dev.vox.lss.common.processing.SendActionIdentityTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.SendActionIdentityTest
   > Could not execute test class 'dev.vox.lss.common.processing.SendPacingFlushTest$TestState'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.SendPacingFlushTest$TestState
   > Could not execute test class 'dev.vox.lss.common.processing.SendPacingFlushTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.SendPacingFlushTest
   > Could not execute test class 'dev.vox.lss.common.processing.SlotAdmissionTest$TestState$NoPayload'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.SlotAdmissionTest$TestState$NoPayload
   > Could not execute test class 'dev.vox.lss.common.processing.SlotAdmissionTest$TestState'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.SlotAdmissionTest$TestState
   > Could not execute test class 'dev.vox.lss.common.processing.SlotAdmissionTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.SlotAdmissionTest
   > Could not execute test class 'dev.vox.lss.common.processing.StoreFrameDeliveryTest$RecordingStore$Dep'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.StoreFrameDeliveryTest$RecordingStore$Dep
   > Could not execute test class 'dev.vox.lss.common.processing.StoreFrameDeliveryTest$RecordingStore$FrameDep'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.StoreFrameDeliveryTest$RecordingStore$FrameDep
   > Could not execute test class 'dev.vox.lss.common.processing.StoreFrameDeliveryTest$RecordingStore'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.StoreFrameDeliveryTest$RecordingStore
   > Could not execute test class 'dev.vox.lss.common.processing.StoreFrameDeliveryTest$Rig'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.StoreFrameDeliveryTest$Rig
   > Could not execute test class 'dev.vox.lss.common.processing.StoreFrameDeliveryTest$TestProcessor$Built'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.StoreFrameDeliveryTest$TestProcessor$Built
   > Could not execute test class 'dev.vox.lss.common.processing.StoreFrameDeliveryTest$TestProcessor'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.StoreFrameDeliveryTest$TestProcessor
   > Could not execute test class 'dev.vox.lss.common.processing.StoreFrameDeliveryTest$TestState'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.StoreFrameDeliveryTest$TestState
   > Could not execute test class 'dev.vox.lss.common.processing.StoreFrameDeliveryTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.StoreFrameDeliveryTest
   > Could not execute test class 'dev.vox.lss.common.processing.StoreFrameServingRungTest$StubStore'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.StoreFrameServingRungTest$StubStore
   > Could not execute test class 'dev.vox.lss.common.processing.StoreFrameServingRungTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.StoreFrameServingRungTest
   > Could not execute test class 'dev.vox.lss.common.processing.TickDiagnosticsTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.TickDiagnosticsTest
   > Could not execute test class 'dev.vox.lss.common.processing.TimestampSaveSchedulerTest$RecordingExecutor'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.TimestampSaveSchedulerTest$RecordingExecutor
   > Could not execute test class 'dev.vox.lss.common.processing.TimestampSaveSchedulerTest$StubDiskReader'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.TimestampSaveSchedulerTest$StubDiskReader
   > Could not execute test class 'dev.vox.lss.common.processing.TimestampSaveSchedulerTest$TestProcessor'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.TimestampSaveSchedulerTest$TestProcessor
   > Could not execute test class 'dev.vox.lss.common.processing.TimestampSaveSchedulerTest$TestState'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.TimestampSaveSchedulerTest$TestState
   > Could not execute test class 'dev.vox.lss.common.processing.TimestampSaveSchedulerTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.TimestampSaveSchedulerTest
   > Could not execute test class 'dev.vox.lss.common.processing.TransportYieldFlushTest$TestState'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.TransportYieldFlushTest$TestState
   > Could not execute test class 'dev.vox.lss.common.processing.TransportYieldFlushTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.processing.TransportYieldFlushTest
   > Could not execute test class 'dev.vox.lss.common.region.ColumnStampsWireTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.region.ColumnStampsWireTest
   > Could not execute test class 'dev.vox.lss.common.region.RegionStampTableTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.region.RegionStampTableTest
   > Could not execute test class 'dev.vox.lss.common.region.RegionSummaryDiagnosticsTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.region.RegionSummaryDiagnosticsTest
   > Could not execute test class 'dev.vox.lss.common.region.RegionSummaryServiceTest$GatedSource'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.region.RegionSummaryServiceTest$GatedSource
   > Could not execute test class 'dev.vox.lss.common.region.RegionSummaryServiceTest$Rig'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.region.RegionSummaryServiceTest$Rig
   > Could not execute test class 'dev.vox.lss.common.region.RegionSummaryServiceTest$Sent'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.region.RegionSummaryServiceTest$Sent
   > Could not execute test class 'dev.vox.lss.common.region.RegionSummaryServiceTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.region.RegionSummaryServiceTest
   > Could not execute test class 'dev.vox.lss.common.region.RegionSummaryWireTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.region.RegionSummaryWireTest
   > Could not execute test class 'dev.vox.lss.common.store.LodStoreModeTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.store.LodStoreModeTest
   > Could not execute test class 'dev.vox.lss.common.store.LodStoresAdviceTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.store.LodStoresAdviceTest
   > Could not execute test class 'dev.vox.lss.common.store.RegistryFingerprintTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.store.RegistryFingerprintTest
   > Could not execute test class 'dev.vox.lss.common.store.SqliteFrameServingTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.store.SqliteFrameServingTest
   > Could not execute test class 'dev.vox.lss.common.store.SqliteIsolationTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.store.SqliteIsolationTest
   > Could not execute test class 'dev.vox.lss.common.store.SqliteLodStoreMaskShutdownTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.store.SqliteLodStoreMaskShutdownTest
   > Could not execute test class 'dev.vox.lss.common.store.SqliteLodStoreMigrationTest$FixtureRow'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.store.SqliteLodStoreMigrationTest$FixtureRow
   > Could not execute test class 'dev.vox.lss.common.store.SqliteLodStoreMigrationTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.store.SqliteLodStoreMigrationTest
   > Could not execute test class 'dev.vox.lss.common.store.SqliteLodStoreTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.store.SqliteLodStoreTest
   > Could not execute test class 'dev.vox.lss.common.store.SqliteOwnershipTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.store.SqliteOwnershipTest
   > Could not execute test class 'dev.vox.lss.common.store.SqliteRuntimeProbe'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.store.SqliteRuntimeProbe
   > Could not execute test class 'dev.vox.lss.common.store.StoreBackfillTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.store.StoreBackfillTest
   > Could not execute test class 'dev.vox.lss.common.store.StorePolicyReloadTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.store.StorePolicyReloadTest
   > Could not execute test class 'dev.vox.lss.common.voxel.ColumnTimestampPolicyTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.voxel.ColumnTimestampPolicyTest
   > Could not execute test class 'dev.vox.lss.common.voxel.SkyLightEstimateTest$Grid'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.voxel.SkyLightEstimateTest$Grid
   > Could not execute test class 'dev.vox.lss.common.voxel.SkyLightEstimateTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.voxel.SkyLightEstimateTest
   > Could not execute test class 'dev.vox.lss.common.wire.CrossRegistrySimulationTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.wire.CrossRegistrySimulationTest
   > Could not execute test class 'dev.vox.lss.common.wire.IdentityCodecTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.wire.IdentityCodecTest
   > Could not execute test class 'dev.vox.lss.common.wire.NativeSectionShapeTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.wire.NativeSectionShapeTest
   > Could not execute test class 'dev.vox.lss.common.wire.NativeToV20TranslatorTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.wire.NativeToV20TranslatorTest
   > Could not execute test class 'dev.vox.lss.common.wire.WireSectionCursorCorpusTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.wire.WireSectionCursorCorpusTest
   > Could not execute test class 'dev.vox.lss.common.wire.WireSectionCursorTest'.
      > java.lang.ClassNotFoundException: dev.vox.lss.common.wire.WireSectionCursorTest

* Try:
> Check common problems https://docs.gradle.org/9.5.1/userguide/java_testing.html#sec:java_testing_troubleshooting.
> Run with --stacktrace option to get the stack trace.
> Run with --info or --debug option to get more log output.
> Run with --scan to get full insights from a Build Scan (powered by Develocity).
> Get more help at https://help.gradle.org.
==============================================================================

Deprecated Gradle features were used in this build, making it incompatible with Gradle 10.

You can use '--warning-mode all' to show the individual deprecation warnings and determine if they come from your own scripts or plugins.

For more on this, please refer to https://docs.gradle.org/9.5.1/userguide/command_line_interface.html#sec:command_line_warnings in the Gradle documentation.

BUILD FAILED in 29s
37 actionable tasks: 25 executed, 12 up-to-date
