wdzizon@DESKTOP-LS6DH9N:~$ jcmd 8184 Thread.print > /tmp/lss-common-test-threads.txt && grep -n -A60 -B3 -E '"main"|Test worker|LodOnlyArchiveStoreTest|LodOnlyArchiveCrashChild|sqlite' /tmp/lss-common-test-threads.txt
11-0x0000736d8058d890, 0x0000736d807bbc90, 0x0000736d807beed0, 0x0000736cf0000fe0
12-}
13-
14:"Test worker" #1 [8187] prio=5 os_prio=0 cpu=1052.25ms elapsed=1847.48s tid=0x0000736d8001b850 nid=8187 waiting for monitor entry  [0x0000736d855fb000]
15-   java.lang.Thread.State: BLOCKED (on object monitor)
16-     at dev.vox.lss.common.lodonly.LodOnlyArchiveStore.statusLine(LodOnlyArchiveStore.java:1534)
17-     - waiting to lock <0x00000000ee937c70> (a java.lang.Object)
18:     at dev.vox.lss.common.lodonly.LodOnlyArchiveStoreTest.sendPermitSerializesOffThreadVisitAndEditPublication(LodOnlyArchiveStoreTest.java:667)
19-     at java.lang.invoke.LambdaForm$DMH/0x0000736d0c154400.invokeVirtual(java.base@21.0.13.1/LambdaForm$DMH)
20-     at java.lang.invoke.LambdaForm$MH/0x0000736d0c0a4800.invoke(java.base@21.0.13.1/LambdaForm$MH)
21-     at java.lang.invoke.Invokers$Holder.invokeExact_MT(java.base@21.0.13.1/Invokers$Holder)
22-     at jdk.internal.reflect.DirectMethodHandleAccessor.invokeImpl(java.base@21.0.13.1/DirectMethodHandleAccessor.java:153)
23-     at jdk.internal.reflect.DirectMethodHandleAccessor.invoke(java.base@21.0.13.1/DirectMethodHandleAccessor.java:103)
24-     at java.lang.reflect.Method.invoke(java.base@21.0.13.1/Method.java:580)
25-     at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:767)
26-     at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60)
27-     at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131)
28-     at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:156)
29-     at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:147)
30-     at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:86)
31-     at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor$$Lambda/0x0000736d0c119a08.apply(Unknown Source)
32-     at org.junit.jupiter.engine.execution.InterceptingExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(InterceptingExecutableInvoker.java:103)
33-     at org.junit.jupiter.engine.execution.InterceptingExecutableInvoker$ReflectiveInterceptorCall$$Lambda/0x0000736d0c119e28.apply(Unknown Source)
34-     at org.junit.jupiter.engine.execution.InterceptingExecutableInvoker.lambda$invoke$0(InterceptingExecutableInvoker.java:93)
35-     at org.junit.jupiter.engine.execution.InterceptingExecutableInvoker$$Lambda/0x0000736d0c14a200.apply(Unknown Source)
36-     at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106)
37-     at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64)
38-     at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45)
39-     at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37)
40-     at org.junit.jupiter.engine.execution.InterceptingExecutableInvoker.invoke(InterceptingExecutableInvoker.java:92)
41-     at org.junit.jupiter.engine.execution.InterceptingExecutableInvoker.invoke(InterceptingExecutableInvoker.java:86)
42-     at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$8(TestMethodTestDescriptor.java:217)
43-     at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor$$Lambda/0x0000736d0c151400.execute(Unknown Source)
44-     at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73)
45-     at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:213)
46-     at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:138)
47-     at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:68)
48-     at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:156)
49-     at org.junit.platform.engine.support.hierarchical.NodeTestTask$$Lambda/0x0000736d0c13c000.execute(Unknown Source)
50-     at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73)
51-     at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:146)
52-     at org.junit.platform.engine.support.hierarchical.NodeTestTask$$Lambda/0x0000736d0c137d18.invoke(Unknown Source)
53-     at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137)
54-     at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:144)
55-     at org.junit.platform.engine.support.hierarchical.NodeTestTask$$Lambda/0x0000736d0c1378f0.execute(Unknown Source)
56-     at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73)
57-     at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:143)
58-     at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:100)
59-     at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService$$Lambda/0x0000736d0c13cb18.accept(Unknown Source)
60-     at java.util.ArrayList.forEach(java.base@21.0.13.1/ArrayList.java:1596)
61-     at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41)
62-     at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:160)
63-     at org.junit.platform.engine.support.hierarchical.NodeTestTask$$Lambda/0x0000736d0c13c000.execute(Unknown Source)
64-     at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73)
65-     at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:146)
66-     at org.junit.platform.engine.support.hierarchical.NodeTestTask$$Lambda/0x0000736d0c137d18.invoke(Unknown Source)
67-     at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137)
68-     at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:144)
69-     at org.junit.platform.engine.support.hierarchical.NodeTestTask$$Lambda/0x0000736d0c1378f0.execute(Unknown Source)
70-     at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73)
71-     at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:143)
72-     at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:100)
73-     at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService$$Lambda/0x0000736d0c13cb18.accept(Unknown Source)
74-     at java.util.ArrayList.forEach(java.base@21.0.13.1/ArrayList.java:1596)
75-     at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41)
76-     at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:160)
77-     at org.junit.platform.engine.support.hierarchical.NodeTestTask$$Lambda/0x0000736d0c13c000.execute(Unknown Source)
78-     at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73)
--
261-    at java.util.concurrent.locks.ReentrantReadWriteLock$WriteLock.lock(java.base@21.0.13.1/ReentrantReadWriteLock.java:959)
262-    at dev.vox.lss.common.lodonly.LodOnlyArchiveStore.markVisited(LodOnlyArchiveStore.java:554)
263-    - locked <0x00000000ee937c70> (a java.lang.Object)
264:    at dev.vox.lss.common.lodonly.LodOnlyArchiveStoreTest.lambda$sendPermitSerializesOffThreadVisitAndEditPublication$14(LodOnlyArchiveStoreTest.java:663)
265:    at dev.vox.lss.common.lodonly.LodOnlyArchiveStoreTest$$Lambda/0x0000736d0c194aa8.call(Unknown Source)
266-    at java.util.concurrent.FutureTask.run(java.base@21.0.13.1/FutureTask.java:317)
267-    at java.util.concurrent.ThreadPoolExecutor.runWorker(java.base@21.0.13.1/ThreadPoolExecutor.java:1144)
268-    at java.util.concurrent.ThreadPoolExecutor$Worker.run(java.base@21.0.13.1/ThreadPoolExecutor.java:642)
269-    at java.lang.Thread.runWith(java.base@21.0.13.1/Thread.java:1596)
270-    at java.lang.Thread.run(java.base@21.0.13.1/Thread.java:1583)
271-
272-"Attach Listener" #37 [8324] daemon prio=9 os_prio=0 cpu=0.66ms elapsed=0.10s tid=0x0000736cf0000fe0 nid=8324 waiting on condition  [0x0000000000000000]
273-   java.lang.Thread.State: RUNNABLE
274-
275-"GC Thread#7" os_prio=0 cpu=3.07ms elapsed=1846.62s tid=0x0000736d0000d500 nid=8221 runnable
276-
277-"GC Thread#6" os_prio=0 cpu=0.79ms elapsed=1846.62s tid=0x0000736d0000c5e0 nid=8220 runnable
278-
279-"GC Thread#5" os_prio=0 cpu=2.59ms elapsed=1846.62s tid=0x0000736d0000b6c0 nid=8219 runnable
280-
281-"GC Thread#4" os_prio=0 cpu=3.62ms elapsed=1846.62s tid=0x0000736d0000a7d0 nid=8218 runnable
282-
283-"GC Thread#3" os_prio=0 cpu=2.77ms elapsed=1846.62s tid=0x0000736d000098e0 nid=8217 runnable
284-
285-"GC Thread#2" os_prio=0 cpu=3.64ms elapsed=1846.62s tid=0x0000736d00008de0 nid=8216 runnable
286-
287-"GC Thread#1" os_prio=0 cpu=3.11ms elapsed=1846.62s tid=0x0000736d000082e0 nid=8215 runnable
288-
289-"VM Thread" os_prio=0 cpu=56.87ms elapsed=1847.44s tid=0x0000736d80188a70 nid=8197 runnable
290-
291-"VM Periodic Task Thread" os_prio=0 cpu=1057.92ms elapsed=1847.44s tid=0x0000736d80176c30 nid=8196 waiting on condition
292-
293-"G1 Service" os_prio=0 cpu=56.84ms elapsed=1847.47s tid=0x0000736d8015df90 nid=8195 runnable
294-
295-"G1 Refine#0" os_prio=0 cpu=0.16ms elapsed=1847.47s tid=0x0000736d8015cfc0 nid=8194 runnable
296-
297-"G1 Conc#0" os_prio=0 cpu=0.11ms elapsed=1847.47s tid=0x0000736d8004f7f0 nid=8193 runnable
298-
299-"G1 Main Marker" os_prio=0 cpu=0.37ms elapsed=1847.47s tid=0x0000736d8004e840 nid=8192 runnable
300-
301-"GC Thread#0" os_prio=0 cpu=4.72ms elapsed=1847.47s tid=0x0000736d80049200 nid=8191 runnable
302-
303-JNI global refs: 15, weak refs: 10
304-
