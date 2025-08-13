# Baby Assistant

Use Home Assistant to Track Daily Baby Tasks

## Contributing

We welcome contributions! This project uses modern Python development tools to ensure code quality and consistency.

### Development Setup

This project uses `uv` for dependency management. Follow these steps to set up your development environment:

1. **Install uv** (if not already installed):
   ```bash
   curl -LsSf https://astral.sh/uv/install.sh | sh
   ```

2. **Clone the repository**:
   ```bash
   git clone https://github.com/elsell/baby-assistant.git
   cd baby-assistant
   ```


3. **Install development dependencies**:
   ```bash
   uv sync
   ```

4. **Install pre-commit hooks**:
   ```bash
   pre-commit install
   ```

### Code Quality Tools

This project uses the following tools to maintain code quality:

- **[Ruff](https://docs.astral.sh/ruff/)** (v0.12.8+): Fast Python linter and formatter
- **[Mypy](https://mypy-lang.org/)** (v1.17.1+): Static type checker with strict mode enabled
- **[Pre-commit](https://pre-commit.com/)** (v4.3.0+): Git hooks for automatic code checking
- **[Commitizen](https://commitizen-tools.github.io/commitizen/)** (v4.1.0+): Enforces conventional commit messages

### Pre-commit Hooks

The following checks run automatically on every commit:

- **Ruff**: Lints and formats Python code
- **Mypy**: Performs type checking
- **Commitizen**: Validates commit message format (conventional commits)
- **File checks**: Trailing whitespace, end-of-file fixes, YAML/TOML/JSON syntax validation

To run all checks manually:
```bash
pre-commit run --all-files
```

### Commit Message Format

We follow the [Conventional Commits](https://www.conventionalcommits.org/) specification. Commit messages should be structured as:

```
<type>(<scope>): <subject>

[optional body]

[optional footer(s)]
```

Common types:
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation changes
- `style`: Code style changes (formatting, etc.)
- `refactor`: Code refactoring
- `test`: Test additions or changes
- `chore`: Maintenance tasks

Example:
```
feat(sensor): add diaper change tracking sensor
```

### Running Code Quality Checks

```bash
# Run all pre-commit hooks
pre-commit run --all-files
```
