---
title: Change Build Verbosity In Visual Studio
date: 2019-03-08 11:48:46
tags: Visual Studio
---

When I trying to build my solution, it failed with the following error message:
```
Found conflicts between different versions of the same dependent assembly that could not be resolved.   
These reference conflicts are listed in the build log when log verbosity is set to detailed. 
```
Here is the way to set the log verbosity to `detailed` in visual studio.
1. Go to `Tools`->`Options` menu in VS
2. Open `Projects and Solutions`->`Build and Run`
3. Change the value of the MSBuild project build output verbosity. Pick one from `Quiet`, `Minimal`, `Normal`, `Detailed` and `Diagnostic`

Check the output window(`Ctrl+Alt+O`) in VS to see the changes in the build log.  
In the Build Output, you will see which dependent has the version conflication.  
![detailed build output](\images\2019\03\detailed_build_output.jpg)
