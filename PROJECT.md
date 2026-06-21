# Effect Dart

`SylphxAI/effect` provides `effect_dart`, a Dart package for typed effect
values, typed errors, dependency context, runtime execution, concurrency, and
functional data types inspired by Effect-TS.

## Lifecycle

- State: `active`
- Layer: `foundation`
- Machine manifest: [`.doctrine/project.json`](./.doctrine/project.json)

## Goals

- Provide the public `effect_dart` package export for Dart applications and
  libraries.
- Own the `Effect`, `Runtime`, `Context`, `Exit`, `Cause`, `Option`, `Either`,
  random, big-decimal, and array utility semantics implemented under `lib/`.
- Keep examples, tests, README examples, and Dart analysis aligned with the
  package API.

## Non-Goals

- This repo does not own Effect-TS, Dart or Flutter application behavior,
  customer workflows, UI frameworks, or AI provider integrations.
- This repo does not own enterprise doctrine, package registry operations, or
  downstream release policy.

## Boundary

Effect Dart is a tenant-neutral foundation package. Consumers use the
`package:effect_dart/effect_dart.dart` export and documented examples. Product
or application-specific behavior belongs in the consuming product or adapter,
not in this package core.

## Public Surfaces

- Dart package metadata: `pubspec.yaml`
- Package export: `lib/effect_dart.dart`
- Examples: `example/`
- Tests: `test/`
- Documentation: `README.md`, `docs/`, `CHANGELOG.md`

## Delivery

This repo currently has no GitHub Actions workflow. Production proof for package
changes is Dart format, `dart analyze --fatal-infos`, `dart test`, example/API
readback, and package registry readback when published. Published package
regressions are recovered with forward fixes or replacement versions.
