# Change Log

All notable changes to the "harness-syntax-highlighter" extension will be documented in this file.

## [0.0.6] - 2026-02-14

### Added
- Colorblind-friendly theme for Harness syntax highlighting.

## [0.0.1] - 2025-01-23

### Added
- Initial release of Harness Syntax Highlighter
- Syntax highlighting for Harness pipeline YAML files
- Support for pipeline structure keywords (pipeline, stages, steps, etc.)
- Highlighting for step types (K8sRollingDeploy, ShellScript, Http, etc.)
- Variable expression highlighting (`<+variable.name>`, `<+input>`)
- Support for variable definitions with types (String, Secret, Number)
- Variable highlighting within quoted strings
- Support for complex expressions with .get() method