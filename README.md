# Harness Syntax Highlighter

A Visual Studio Code extension that provides comprehensive syntax highlighting for Harness CI/CD pipeline YAML files.

## Features

This extension enhances your Harness pipeline development experience by providing:

### Pipeline Structure Highlighting
- **Pipeline Keywords**: `pipeline`, `stages`, `steps`, `stepGroup`, `execution`, `rollbackSteps`
- **Common Properties**: `name`, `identifier`, `type`, `spec`, `timeout`, `when`, `condition`
- **Template Support**: `template`, `templateRef`, `versionLabel`, `templateInputs`

### Step Type Recognition
- **Deployment Steps**: `K8sRollingDeploy`, `K8sApply`, `K8sDryRun`, `K8sRollingRollback`
- **Utility Steps**: `ShellScript`, `Http`, `HarnessApproval`
- **Integration Steps**: `JiraCreate`, `JiraUpdate`
- **Deployment Types**: `Kubernetes`, `Rolling`, `Canary`, `BlueGreen`

### Variable Support
- **Harness Expressions**: `<+variable.account.name>`, `<+pipeline.variables.var>`
- **Complex Expressions**: `<+pipeline.variables.get("var-name")>` (for variables with hyphens/periods)
- **Runtime Inputs**: `<+input>`
- **Variables in Strings**: Highlights Harness expressions even when embedded in quoted strings

### Variable Definitions
- **Variable Blocks**: Proper highlighting for `variables:` sections
- **Variable Properties**: `name`, `type`, `description`, `required`, `value`
- **Variable Types**: `Secret`, `String`, `Number`
- **Boolean Values**: `true`, `false`

## Installation

1. Open VS Code
2. Go to Extensions (Ctrl+Shift+X)
3. Search for "Harness Syntax Highlighter"
4. Click Install

## Usage

The extension automatically activates when you open `.yml` or `.yaml` files. For best results with Harness pipeline files:

1. Ensure your Harness pipeline files have `.yml` or `.yaml` extensions
2. The syntax highlighting will automatically apply to recognize Harness-specific syntax
3. Variables and expressions will be highlighted with distinct colors based on your VS Code theme

## Example

```yaml
pipeline:
  name: Sample Pipeline
  identifier: sample_pipeline
  stages:
    - stage:
        name: Deploy Stage
        identifier: deploy
        type: Deployment
        spec:
          services:
            values: <+input>
          environments:
            values: <+input>
          execution:
            steps:
              - step:
                  type: ShellScript
                  name: Deploy Script
                  identifier: deploy_script
                  spec:
                    shell: Bash
                    source:
                      type: Inline
                      spec:
                        script: |
                          echo "Deploying <+service.name> to <+env.name>"
variables:
  - name: deploymentType
    type: String
    description: Type of deployment
    required: true
    value: <+input>
```

## Requirements

- VS Code 1.102.0 or higher
- No additional dependencies required

## Extension Settings

This extension does not add any VS Code settings.

## Known Issues

- Currently supports YAML files with `.yml` and `.yaml` extensions
- Complex nested expressions may require specific formatting for optimal highlighting

## Contributing

Contributions are welcome! Please feel free to submit issues or pull requests.

## Release Notes

### 0.0.1

Initial release of Harness Syntax Highlighter

- Basic pipeline structure highlighting
- Variable expression support
- Step type recognition
- Variable definition highlighting
- Support for Harness expressions in strings

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author

**Mike Strid** - [mike.strid@protonmail.com](mailto:mike.strid@protonmail.com)

---

**Enjoy enhanced Harness pipeline development!**
