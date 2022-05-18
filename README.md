# dotnet-run-platforms-bug
Demonstrates a bug in dotnet run's cli


The 'main' branch is just an unmodified VS2022 C# Console App from the template, targetting dotnet 6.

The 'x64-added-AnyCPU-removed' branch adds x64 and removes AnyCPU, and reproduces the bug.

The 'hackfixed-x64-added-AnyCPU-removed' branch shows that adding <Platform> alongside <Platforms> works around the problem.  I suspect the functionality of this workaround will make the nature of the problem clearer for those trying to fix it.
