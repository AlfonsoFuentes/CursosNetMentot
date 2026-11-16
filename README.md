# CursosNetMentot

Workspace for .NET course work (NetMentor courses). The repository holds a single
Visual Studio solution, and course projects get added to it over time.

## Status

The solution (`CursosNetMentot.slnx`) is empty for now. No projects have been added yet.

## Requirements

- [.NET SDK](https://dotnet.microsoft.com/download) 9.0.200 or later. The solution
  uses the newer XML-based `.slnx` format, which older SDKs can't read.
- Optional: Visual Studio 2022 17.13+, JetBrains Rider, or VS Code with C# Dev Kit.

## Getting started

```bash
git clone https://github.com/AlfonsoFuentes/CursosNetMentot.git
cd CursosNetMentot
dotnet build CursosNetMentot.slnx
```

## Adding a project

Create a project and register it in the solution:

```bash
dotnet new console -o src/MyProject
dotnet sln CursosNetMentot.slnx add src/MyProject/MyProject.csproj
```

## Repository layout

| Path | Purpose |
| --- | --- |
| `CursosNetMentot.slnx` | Solution file |
| `.gitignore` | Standard Visual Studio / .NET ignore rules |
| `.gitattributes` | Line-ending and diff settings |
