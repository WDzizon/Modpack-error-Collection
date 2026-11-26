5404:
2026-11-26 19:29:29
Full thread dump OpenJDK 64-Bit Server VM (21.0.12.1+1-LTS mixed mode, sharing):

Threads class SMR info:
_java_thread_list=0x000001a08ca21c30, length=40, elements={
0x000001a0860044b0, 0x000001a0860052d0, 0x000001a0860092b0, 0x000001a086009f90,
0x000001a086014a10, 0x000001a08601b120, 0x000001a08601d0a0, 0x000001a08601e150,
0x000001a0860189c0, 0x000001a08601b7b0, 0x000001a086c69b40, 0x000001a0887646e0,
0x000001a088762610, 0x000001a088765a90, 0x000001a088768880, 0x000001a0887695a0,
0x000001a0864c83b0, 0x000001a0864c6970, 0x000001a0864c8a40, 0x000001a0864c7000,
0x000001a0864c7690, 0x000001a0864c4f30, 0x000001a0864c9760, 0x000001a0864c7d20,
0x000001a0864c2e60, 0x000001a0864c62e0, 0x000001a0864c4210, 0x000001a0865900b0,
0x000001a08658f390, 0x000001a086592180, 0x000001a08658dfe0, 0x000001a086593bc0,
0x000001a086591af0, 0x000001a08658fa20, 0x000001a086590dd0, 0x000001a086594250,
0x000001a08c80e6d0, 0x000001a0864ca480, 0x000001a08cdaf9c0, 0x000001a08cdacbd0
}

"Reference Handler" #9 [19692] daemon prio=10 os_prio=2 cpu=140.62ms elapsed=12557.73s tid=0x000001a0860044b0 nid=19692 waiting on condition  [0x000000570a5ff000]
   java.lang.Thread.State: RUNNABLE
	at java.lang.ref.Reference.waitForReferencePendingList(java.base@21.0.12.1/Native Method)
	at java.lang.ref.Reference.processPendingReferences(java.base@21.0.12.1/Reference.java:246)
	at java.lang.ref.Reference$ReferenceHandler.run(java.base@21.0.12.1/Reference.java:208)

   Locked ownable synchronizers:
	- None

"Finalizer" #10 [18704] daemon prio=8 os_prio=1 cpu=0.00ms elapsed=12557.73s tid=0x000001a0860052d0 nid=18704 in Object.wait()  [0x000000570a6fe000]
   java.lang.Thread.State: WAITING (on object monitor)
	at java.lang.Object.wait0(java.base@21.0.12.1/Native Method)
	- waiting on <0x00000007ffb81038> (a java.lang.ref.NativeReferenceQueue$Lock)
	at java.lang.Object.wait(java.base@21.0.12.1/Object.java:366)
	at java.lang.Object.wait(java.base@21.0.12.1/Object.java:339)
	at java.lang.ref.NativeReferenceQueue.await(java.base@21.0.12.1/NativeReferenceQueue.java:48)
	at java.lang.ref.ReferenceQueue.remove0(java.base@21.0.12.1/ReferenceQueue.java:158)
	at java.lang.ref.NativeReferenceQueue.remove(java.base@21.0.12.1/NativeReferenceQueue.java:89)
	- locked <0x00000007ffb81038> (a java.lang.ref.NativeReferenceQueue$Lock)
	at java.lang.ref.Finalizer$FinalizerThread.run(java.base@21.0.12.1/Finalizer.java:173)

   Locked ownable synchronizers:
	- None

"Signal Dispatcher" #11 [19824] daemon prio=9 os_prio=2 cpu=0.00ms elapsed=12557.73s tid=0x000001a0860092b0 nid=19824 waiting on condition  [0x0000000000000000]
   java.lang.Thread.State: RUNNABLE

   Locked ownable synchronizers:
	- None

"Attach Listener" #12 [18424] daemon prio=5 os_prio=2 cpu=0.00ms elapsed=12557.73s tid=0x000001a086009f90 nid=18424 waiting on condition  [0x0000000000000000]
   java.lang.Thread.State: RUNNABLE

   Locked ownable synchronizers:
	- None

"Service Thread" #13 [21640] daemon prio=9 os_prio=0 cpu=93.75ms elapsed=12557.73s tid=0x000001a086014a10 nid=21640 runnable  [0x0000000000000000]
   java.lang.Thread.State: RUNNABLE

   Locked ownable synchronizers:
	- None

"Monitor Deflation Thread" #14 [6288] daemon prio=9 os_prio=0 cpu=109.38ms elapsed=12557.73s tid=0x000001a08601b120 nid=6288 runnable  [0x0000000000000000]
   java.lang.Thread.State: RUNNABLE

   Locked ownable synchronizers:
	- None

"C2 CompilerThread0" #15 [19120] daemon prio=9 os_prio=2 cpu=132843.75ms elapsed=12557.73s tid=0x000001a08601d0a0 nid=19120 waiting on condition  [0x0000000000000000]
   java.lang.Thread.State: RUNNABLE
   No compile task

   Locked ownable synchronizers:
	- None

"C1 CompilerThread0" #18 [12368] daemon prio=9 os_prio=2 cpu=13671.88ms elapsed=12557.72s tid=0x000001a08601e150 nid=12368 waiting on condition  [0x0000000000000000]
   java.lang.Thread.State: RUNNABLE
   No compile task

   Locked ownable synchronizers:
	- None

"Common-Cleaner" #19 [18732] daemon prio=8 os_prio=1 cpu=0.00ms elapsed=12557.70s tid=0x000001a0860189c0 nid=18732 waiting on condition  [0x000000570adff000]
   java.lang.Thread.State: TIMED_WAITING (parking)
	at jdk.internal.misc.Unsafe.park(java.base@21.0.12.1/Native Method)
	- parking to wait for  <0x0000000601400078> (a java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject)
	at java.util.concurrent.locks.LockSupport.parkNanos(java.base@21.0.12.1/LockSupport.java:269)
	at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(java.base@21.0.12.1/AbstractQueuedSynchronizer.java:1886)
	at java.lang.ref.ReferenceQueue.await(java.base@21.0.12.1/ReferenceQueue.java:71)
	at java.lang.ref.ReferenceQueue.remove0(java.base@21.0.12.1/ReferenceQueue.java:143)
	at java.lang.ref.ReferenceQueue.remove(java.base@21.0.12.1/ReferenceQueue.java:218)
	at jdk.internal.ref.CleanerImpl.run(java.base@21.0.12.1/CleanerImpl.java:140)
	at java.lang.Thread.runWith(java.base@21.0.12.1/Thread.java:1596)
	at java.lang.Thread.run(java.base@21.0.12.1/Thread.java:1583)
	at jdk.internal.misc.InnocuousThread.run(java.base@21.0.12.1/InnocuousThread.java:186)

   Locked ownable synchronizers:
	- None

"Notification Thread" #20 [3908] daemon prio=9 os_prio=0 cpu=0.00ms elapsed=12557.50s tid=0x000001a08601b7b0 nid=3908 runnable  [0x0000000000000000]
   java.lang.Thread.State: RUNNABLE

   Locked ownable synchronizers:
	- None

"JNA Cleaner" #50 [11056] daemon prio=5 os_prio=0 cpu=0.00ms elapsed=12550.48s tid=0x000001a086c69b40 nid=11056 waiting on condition  [0x000000570cafe000]
   java.lang.Thread.State: TIMED_WAITING (parking)
	at jdk.internal.misc.Unsafe.park(java.base@21.0.12.1/Native Method)
	- parking to wait for  <0x00000007ff42e588> (a java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject)
	at java.util.concurrent.locks.LockSupport.parkNanos(java.base@21.0.12.1/LockSupport.java:269)
	at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(java.base@21.0.12.1/AbstractQueuedSynchronizer.java:1886)
	at java.lang.ref.ReferenceQueue.await(java.base@21.0.12.1/ReferenceQueue.java:71)
	at java.lang.ref.ReferenceQueue.remove0(java.base@21.0.12.1/ReferenceQueue.java:143)
	at java.lang.ref.ReferenceQueue.remove(java.base@21.0.12.1/ReferenceQueue.java:218)
	at com.sun.jna.internal.Cleaner$CleanerThread.run(com.sun.jna@5.14.0/Cleaner.java:154)

   Locked ownable synchronizers:
	- None

"Timer hack thread" #51 [21884] daemon prio=5 os_prio=0 cpu=0.00ms elapsed=12535.35s tid=0x000001a0887646e0 nid=21884 waiting on condition  [0x000000570ceff000]
   java.lang.Thread.State: TIMED_WAITING (sleeping)
	at java.lang.Thread.sleep0(java.base@21.0.12.1/Native Method)
	at java.lang.Thread.sleep(java.base@21.0.12.1/Thread.java:509)
	at net.minecraft.Util$7.run(minecraft@1.21.1/Util.java:759)

   Locked ownable synchronizers:
	- None

"modloading-sync-worker" #54 [17868] daemon prio=5 os_prio=0 cpu=328.12ms elapsed=12534.46s tid=0x000001a088762610 nid=17868 waiting on condition  [0x000000570b9fe000]
   java.lang.Thread.State: WAITING (parking)
	at jdk.internal.misc.Unsafe.park(java.base@21.0.12.1/Native Method)
	- parking to wait for  <0x0000000609569418> (a java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject)
	at java.util.concurrent.locks.LockSupport.park(java.base@21.0.12.1/LockSupport.java:371)
	at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(java.base@21.0.12.1/AbstractQueuedSynchronizer.java:519)
	at java.util.concurrent.ForkJoinPool.unmanagedBlock(java.base@21.0.12.1/ForkJoinPool.java:3780)
	at java.util.concurrent.ForkJoinPool.managedBlock(java.base@21.0.12.1/ForkJoinPool.java:3725)
	at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(java.base@21.0.12.1/AbstractQueuedSynchronizer.java:1746)
	at java.util.concurrent.LinkedBlockingQueue.take(java.base@21.0.12.1/LinkedBlockingQueue.java:435)
	at java.util.concurrent.ThreadPoolExecutor.getTask(java.base@21.0.12.1/ThreadPoolExecutor.java:1070)
	at java.util.concurrent.ThreadPoolExecutor.runWorker(java.base@21.0.12.1/ThreadPoolExecutor.java:1130)
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(java.base@21.0.12.1/ThreadPoolExecutor.java:642)
	at java.lang.Thread.runWith(java.base@21.0.12.1/Thread.java:1596)
	at java.lang.Thread.run(java.base@21.0.12.1/Thread.java:1583)

   Locked ownable synchronizers:
	- None

"FileSystemWatchService" #55 [14148] daemon prio=5 os_prio=0 cpu=0.00ms elapsed=12533.99s tid=0x000001a088765a90 nid=14148 runnable  [0x000000570cfff000]
   java.lang.Thread.State: RUNNABLE
	at sun.nio.fs.WindowsNativeDispatcher.GetQueuedCompletionStatus0(java.base@21.0.12.1/Native Method)
	at sun.nio.fs.WindowsNativeDispatcher.GetQueuedCompletionStatus(java.base@21.0.12.1/WindowsNativeDispatcher.java:1075)
	at sun.nio.fs.WindowsWatchService$Poller.run(java.base@21.0.12.1/WindowsWatchService.java:587)
	at java.lang.Thread.runWith(java.base@21.0.12.1/Thread.java:1596)
	at java.lang.Thread.run(java.base@21.0.12.1/Thread.java:1583)

   Locked ownable synchronizers:
	- None

"config-file-watcher-0-0" #56 [4440] daemon prio=5 os_prio=0 cpu=250.00ms elapsed=12533.99s tid=0x000001a088768880 nid=4440 runnable  [0x000000570d0ff000]
   java.lang.Thread.State: TIMED_WAITING (parking)
	at jdk.internal.misc.Unsafe.park(java.base@21.0.12.1/Native Method)
	- parking to wait for  <0x00000006095a1678> (a java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject)
	at java.util.concurrent.locks.LockSupport.parkNanos(java.base@21.0.12.1/LockSupport.java:269)
	at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(java.base@21.0.12.1/AbstractQueuedSynchronizer.java:1797)
	at java.util.concurrent.LinkedBlockingDeque.pollFirst(java.base@21.0.12.1/LinkedBlockingDeque.java:515)
	at java.util.concurrent.LinkedBlockingDeque.poll(java.base@21.0.12.1/LinkedBlockingDeque.java:677)
	at sun.nio.fs.AbstractWatchService.poll(java.base@21.0.12.1/AbstractWatchService.java:108)
	at com.electronwill.nightconfig.core.file.FileWatcher$FsWatcher.run(com.electronwill.nightconfig.core@3.8.3/FileWatcher.java:531)
	at java.lang.Thread.runWith(java.base@21.0.12.1/Thread.java:1596)
	at java.lang.Thread.run(java.base@21.0.12.1/Thread.java:1583)

   Locked ownable synchronizers:
	- None

"Yggdrasil Key Fetcher" #60 [14536] daemon prio=5 os_prio=0 cpu=312.50ms elapsed=12533.36s tid=0x000001a0887695a0 nid=14536 waiting on condition  [0x000000570d4fe000]
   java.lang.Thread.State: TIMED_WAITING (parking)
	at jdk.internal.misc.Unsafe.park(java.base@21.0.12.1/Native Method)
	- parking to wait for  <0x00000006094f90b0> (a java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject)
	at java.util.concurrent.locks.LockSupport.parkNanos(java.base@21.0.12.1/LockSupport.java:269)
	at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(java.base@21.0.12.1/AbstractQueuedSynchronizer.java:1797)
	at java.util.concurrent.ScheduledThreadPoolExecutor$DelayedWorkQueue.take(java.base@21.0.12.1/ScheduledThreadPoolExecutor.java:1182)
	at java.util.concurrent.ScheduledThreadPoolExecutor$DelayedWorkQueue.take(java.base@21.0.12.1/ScheduledThreadPoolExecutor.java:899)
	at java.util.concurrent.ThreadPoolExecutor.getTask(java.base@21.0.12.1/ThreadPoolExecutor.java:1070)
	at java.util.concurrent.ThreadPoolExecutor.runWorker(java.base@21.0.12.1/ThreadPoolExecutor.java:1130)
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(java.base@21.0.12.1/ThreadPoolExecutor.java:642)
	at java.lang.Thread.runWith(java.base@21.0.12.1/Thread.java:1596)
	at java.lang.Thread.run(java.base@21.0.12.1/Thread.java:1583)

   Locked ownable synchronizers:
	- None

"Java2D Disposer" #75 [13872] daemon prio=10 os_prio=2 cpu=0.00ms elapsed=12528.63s tid=0x000001a0864c83b0 nid=13872 waiting on condition  [0x000000570aeff000]
   java.lang.Thread.State: WAITING (parking)
	at jdk.internal.misc.Unsafe.park(java.base@21.0.12.1/Native Method)
	- parking to wait for  <0x000000060beb7b58> (a java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject)
	at java.util.concurrent.locks.LockSupport.park(java.base@21.0.12.1/LockSupport.java:371)
	at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(java.base@21.0.12.1/AbstractQueuedSynchronizer.java:519)
	at java.util.concurrent.ForkJoinPool.unmanagedBlock(java.base@21.0.12.1/ForkJoinPool.java:3780)
	at java.util.concurrent.ForkJoinPool.managedBlock(java.base@21.0.12.1/ForkJoinPool.java:3725)
	at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(java.base@21.0.12.1/AbstractQueuedSynchronizer.java:1746)
	at java.lang.ref.ReferenceQueue.await(java.base@21.0.12.1/ReferenceQueue.java:67)
	at java.lang.ref.ReferenceQueue.remove0(java.base@21.0.12.1/ReferenceQueue.java:158)
	at java.lang.ref.ReferenceQueue.remove(java.base@21.0.12.1/ReferenceQueue.java:234)
	at sun.java2d.Disposer.run(java.desktop@21.0.12.1/Disposer.java:145)
	at java.lang.Thread.runWith(java.base@21.0.12.1/Thread.java:1596)
	at java.lang.Thread.run(java.base@21.0.12.1/Thread.java:1583)

   Locked ownable synchronizers:
	- None

"AWT-Windows" #77 [1416] daemon prio=6 os_prio=0 cpu=5109.38ms elapsed=12528.63s tid=0x000001a0864c6970 nid=1416 runnable  [0x000000570e0ff000]
   java.lang.Thread.State: RUNNABLE
	at sun.awt.windows.WToolkit.eventLoop(java.desktop@21.0.12.1/Native Method)
	at sun.awt.windows.WToolkit.run(java.desktop@21.0.12.1/WToolkit.java:360)
	at java.lang.Thread.runWith(java.base@21.0.12.1/Thread.java:1596)
	at java.lang.Thread.run(java.base@21.0.12.1/Thread.java:1583)

   Locked ownable synchronizers:
	- None

"AWT-Shutdown" #80 [25336] prio=5 os_prio=0 cpu=0.00ms elapsed=12526.32s tid=0x000001a0864c8a40 nid=25336 in Object.wait()  [0x000000570e3ff000]
   java.lang.Thread.State: WAITING (on object monitor)
	at java.lang.Object.wait0(java.base@21.0.12.1/Native Method)
	- waiting on <0x000000060bf17428> (a java.lang.Object)
	at java.lang.Object.wait(java.base@21.0.12.1/Object.java:366)
	at java.lang.Object.wait(java.base@21.0.12.1/Object.java:339)
	at sun.awt.AWTAutoShutdown.run(java.desktop@21.0.12.1/AWTAutoShutdown.java:291)
	- locked <0x000000060bf17428> (a java.lang.Object)
	at java.lang.Thread.runWith(java.base@21.0.12.1/Thread.java:1596)
	at java.lang.Thread.run(java.base@21.0.12.1/Thread.java:1583)

   Locked ownable synchronizers:
	- None

"AWT-EventQueue-0" #79 [5532] prio=6 os_prio=0 cpu=3859.38ms elapsed=12526.31s tid=0x000001a0864c7000 nid=5532 waiting on condition  [0x000000570e4ff000]
   java.lang.Thread.State: WAITING (parking)
	at jdk.internal.misc.Unsafe.park(java.base@21.0.12.1/Native Method)
	- parking to wait for  <0x000000060bf470a8> (a java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject)
	at java.util.concurrent.locks.LockSupport.park(java.base@21.0.12.1/LockSupport.java:371)
	at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(java.base@21.0.12.1/AbstractQueuedSynchronizer.java:519)
	at java.util.concurrent.ForkJoinPool.unmanagedBlock(java.base@21.0.12.1/ForkJoinPool.java:3780)
	at java.util.concurrent.ForkJoinPool.managedBlock(java.base@21.0.12.1/ForkJoinPool.java:3725)
	at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(java.base@21.0.12.1/AbstractQueuedSynchronizer.java:1746)
	at java.awt.EventQueue.getNextEvent(java.desktop@21.0.12.1/EventQueue.java:565)
	at java.awt.EventDispatchThread.pumpOneEventForFilters(java.desktop@21.0.12.1/EventDispatchThread.java:190)
	at java.awt.EventDispatchThread.pumpEventsForFilter(java.desktop@21.0.12.1/EventDispatchThread.java:124)
	at java.awt.EventDispatchThread.pumpEventsForHierarchy(java.desktop@21.0.12.1/EventDispatchThread.java:113)
	at java.awt.EventDispatchThread.pumpEvents(java.desktop@21.0.12.1/EventDispatchThread.java:109)
	at java.awt.EventDispatchThread.pumpEvents(java.desktop@21.0.12.1/EventDispatchThread.java:101)
	at java.awt.EventDispatchThread.run(java.desktop@21.0.12.1/EventDispatchThread.java:90)

   Locked ownable synchronizers:
	- None

"TimerQueue" #82 [6240] daemon prio=5 os_prio=0 cpu=390.62ms elapsed=12526.28s tid=0x000001a0864c7690 nid=6240 runnable  [0x000000570e5ff000]
   java.lang.Thread.State: TIMED_WAITING (parking)
	at jdk.internal.misc.Unsafe.park(java.base@21.0.12.1/Native Method)
	- parking to wait for  <0x000000060bf76d18> (a java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject)
	at java.util.concurrent.locks.LockSupport.parkNanos(java.base@21.0.12.1/LockSupport.java:269)
	at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.awaitNanos(java.base@21.0.12.1/AbstractQueuedSynchronizer.java:1797)
	at java.util.concurrent.DelayQueue.take(java.base@21.0.12.1/DelayQueue.java:254)
	at javax.swing.TimerQueue.run(java.desktop@21.0.12.1/TimerQueue.java:165)
	at java.lang.Thread.runWith(java.base@21.0.12.1/Thread.java:1596)
	at java.lang.Thread.run(java.base@21.0.12.1/Thread.java:1583)

   Locked ownable synchronizers:
	- <0x0000000615330ed8> (a java.util.concurrent.locks.ReentrantLock$NonfairSync)

"Thread-0" #81 [14900] daemon prio=5 os_prio=0 cpu=46.88ms elapsed=12526.09s tid=0x000001a0864c4f30 nid=14900 waiting on condition  [0x000000570e6fe000]
   java.lang.Thread.State: WAITING (parking)
	at jdk.internal.misc.Unsafe.park(java.base@21.0.12.1/Native Method)
	- parking to wait for  <0x00000007ff45ae48> (a java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject)
	at java.util.concurrent.locks.LockSupport.park(java.base@21.0.12.1/LockSupport.java:371)
	at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(java.base@21.0.12.1/AbstractQueuedSynchronizer.java:519)
	at java.util.concurrent.ForkJoinPool.unmanagedBlock(java.base@21.0.12.1/ForkJoinPool.java:3780)
	at java.util.concurrent.ForkJoinPool.managedBlock(java.base@21.0.12.1/ForkJoinPool.java:3725)
	at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(java.base@21.0.12.1/AbstractQueuedSynchronizer.java:1746)
	at java.util.concurrent.LinkedBlockingQueue.take(java.base@21.0.12.1/LinkedBlockingQueue.java:435)
	at com.mojang.logging.LogQueues.getNextLogEvent(logging@1.2.7/LogQueues.java:41)
	at net.minecraft.server.gui.MinecraftServerGui.lambda$buildChatPanel$1(minecraft@1.21.1/MinecraftServerGui.java:131)
	at net.minecraft.server.gui.MinecraftServerGui$$Lambda/0x000001a042ee1690.run(minecraft@1.21.1/Unknown Source)
	at java.lang.Thread.runWith(java.base@21.0.12.1/Thread.java:1596)
	at java.lang.Thread.run(java.base@21.0.12.1/Thread.java:1583)

   Locked ownable synchronizers:
	- None

"Server thread" #74 [1216] prio=8 os_prio=1 cpu=10587265.62ms elapsed=12526.09s tid=0x000001a0864c9760 nid=1216 runnable  [0x000000570e7fe000]
   java.lang.Thread.State: RUNNABLE
	at java.util.concurrent.ForkJoinTask.compareAndSetForkJoinTaskTag(java.base@21.0.12.1/ForkJoinTask.java:1359)
	at java.util.concurrent.CompletableFuture$UniCompletion.claim(java.base@21.0.12.1/CompletableFuture.java:568)
	at java.util.concurrent.CompletableFuture.uniWhenComplete(java.base@21.0.12.1/CompletableFuture.java:854)
	at java.util.concurrent.CompletableFuture$UniWhenComplete.tryFire(java.base@21.0.12.1/CompletableFuture.java:841)
	at java.util.concurrent.CompletableFuture.postComplete(java.base@21.0.12.1/CompletableFuture.java:510)
	at java.util.concurrent.CompletableFuture.postFire(java.base@21.0.12.1/CompletableFuture.java:614)
	at java.util.concurrent.CompletableFuture$UniRun.tryFire(java.base@21.0.12.1/CompletableFuture.java:795)
	at java.util.concurrent.CompletableFuture$Completion.run(java.base@21.0.12.1/CompletableFuture.java:482)
	at net.minecraft.server.level.ChunkMap.processUnloads(minecraft@1.21.1/ChunkMap.java:492)
	at net.minecraft.server.level.ChunkMap.tick(minecraft@1.21.1/ChunkMap.java:448)
	at net.minecraft.server.level.ServerChunkCache.tick(minecraft@1.21.1/ServerChunkCache.java:326)
	at net.minecraft.server.MinecraftServer.stopServer(minecraft@1.21.1/MinecraftServer.java:616)
	at net.minecraft.server.dedicated.DedicatedServer.stopServer(minecraft@1.21.1/DedicatedServer.java:567)
	at net.minecraft.server.MinecraftServer.runServer(minecraft@1.21.1/MinecraftServer.java:742)
	at net.minecraft.server.MinecraftServer.lambda$spin$2(minecraft@1.21.1/MinecraftServer.java:267)
	at net.minecraft.server.MinecraftServer$$Lambda/0x000001a042ede190.run(minecraft@1.21.1/Unknown Source)
	at java.lang.Thread.runWith(java.base@21.0.12.1/Thread.java:1596)
	at java.lang.Thread.run(java.base@21.0.12.1/Thread.java:1583)

   Locked ownable synchronizers:
	- None

"DestroyJavaVM" #85 [22004] prio=5 os_prio=0 cpu=16421.88ms elapsed=12526.09s tid=0x000001a0864c7d20 nid=22004 waiting on condition  [0x0000000000000000]
   java.lang.Thread.State: RUNNABLE

   Locked ownable synchronizers:
	- None

"Server console handler" #86 [22064] daemon prio=8 os_prio=1 cpu=31.25ms elapsed=12526.09s tid=0x000001a0864c2e60 nid=22064 runnable  [0x000000570e8fe000]
   java.lang.Thread.State: RUNNABLE
	at java.io.FileInputStream.readBytes(java.base@21.0.12.1/Native Method)
	at java.io.FileInputStream.read(java.base@21.0.12.1/FileInputStream.java:287)
	at java.io.BufferedInputStream.read1(java.base@21.0.12.1/BufferedInputStream.java:345)
	at java.io.BufferedInputStream.implRead(java.base@21.0.12.1/BufferedInputStream.java:420)
	at java.io.BufferedInputStream.read(java.base@21.0.12.1/BufferedInputStream.java:399)
	at sun.nio.cs.StreamDecoder.readBytes(java.base@21.0.12.1/StreamDecoder.java:350)
	at sun.nio.cs.StreamDecoder.implRead(java.base@21.0.12.1/StreamDecoder.java:393)
	at sun.nio.cs.StreamDecoder.lockedRead(java.base@21.0.12.1/StreamDecoder.java:217)
	at sun.nio.cs.StreamDecoder.read(java.base@21.0.12.1/StreamDecoder.java:171)
	at java.io.InputStreamReader.read(java.base@21.0.12.1/InputStreamReader.java:188)
	at java.io.BufferedReader.fill(java.base@21.0.12.1/BufferedReader.java:160)
	at java.io.BufferedReader.implReadLine(java.base@21.0.12.1/BufferedReader.java:370)
	at java.io.BufferedReader.readLine(java.base@21.0.12.1/BufferedReader.java:347)
	at java.io.BufferedReader.readLine(java.base@21.0.12.1/BufferedReader.java:436)
	at net.minecraft.server.dedicated.DedicatedServer$1.run(minecraft@1.21.1/DedicatedServer.java:113)

   Locked ownable synchronizers:
	- <0x0000000602e9f578> (a java.util.concurrent.locks.ReentrantLock$NonfairSync)
	- <0x00000006152baeb8> (a java.util.concurrent.locks.ReentrantLock$NonfairSync)
	- <0x00000006152bef10> (a java.util.concurrent.locks.ReentrantLock$NonfairSync)

"D3D Screen Updater" #87 [17812] daemon prio=7 os_prio=1 cpu=1453.12ms elapsed=12526.09s tid=0x000001a0864c62e0 nid=17812 in Object.wait()  [0x000000570e9ff000]
   java.lang.Thread.State: TIMED_WAITING (on object monitor)
	at java.lang.Object.wait0(java.base@21.0.12.1/Native Method)
	- waiting on <no object reference available>
	at java.lang.Object.wait(java.base@21.0.12.1/Object.java:366)
	at sun.java2d.d3d.D3DScreenUpdateManager.run(java.desktop@21.0.12.1/D3DScreenUpdateManager.java:425)
	- locked <0x000000060bf17550> (a java.lang.Object)
	at java.lang.Thread.runWith(java.base@21.0.12.1/Thread.java:1596)
	at java.lang.Thread.run(java.base@21.0.12.1/Thread.java:1583)

   Locked ownable synchronizers:
	- None

"Netty Server IO #0" #88 [27608] daemon prio=8 os_prio=1 cpu=15.62ms elapsed=12525.59s tid=0x000001a0864c4210 nid=27608 runnable  [0x000000570c9fe000]
   java.lang.Thread.State: RUNNABLE
	at sun.nio.ch.WEPoll.wait(java.base@21.0.12.1/Native Method)
	at sun.nio.ch.WEPollSelectorImpl.doSelect(java.base@21.0.12.1/WEPollSelectorImpl.java:114)
	at sun.nio.ch.SelectorImpl.lockAndDoSelect(java.base@21.0.12.1/SelectorImpl.java:130)
	- locked <0x000000060beb7d08> (a io.netty.channel.nio.SelectedSelectionKeySet)
	- locked <0x000000060beb7ca8> (a sun.nio.ch.WEPollSelectorImpl)
	at sun.nio.ch.SelectorImpl.select(java.base@21.0.12.1/SelectorImpl.java:147)
	at io.netty.channel.nio.SelectedSelectionKeySetSelector.select(io.netty.transport@4.1.97.Final/SelectedSelectionKeySetSelector.java:68)
	at io.netty.channel.nio.NioEventLoop.select(io.netty.transport@4.1.97.Final/NioEventLoop.java:879)
	at io.netty.channel.nio.NioEventLoop.run(io.netty.transport@4.1.97.Final/NioEventLoop.java:526)
	at io.netty.util.concurrent.SingleThreadEventExecutor$4.run(io.netty.common@4.1.97.Final/SingleThreadEventExecutor.java:997)
	at io.netty.util.internal.ThreadExecutorMap$2.run(io.netty.common@4.1.97.Final/ThreadExecutorMap.java:74)
	at java.lang.Thread.runWith(java.base@21.0.12.1/Thread.java:1596)
	at java.lang.Thread.run(java.base@21.0.12.1/Thread.java:1583)

   Locked ownable synchronizers:
	- None

"LanServerPinger #1" #94 [13268] daemon prio=8 os_prio=1 cpu=93.75ms elapsed=12520.69s tid=0x000001a0865900b0 nid=13268 sleeping [0x000000570f1ff000]
   java.lang.Thread.State: TIMED_WAITING (sleeping)
	at java.lang.Thread.sleep0(java.base@21.0.12.1/Native Method)
	at java.lang.Thread.sleep(java.base@21.0.12.1/Thread.java:509)
	at net.minecraft.client.server.LanServerPinger.run(minecraft@1.21.1/LanServerPinger.java:52)

   Locked ownable synchronizers:
	- None

"LSS LOD-only Archive SQLite" #95 [15640] daemon prio=2 os_prio=-2 cpu=22390.62ms elapsed=12520.49s tid=0x000001a08658f390 nid=15640 waiting on condition  [0x000000570f2fe000]
   java.lang.Thread.State: WAITING (parking)
	at jdk.internal.misc.Unsafe.park(java.base@21.0.12.1/Native Method)
	- parking to wait for  <0x000000060bfa71c8> (a java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject)
	at java.util.concurrent.locks.LockSupport.park(java.base@21.0.12.1/LockSupport.java:371)
	at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(java.base@21.0.12.1/AbstractQueuedSynchronizer.java:519)
	at java.util.concurrent.ForkJoinPool.unmanagedBlock(java.base@21.0.12.1/ForkJoinPool.java:3780)
	at java.util.concurrent.ForkJoinPool.managedBlock(java.base@21.0.12.1/ForkJoinPool.java:3725)
	at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(java.base@21.0.12.1/AbstractQueuedSynchronizer.java:1746)
	at java.util.concurrent.ArrayBlockingQueue.take(java.base@21.0.12.1/ArrayBlockingQueue.java:420)
	at dev.vox.lss.common.lodonly.LodOnlyArchiveStore.writerLoop(lss@0.23.0/LodOnlyArchiveStore.java:412)
	at dev.vox.lss.common.lodonly.LodOnlyArchiveStore.lambda$new$0(lss@0.23.0/LodOnlyArchiveStore.java:346)
	at dev.vox.lss.common.lodonly.LodOnlyArchiveStore$$Lambda/0x000001a0430d5ab8.run(lss@0.23.0/Unknown Source)
	at java.lang.Thread.runWith(java.base@21.0.12.1/Thread.java:1596)
	at java.lang.Thread.run(java.base@21.0.12.1/Thread.java:1583)

   Locked ownable synchronizers:
	- None

"LSS Processing Thread" #96 [584] daemon prio=4 os_prio=-1 cpu=8265.62ms elapsed=12503.07s tid=0x000001a086592180 nid=584 in Object.wait()  [0x000000570d3ff000]
   java.lang.Thread.State: TIMED_WAITING (on object monitor)
	at java.lang.Object.wait0(java.base@21.0.12.1/Native Method)
	- waiting on <no object reference available>
	at java.lang.Object.wait(java.base@21.0.12.1/Object.java:366)
	at dev.vox.lss.common.processing.OffThreadProcessor.processingLoop(lss@0.23.0/OffThreadProcessor.java:789)
	- locked <0x000000060cae3510> (a java.lang.Object)
	at dev.vox.lss.common.processing.OffThreadProcessor.lambda$new$4(lss@0.23.0/OffThreadProcessor.java:345)
	at dev.vox.lss.common.processing.OffThreadProcessor$$Lambda/0x000001a043119008.run(lss@0.23.0/Unknown Source)
	at java.lang.Thread.runWith(java.base@21.0.12.1/Thread.java:1596)
	at java.lang.Thread.run(java.base@21.0.12.1/Thread.java:1583)

   Locked ownable synchronizers:
	- None

"Netty Server IO #1" #98 [6380] daemon prio=8 os_prio=1 cpu=6718.75ms elapsed=12480.87s tid=0x000001a08658dfe0 nid=6380 runnable  [0x000000570c4fe000]
   java.lang.Thread.State: RUNNABLE
	at sun.nio.ch.WEPoll.wait(java.base@21.0.12.1/Native Method)
	at sun.nio.ch.WEPollSelectorImpl.doSelect(java.base@21.0.12.1/WEPollSelectorImpl.java:114)
	at sun.nio.ch.SelectorImpl.lockAndDoSelect(java.base@21.0.12.1/SelectorImpl.java:130)
	- locked <0x000000060b0f1ad8> (a io.netty.channel.nio.SelectedSelectionKeySet)
	- locked <0x000000060b0f2b00> (a sun.nio.ch.WEPollSelectorImpl)
	at sun.nio.ch.SelectorImpl.select(java.base@21.0.12.1/SelectorImpl.java:147)
	at io.netty.channel.nio.SelectedSelectionKeySetSelector.select(io.netty.transport@4.1.97.Final/SelectedSelectionKeySetSelector.java:68)
	at io.netty.channel.nio.NioEventLoop.select(io.netty.transport@4.1.97.Final/NioEventLoop.java:879)
	at io.netty.channel.nio.NioEventLoop.run(io.netty.transport@4.1.97.Final/NioEventLoop.java:526)
	at io.netty.util.concurrent.SingleThreadEventExecutor$4.run(io.netty.common@4.1.97.Final/SingleThreadEventExecutor.java:997)
	at io.netty.util.internal.ThreadExecutorMap$2.run(io.netty.common@4.1.97.Final/ThreadExecutorMap.java:74)
	at java.lang.Thread.runWith(java.base@21.0.12.1/Thread.java:1596)
	at java.lang.Thread.run(java.base@21.0.12.1/Thread.java:1583)

   Locked ownable synchronizers:
	- None

"LSS Region Summary Sweeper" #97 [16916] daemon prio=1 os_prio=-2 cpu=421.88ms elapsed=12476.43s tid=0x000001a086593bc0 nid=16916 in Object.wait()  [0x000000570f3ff000]
   java.lang.Thread.State: TIMED_WAITING (on object monitor)
	at java.lang.Object.wait0(java.base@21.0.12.1/Native Method)
	- waiting on <no object reference available>
	at java.lang.Object.wait(java.base@21.0.12.1/Object.java:366)
	at dev.vox.lss.common.region.RegionSummaryService.sweeperLoop(lss@0.23.0/RegionSummaryService.java:384)
	- locked <0x00000006053c73b8> (a java.lang.Object)
	at dev.vox.lss.common.region.RegionSummaryService$$Lambda/0x000001a04311b1a0.run(lss@0.23.0/Unknown Source)
	at java.lang.Thread.runWith(java.base@21.0.12.1/Thread.java:1596)
	at java.lang.Thread.run(java.base@21.0.12.1/Thread.java:1583)

   Locked ownable synchronizers:
	- None

"Netty Server IO #2" #102 [3368] daemon prio=8 os_prio=1 cpu=3187.50ms elapsed=12473.26s tid=0x000001a086591af0 nid=3368 runnable  [0x000000570c7fe000]
   java.lang.Thread.State: RUNNABLE
	at sun.nio.ch.WEPoll.wait(java.base@21.0.12.1/Native Method)
	at sun.nio.ch.WEPollSelectorImpl.doSelect(java.base@21.0.12.1/WEPollSelectorImpl.java:114)
	at sun.nio.ch.SelectorImpl.lockAndDoSelect(java.base@21.0.12.1/SelectorImpl.java:130)
	- locked <0x000000060b08e368> (a io.netty.channel.nio.SelectedSelectionKeySet)
	- locked <0x000000060b08f390> (a sun.nio.ch.WEPollSelectorImpl)
	at sun.nio.ch.SelectorImpl.select(java.base@21.0.12.1/SelectorImpl.java:147)
	at io.netty.channel.nio.SelectedSelectionKeySetSelector.select(io.netty.transport@4.1.97.Final/SelectedSelectionKeySetSelector.java:68)
	at io.netty.channel.nio.NioEventLoop.select(io.netty.transport@4.1.97.Final/NioEventLoop.java:879)
	at io.netty.channel.nio.NioEventLoop.run(io.netty.transport@4.1.97.Final/NioEventLoop.java:526)
	at io.netty.util.concurrent.SingleThreadEventExecutor$4.run(io.netty.common@4.1.97.Final/SingleThreadEventExecutor.java:997)
	at io.netty.util.internal.ThreadExecutorMap$2.run(io.netty.common@4.1.97.Final/ThreadExecutorMap.java:74)
	at java.lang.Thread.runWith(java.base@21.0.12.1/Thread.java:1596)
	at java.lang.Thread.run(java.base@21.0.12.1/Thread.java:1583)

   Locked ownable synchronizers:
	- None

"LSS Disk Reader #1" #106 [26344] daemon prio=1 os_prio=-2 cpu=8312.50ms elapsed=12443.26s tid=0x000001a08658fa20 nid=26344 waiting on condition  [0x0000005709afe000]
   java.lang.Thread.State: WAITING (parking)
	at jdk.internal.misc.Unsafe.park(java.base@21.0.12.1/Native Method)
	- parking to wait for  <0x00000006053c6178> (a java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject)
	at java.util.concurrent.locks.LockSupport.park(java.base@21.0.12.1/LockSupport.java:371)
	at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(java.base@21.0.12.1/AbstractQueuedSynchronizer.java:519)
	at java.util.concurrent.ForkJoinPool.unmanagedBlock(java.base@21.0.12.1/ForkJoinPool.java:3780)
	at java.util.concurrent.ForkJoinPool.managedBlock(java.base@21.0.12.1/ForkJoinPool.java:3725)
	at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(java.base@21.0.12.1/AbstractQueuedSynchronizer.java:1746)
	at java.util.concurrent.ArrayBlockingQueue.take(java.base@21.0.12.1/ArrayBlockingQueue.java:420)
	at java.util.concurrent.ThreadPoolExecutor.getTask(java.base@21.0.12.1/ThreadPoolExecutor.java:1070)
	at java.util.concurrent.ThreadPoolExecutor.runWorker(java.base@21.0.12.1/ThreadPoolExecutor.java:1130)
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(java.base@21.0.12.1/ThreadPoolExecutor.java:642)
	at java.lang.Thread.runWith(java.base@21.0.12.1/Thread.java:1596)
	at java.lang.Thread.run(java.base@21.0.12.1/Thread.java:1583)

   Locked ownable synchronizers:
	- None

"LSS Disk Reader #2" #107 [24368] daemon prio=1 os_prio=-2 cpu=8640.62ms elapsed=12443.26s tid=0x000001a086590dd0 nid=24368 waiting on condition  [0x0000005709bff000]
   java.lang.Thread.State: WAITING (parking)
	at jdk.internal.misc.Unsafe.park(java.base@21.0.12.1/Native Method)
	- parking to wait for  <0x00000006053c6178> (a java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject)
	at java.util.concurrent.locks.LockSupport.park(java.base@21.0.12.1/LockSupport.java:371)
	at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(java.base@21.0.12.1/AbstractQueuedSynchronizer.java:519)
	at java.util.concurrent.ForkJoinPool.unmanagedBlock(java.base@21.0.12.1/ForkJoinPool.java:3780)
	at java.util.concurrent.ForkJoinPool.managedBlock(java.base@21.0.12.1/ForkJoinPool.java:3725)
	at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(java.base@21.0.12.1/AbstractQueuedSynchronizer.java:1746)
	at java.util.concurrent.ArrayBlockingQueue.take(java.base@21.0.12.1/ArrayBlockingQueue.java:420)
	at java.util.concurrent.ThreadPoolExecutor.getTask(java.base@21.0.12.1/ThreadPoolExecutor.java:1070)
	at java.util.concurrent.ThreadPoolExecutor.runWorker(java.base@21.0.12.1/ThreadPoolExecutor.java:1130)
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(java.base@21.0.12.1/ThreadPoolExecutor.java:642)
	at java.lang.Thread.runWith(java.base@21.0.12.1/Thread.java:1596)
	at java.lang.Thread.run(java.base@21.0.12.1/Thread.java:1583)

   Locked ownable synchronizers:
	- None

"LSS Disk Reader #3" #108 [28360] daemon prio=1 os_prio=-2 cpu=8500.00ms elapsed=12443.26s tid=0x000001a086594250 nid=28360 waiting on condition  [0x0000005709cfe000]
   java.lang.Thread.State: WAITING (parking)
	at jdk.internal.misc.Unsafe.park(java.base@21.0.12.1/Native Method)
	- parking to wait for  <0x00000006053c6178> (a java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject)
	at java.util.concurrent.locks.LockSupport.park(java.base@21.0.12.1/LockSupport.java:371)
	at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(java.base@21.0.12.1/AbstractQueuedSynchronizer.java:519)
	at java.util.concurrent.ForkJoinPool.unmanagedBlock(java.base@21.0.12.1/ForkJoinPool.java:3780)
	at java.util.concurrent.ForkJoinPool.managedBlock(java.base@21.0.12.1/ForkJoinPool.java:3725)
	at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(java.base@21.0.12.1/AbstractQueuedSynchronizer.java:1746)
	at java.util.concurrent.ArrayBlockingQueue.take(java.base@21.0.12.1/ArrayBlockingQueue.java:420)
	at java.util.concurrent.ThreadPoolExecutor.getTask(java.base@21.0.12.1/ThreadPoolExecutor.java:1070)
	at java.util.concurrent.ThreadPoolExecutor.runWorker(java.base@21.0.12.1/ThreadPoolExecutor.java:1130)
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(java.base@21.0.12.1/ThreadPoolExecutor.java:642)
	at java.lang.Thread.runWith(java.base@21.0.12.1/Thread.java:1596)
	at java.lang.Thread.run(java.base@21.0.12.1/Thread.java:1583)

   Locked ownable synchronizers:
	- None

"LSS-TimestampSave" #111 [13720] daemon prio=4 os_prio=-1 cpu=1484.38ms elapsed=12420.81s tid=0x000001a08c80e6d0 nid=13720 waiting on condition  [0x000000570c1ff000]
   java.lang.Thread.State: WAITING (parking)
	at jdk.internal.misc.Unsafe.park(java.base@21.0.12.1/Native Method)
	- parking to wait for  <0x000000060cc0c7f8> (a java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject)
	at java.util.concurrent.locks.LockSupport.park(java.base@21.0.12.1/LockSupport.java:371)
	at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(java.base@21.0.12.1/AbstractQueuedSynchronizer.java:519)
	at java.util.concurrent.ForkJoinPool.unmanagedBlock(java.base@21.0.12.1/ForkJoinPool.java:3780)
	at java.util.concurrent.ForkJoinPool.managedBlock(java.base@21.0.12.1/ForkJoinPool.java:3725)
	at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(java.base@21.0.12.1/AbstractQueuedSynchronizer.java:1746)
	at java.util.concurrent.LinkedBlockingQueue.take(java.base@21.0.12.1/LinkedBlockingQueue.java:435)
	at java.util.concurrent.ThreadPoolExecutor.getTask(java.base@21.0.12.1/ThreadPoolExecutor.java:1070)
	at java.util.concurrent.ThreadPoolExecutor.runWorker(java.base@21.0.12.1/ThreadPoolExecutor.java:1130)
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(java.base@21.0.12.1/ThreadPoolExecutor.java:642)
	at java.lang.Thread.runWith(java.base@21.0.12.1/Thread.java:1596)
	at java.lang.Thread.run(java.base@21.0.12.1/Thread.java:1583)

   Locked ownable synchronizers:
	- None

"Netty Server IO #3" #113 [2676] daemon prio=8 os_prio=1 cpu=18703.12ms elapsed=12016.36s tid=0x000001a0864ca480 nid=2676 runnable  [0x000000570bdfe000]
   java.lang.Thread.State: RUNNABLE
	at sun.nio.ch.WEPoll.wait(java.base@21.0.12.1/Native Method)
	at sun.nio.ch.WEPollSelectorImpl.doSelect(java.base@21.0.12.1/WEPollSelectorImpl.java:114)
	at sun.nio.ch.SelectorImpl.lockAndDoSelect(java.base@21.0.12.1/SelectorImpl.java:130)
	- locked <0x000000060b08a530> (a io.netty.channel.nio.SelectedSelectionKeySet)
	- locked <0x000000060b08b558> (a sun.nio.ch.WEPollSelectorImpl)
	at sun.nio.ch.SelectorImpl.select(java.base@21.0.12.1/SelectorImpl.java:147)
	at io.netty.channel.nio.SelectedSelectionKeySetSelector.select(io.netty.transport@4.1.97.Final/SelectedSelectionKeySetSelector.java:68)
	at io.netty.channel.nio.NioEventLoop.select(io.netty.transport@4.1.97.Final/NioEventLoop.java:879)
	at io.netty.channel.nio.NioEventLoop.run(io.netty.transport@4.1.97.Final/NioEventLoop.java:526)
	at io.netty.util.concurrent.SingleThreadEventExecutor$4.run(io.netty.common@4.1.97.Final/SingleThreadEventExecutor.java:997)
	at io.netty.util.internal.ThreadExecutorMap$2.run(io.netty.common@4.1.97.Final/ThreadExecutorMap.java:74)
	at java.lang.Thread.runWith(java.base@21.0.12.1/Thread.java:1596)
	at java.lang.Thread.run(java.base@21.0.12.1/Thread.java:1583)

   Locked ownable synchronizers:
	- None

"Netty Server IO #4" #117 [14976] daemon prio=8 os_prio=1 cpu=17671.88ms elapsed=12013.06s tid=0x000001a08cdaf9c0 nid=14976 runnable  [0x000000570befe000]
   java.lang.Thread.State: RUNNABLE
	at sun.nio.ch.WEPoll.wait(java.base@21.0.12.1/Native Method)
	at sun.nio.ch.WEPollSelectorImpl.doSelect(java.base@21.0.12.1/WEPollSelectorImpl.java:114)
	at sun.nio.ch.SelectorImpl.lockAndDoSelect(java.base@21.0.12.1/SelectorImpl.java:130)
	- locked <0x000000060b0866f8> (a io.netty.channel.nio.SelectedSelectionKeySet)
	- locked <0x000000060b087720> (a sun.nio.ch.WEPollSelectorImpl)
	at sun.nio.ch.SelectorImpl.select(java.base@21.0.12.1/SelectorImpl.java:147)
	at io.netty.channel.nio.SelectedSelectionKeySetSelector.select(io.netty.transport@4.1.97.Final/SelectedSelectionKeySetSelector.java:68)
	at io.netty.channel.nio.NioEventLoop.select(io.netty.transport@4.1.97.Final/NioEventLoop.java:879)
	at io.netty.channel.nio.NioEventLoop.run(io.netty.transport@4.1.97.Final/NioEventLoop.java:526)
	at io.netty.util.concurrent.SingleThreadEventExecutor$4.run(io.netty.common@4.1.97.Final/SingleThreadEventExecutor.java:997)
	at io.netty.util.internal.ThreadExecutorMap$2.run(io.netty.common@4.1.97.Final/ThreadExecutorMap.java:74)
	at java.lang.Thread.runWith(java.base@21.0.12.1/Thread.java:1596)
	at java.lang.Thread.run(java.base@21.0.12.1/Thread.java:1583)

   Locked ownable synchronizers:
	- None

"CompletableFutureDelayScheduler" #120 [20996] daemon prio=8 os_prio=1 cpu=0.00ms elapsed=11997.66s tid=0x000001a08cdacbd0 nid=20996 waiting on condition  [0x000000570c0ff000]
   java.lang.Thread.State: WAITING (parking)
	at jdk.internal.misc.Unsafe.park(java.base@21.0.12.1/Native Method)
	- parking to wait for  <0x000000060e0099f0> (a java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject)
	at java.util.concurrent.locks.LockSupport.park(java.base@21.0.12.1/LockSupport.java:371)
	at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionNode.block(java.base@21.0.12.1/AbstractQueuedSynchronizer.java:519)
	at java.util.concurrent.ForkJoinPool.unmanagedBlock(java.base@21.0.12.1/ForkJoinPool.java:3780)
	at java.util.concurrent.ForkJoinPool.managedBlock(java.base@21.0.12.1/ForkJoinPool.java:3725)
	at java.util.concurrent.locks.AbstractQueuedSynchronizer$ConditionObject.await(java.base@21.0.12.1/AbstractQueuedSynchronizer.java:1746)
	at java.util.concurrent.ScheduledThreadPoolExecutor$DelayedWorkQueue.take(java.base@21.0.12.1/ScheduledThreadPoolExecutor.java:1170)
	at java.util.concurrent.ScheduledThreadPoolExecutor$DelayedWorkQueue.take(java.base@21.0.12.1/ScheduledThreadPoolExecutor.java:899)
	at java.util.concurrent.ThreadPoolExecutor.getTask(java.base@21.0.12.1/ThreadPoolExecutor.java:1070)
	at java.util.concurrent.ThreadPoolExecutor.runWorker(java.base@21.0.12.1/ThreadPoolExecutor.java:1130)
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(java.base@21.0.12.1/ThreadPoolExecutor.java:642)
	at java.lang.Thread.runWith(java.base@21.0.12.1/Thread.java:1596)
	at java.lang.Thread.run(java.base@21.0.12.1/Thread.java:1583)

   Locked ownable synchronizers:
	- None

"G1 Conc#2" os_prio=2 cpu=123687.50ms elapsed=12552.06s tid=0x000001a0872717c0 nid=14104 runnable  

"G1 Conc#1" os_prio=2 cpu=125250.00ms elapsed=12552.06s tid=0x000001a087272a30 nid=17556 runnable  

"GC Thread#9" os_prio=2 cpu=32312.50ms elapsed=12555.33s tid=0x000001a0863b6b70 nid=3400 runnable  

"GC Thread#8" os_prio=2 cpu=31187.50ms elapsed=12555.33s tid=0x000001a0863b67c0 nid=15324 runnable  

"GC Thread#7" os_prio=2 cpu=30906.25ms elapsed=12555.33s tid=0x000001a0864dddf0 nid=3440 runnable  

"GC Thread#6" os_prio=2 cpu=31078.12ms elapsed=12555.33s tid=0x000001a0864dd630 nid=23372 runnable  

"GC Thread#5" os_prio=2 cpu=31421.88ms elapsed=12555.33s tid=0x000001a0864dd280 nid=23964 runnable  

"GC Thread#4" os_prio=2 cpu=32468.75ms elapsed=12555.33s tid=0x000001a0864dced0 nid=17808 runnable  

"GC Thread#3" os_prio=2 cpu=32046.88ms elapsed=12555.33s tid=0x000001a086621990 nid=11672 runnable  

"GC Thread#2" os_prio=2 cpu=31171.88ms elapsed=12555.33s tid=0x000001a0863e8ec0 nid=4492 runnable  

"GC Thread#1" os_prio=2 cpu=30734.38ms elapsed=12555.33s tid=0x000001a0863e8b10 nid=23824 runnable  

"VM Thread" os_prio=2 cpu=7296.88ms elapsed=12557.74s tid=0x000001a040482e50 nid=15648 runnable  

"VM Periodic Task Thread" os_prio=2 cpu=718.75ms elapsed=12557.75s tid=0x000001a040475920 nid=18224 waiting on condition  

"G1 Service" os_prio=2 cpu=812.50ms elapsed=12557.76s tid=0x000001a0403391a0 nid=9568 runnable  

"G1 Refine#0" os_prio=2 cpu=2671.88ms elapsed=12557.76s tid=0x000001a040338620 nid=2152 runnable  

"G1 Conc#0" os_prio=2 cpu=125656.25ms elapsed=12557.76s tid=0x000001a01c500900 nid=23164 runnable  

"G1 Main Marker" os_prio=2 cpu=140.62ms elapsed=12557.76s tid=0x000001a01c4fdc30 nid=21568 runnable  

"GC Thread#0" os_prio=2 cpu=31875.00ms elapsed=12557.76s tid=0x000001a01c4eccc0 nid=7928 runnable  

JNI global refs: 135, weak refs: 224

