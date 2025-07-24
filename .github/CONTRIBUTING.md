# Contributing to Harness Syntax Highlighter

Thank you for your interest in contributing! This document provides guidelines for contributing to the Harness Syntax Highlighter extension.

## 🚀 Getting Started

1. **Fork the repository** on GitHub
2. **Clone your fork** locally
3. **Create a branch** for your changes
4. **Make your changes** and test them
5. **Submit a pull request**

## 🐛 Reporting Bugs

Before submitting a bug report:
1. **Search existing issues** to avoid duplicates
2. **Use the bug report template** when creating new issues
3. **Include all requested information**

**Security Note**: Never include sensitive information like API keys, credentials, or confidential data in bug reports.

## 💡 Suggesting Features

We welcome feature suggestions! Please:
1. **Use the feature request template**
2. **Explain the use case** and how it would improve the Harness development experience
3. **Check existing feature requests** to avoid duplicates

## 🔧 Development Setup

### Prerequisites
- Node.js (v18+)
- npm
- VS Code
- Git

### Setup
```bash
# Clone your fork
git clone https://github.com/YOUR_USERNAME/harness-syntax-highlighter.git
cd harness-syntax-highlighter

# Install dependencies
npm install

# Open in VS Code
code .
```

### Testing
1. Press `F5` in VS Code to launch Extension Development Host
2. Open a Harness YAML file to test syntax highlighting
3. Make changes and reload the extension host

## 📝 Pull Request Guidelines

### Before Submitting
- [ ] Test your changes thoroughly
- [ ] Update documentation if needed
- [ ] Follow the existing code style
- [ ] Write clear commit messages

### Pull Request Process
1. **Create a descriptive title**
2. **Fill out the PR template** (when available)
3. **Link related issues** using keywords like "Fixes #123"
4. **Request review** from maintainers

### Commit Message Format
```
type(scope): description

[optional body]

[optional footer]
```

Examples:
- `feat: add support for Harness step groups`
- `fix: resolve variable highlighting in expressions`
- `docs: update README with new features`

## 🎨 Code Style

- Use consistent indentation (2 spaces)
- Follow existing naming conventions
- Comment complex logic
- Keep functions focused and small

## 📚 Documentation

When contributing:
- Update README.md if adding new features
- Add comments for complex syntax rules
- Update CHANGELOG.md for user-facing changes

## 🔒 Security

- **Never commit sensitive information**
- **Review dependencies** for security issues
- **Follow secure coding practices**
- **Report security issues privately** (see SECURITY.md)

## ❓ Questions

- **GitHub Discussions**: For general questions and community help
- **Issues**: For bug reports and feature requests
- **Email**: mike.strid@protonmail.com for security concerns

## 🏆 Recognition

Contributors will be acknowledged in release notes and the README.md file.

## 📄 License

By contributing, you agree that your contributions will be licensed under the MIT License.
