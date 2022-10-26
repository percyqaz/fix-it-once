Getting the actual path of the source code for the calling file -- For weird meta tools

```fsharp
// F#
open System.Runtime.CompilerServices
open System.Runtime.InteropServices

type PathHelper() =
    static member Path( [<CallerFilePath; Optional; DefaultParameterValue("")>] path: string ) : string =
        ...
```

```csharp
// C#
using System.Runtime.CompilerServices;

static member Path([CallerFilePath] path = "")
{
   ...
}
```
