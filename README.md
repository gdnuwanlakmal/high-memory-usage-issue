# High memory usage issue (Conserve Mode)
 FortiGate device is experiencing a high memory usage issue, especially entering Conserve Mode, here are temporary fixes to stabilize the system until a proper root cause can be found:
 
* checks whether the system is in conserve mode, which is triggered when memory usage crosses a critical threshold.

  ```shell
     diagnose hardware sysinfo conserve
  ```
  
* Shows a real-time, per-CPU view of resource usage (CPU and memory) per process

  ```shell
     diagnose sys top-me
  ```
  * Kills a process using its PID (process ID).

    ```shell
    diagnose sys kill 11 xxxx  #  PID (process ID)
    ```
