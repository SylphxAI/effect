# Repository Agent Instructions

This repository follows the central doctrine in
[SylphxAI/doctrine](https://github.com/SylphxAI/doctrine).

Before changing behavior, read [PROJECT.md](./PROJECT.md) and
[.doctrine/project.json](./.doctrine/project.json). Keep enterprise policy in
doctrine; keep only repo-local package facts here.

Useful validation for package changes:

- `dart format --output=none --set-exit-if-changed .`
- `dart analyze --fatal-infos`
- `dart test`

Do not add consumer-specific application behavior, UI framework assumptions, AI
provider integrations, or customer workflow policy to Effect Dart core.
Consumers should use `package:effect_dart/effect_dart.dart` and documented
examples.
