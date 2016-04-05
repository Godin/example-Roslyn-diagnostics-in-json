1. add analyzers into project using NuGet, e.g. [SonarAnalyzer.CSharp](https://www.nuget.org/packages/SonarAnalyzer.CSharp)
2. command `msbuild /p:ErrorLog=roslyn-diagnostics.json /t:Rebuild`
will produce [JSON in SARIF format](https://github.com/dotnet/roslyn/blob/master/docs/compilers/Error%20Log%20Format.md),
containing diagnostics from all analyzers
