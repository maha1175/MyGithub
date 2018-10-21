Sometimes, it is hard to find out why a PowerShell script is not doing what it should do. To get a better understanding of what the code does, use the debugger that is built into the PowerShell ISE.

Before you can debug a script, you need to save it. Untitled scripts are really no scripts, so PowerShell ISE cannot debug them.

Here are the easy steps of debugging a script:

Set breakpoints. Breakpoints are places in your code where you want the debugger to stop, so you can examine current variable states. To set a breakpoint, click into a line, and then press F9. The line turns red. If the line does not turn red, you either did not save the script before, or the line does not contain executable code.
Run script: the script will run as normal, but once it hits a breakpoint line, PowerShell ISE pauses. The current line is marked yellow. You can now hover over variables in your code to see their content, or execute any code in the interactive window, for example dump variable content – or even change it.
Continue: To continue only the next instruction, press F10 or F11. F10 executes the next instruction in the current scope. F11 executes the next instruction, regardless of scope. So if the current line would execute a function, and you press F10, the entire function executes. If you press F11, you will be taken to the first line in that function. It is like a “Micro-Step”.
Press F5 to continue the entire script. It will then run until it is either finished, or the next breakpoint is hit.
Press SHIFT+F5 to abort execution and stop the debugger.
Debugging is really easy once you know these steps. And it can give you a lot of insight and help with otherwise hard to investigate script errors
