**Command Format**

procdump.exe -ma -accepteula -c 80 -n 3 -s 30

**Here's the explanation of each option:**

    procdump.exe: This is the command-line executable for Procdump.

    -ma: Specifies that Procdump should create a full memory dump. The -ma option stands for "Mini Plus Full Memory Dump."

    -accepteula: Automatically accepts the End-User License Agreement (EULA) without prompting. This is useful for non-interactive use.

    -c 80: Sets the CPU threshold at 80%. Procdump will create a dump when the CPU usage of the monitored process exceeds 80%.

    -n 3: Specifies that Procdump should create a total of 3 dumps. After creating three dumps, Procdump will exit.

    -s 30: Sets the time interval (in seconds) between each dump creation. In this case, Procdump will wait for 30 seconds between creating each dump.

So, when we run this command, Procdump will monitor the specified process, create a full memory dump when the CPU usage exceeds 80%, repeat this process three times with a 30-second interval between each dump, and then exit.
