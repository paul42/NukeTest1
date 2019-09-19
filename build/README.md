Setup process:
using visual studio 2019:
* make new solution blank
* add new project (I chose .net core console app)
* using nuke global tool, run 'nuke :setup' in directory like this:
```
PS C:\Users\paul42\source\repos\NukeTest1> nuke :setup
Could not find root directory. Falling back to working directory.
How should the build project be named?
¬  _build
Where should the build project be located?
¬  ./build
Which NUKE version should be used?
¬  0.22.0 (latest release)
Which solution should be the default?
¬  NukeTest1.sln
Do you need help getting started with a basic build?
¬  Yes, get me started!
Restore, compile, pack using ...
¬  dotnet CLI
Source files are located in ...
¬  Neither
Move packages to ...
¬  Neither
Where do test projects go?
¬  Same as source
Do you use git?
¬  Yes, just not setup yet
Do you use GitVersion?
¬  No, custom versioning
Creating directory 'C:\Users\paul42\source\repos\NukeTest1\.\build'...
PS C:\Users\paul42\source\repos\NukeTest1> dotnet --info
.NET Core SDK (reflecting any global.json):
 Version:   2.2.402
 Commit:    c7f2f96116

Runtime Environment:
 OS Name:     Windows
 OS Version:  10.0.16299
 OS Platform: Windows
 RID:         win10-x64
 Base Path:   C:\Program Files\dotnet\sdk\2.2.402\

Host (useful for support):
  Version: 2.2.7
  Commit:  b1e29ae826

.NET Core SDKs installed:
  2.1.202 [C:\Program Files\dotnet\sdk]
  2.1.402 [C:\Program Files\dotnet\sdk]
  2.1.500 [C:\Program Files\dotnet\sdk]
  2.1.802 [C:\Program Files\dotnet\sdk]
  2.2.402 [C:\Program Files\dotnet\sdk]

.NET Core runtimes installed:
  Microsoft.AspNetCore.All 2.1.4 [C:\Program Files\dotnet\shared\Microsoft.AspNetCore.All]
  Microsoft.AspNetCore.All 2.1.6 [C:\Program Files\dotnet\shared\Microsoft.AspNetCore.All]
  Microsoft.AspNetCore.All 2.1.13 [C:\Program Files\dotnet\shared\Microsoft.AspNetCore.All]
  Microsoft.AspNetCore.All 2.2.7 [C:\Program Files\dotnet\shared\Microsoft.AspNetCore.All]
  Microsoft.AspNetCore.App 2.1.4 [C:\Program Files\dotnet\shared\Microsoft.AspNetCore.App]
  Microsoft.AspNetCore.App 2.1.6 [C:\Program Files\dotnet\shared\Microsoft.AspNetCore.App]
  Microsoft.AspNetCore.App 2.1.13 [C:\Program Files\dotnet\shared\Microsoft.AspNetCore.App]
  Microsoft.AspNetCore.App 2.2.7 [C:\Program Files\dotnet\shared\Microsoft.AspNetCore.App]
  Microsoft.NETCore.App 2.0.9 [C:\Program Files\dotnet\shared\Microsoft.NETCore.App]
  Microsoft.NETCore.App 2.1.4 [C:\Program Files\dotnet\shared\Microsoft.NETCore.App]
  Microsoft.NETCore.App 2.1.6 [C:\Program Files\dotnet\shared\Microsoft.NETCore.App]
  Microsoft.NETCore.App 2.1.13 [C:\Program Files\dotnet\shared\Microsoft.NETCore.App]
  Microsoft.NETCore.App 2.2.7 [C:\Program Files\dotnet\shared\Microsoft.NETCore.App]

To install additional .NET Core runtimes or SDKs:
  https://aka.ms/dotnet-download
PS C:\Users\paul42\source\repos\NukeTest1>
```

* make a new folder 'specifications'
* make a new json file 'DotNetLambdaTools.json' inside folder
right click on _build in visual studio and click 'build'

Expected: 
DotnetLambdaTools.Generated.cs would be created like previous