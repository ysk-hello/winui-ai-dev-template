# Project rules

This repository builds a **WinUI 3** desktop app (Windows App SDK, C# / .NET) with an
AI coding agent. Follow these rules in every session.

## Workflow

- **One Issue = one branch = one PR.** Keep each task small — about half a day of work.
- **Never commit directly to `main`.** All changes go through a Pull Request.
- **Never say "done" until it builds.** `dotnet build` and `dotnet test` must pass locally first.
- Leave PRs as **Draft** and let the human review and merge (squash) manually.

## WinUI

- Target **WinUI 3 / Windows App SDK**. Do **not** use WPF, UWP, or WinForms APIs.
- Use `ThemeResource` for colors so the UI stays readable in Light and Dark themes.
- Once the app is scaffolded, build and run it with `.\BuildAndRun.ps1`.
- Prefer MVVM with `CommunityToolkit.Mvvm` (`[ObservableProperty]`, `[RelayCommand]`).

## Style

- Write code comments and identifiers in **English**.
- Describe *what* should work; let the agent choose *how* unless a method truly matters.
