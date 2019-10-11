---
title: 'C# WriteLine()'
date: 2019-10-11 13:24:59
tags: C#
---

There are two ways to call `WriteLine()` function in C#.

First solution:
```
using System;

Consolel.WriteLine("XXXXXX");
```

Second solution:
```
using static System.Console;

WriteLine("XXXXXX");
```

In the second solution, we need to add `static` in the using directive statement. The reason is `Console` is a static class inside of `System` namespace.

More Info: [using static](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/using-static)
