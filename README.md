# JavaPracticeMultithreading
Self-Taught Multithreading courses<br>












<br><B> Explaination of Test.java</B><br>
When a new thread is created, the thread is in the NEW state.<br> When the start() method is called on a thread, the thread scheduler moves it to the Runnable state.<br> Whenever the join() method is called on a thread instance, the current thread executing that statement will wait for this thread to move to the Terminated state.<br> So, before the final statement is printed on the console, the program calls join() on thread2 making the thread1 wait while thread2 completes its execution and is moved to the Terminated state.<br> thread1 goes to the Waiting state because it is waiting for thread2 to complete its execution as it has called join on thread2.
