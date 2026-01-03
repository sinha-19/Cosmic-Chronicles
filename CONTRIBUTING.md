# Contributing to Cosmic Chronicles

First off, thank you for considering contributing to Cosmic Chronicles! It's people like you that make this game better for everyone.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Development Setup](#development-setup)
- [Coding Guidelines](#coding-guidelines)
- [Commit Guidelines](#commit-guidelines)
- [Pull Request Process](#pull-request-process)

## Code of Conduct

This project and everyone participating in it is governed by respect and professionalism. By participating, you are expected to uphold this standard. Please report unacceptable behavior by opening an issue.

## How Can I Contribute?

### Reporting Bugs

Before creating bug reports, please check existing issues to avoid duplicates. When creating a bug report, include as many details as possible:

**Bug Report Template:**
```markdown
**Describe the bug**
A clear description of what the bug is.

**To Reproduce**
Steps to reproduce the behavior:
1. Start game with seed '...'
2. Navigate to '...'
3. Select option '...'
4. See error

**Expected behavior**
What you expected to happen.

**Screenshots/Console Output**
If applicable, add screenshots or console output.

**System Information:**
 - OS: [e.g. Windows 10, Ubuntu 20.04]
 - Python Version: [e.g. 3.8.5]
 - Game Version: [e.g. 1.0.0]

**Additional context**
Any other relevant information.
```

### Suggesting Features

Feature suggestions are welcome! Please provide:

**Feature Request Template:**
```markdown
**Is your feature request related to a problem?**
A clear description of the problem.

**Describe the solution you'd like**
A clear description of what you want to happen.

**Describe alternatives you've considered**
Other solutions or features you've considered.

**Additional context**
Any other context or screenshots.
```

### Code Contributions

#### Areas to Contribute

- **New Features**: Combat abilities, locations, bosses, NPCs
- **Game Balance**: Power scaling, combat mechanics
- **UI/UX**: Better terminal interface, color schemes
- **Story**: More lore, dialogue, adventures
- **Performance**: Optimize generation algorithms
- **Documentation**: Improve README, add tutorials
- **Refactoring**: Clean up code, improve structure
- **Testing**: Add unit tests, integration tests

## Development Setup

1. **Fork the Repository**
   ```bash
   # Click 'Fork' on GitHub, then:
   git clone https://github.com/YOUR-USERNAME/Cosmic-Chronicles.git
   cd Cosmic-Chronicles
   ```

2. **Create a Branch**
   ```bash
   git checkout -b feature/your-feature-name
   # or
   git checkout -b fix/your-bug-fix
   ```

3. **Make Your Changes**
   - Edit the code
   - Test thoroughly
   - Ensure Python 3.6+ compatibility

4. **Test Your Changes**
   ```bash
   python game.py
   # Test all affected features
   # Try different seeds and scenarios
   ```

## Coding Guidelines

### Python Style

- Follow PEP 8 style guide
- Use tabs for indentation (as per existing code)
- Keep functions focused and single-purpose
- Add docstrings for complex functions
- Use meaningful variable names

### Code Structure

```python
# Good example
def create_character_name(self, prefix=""):
    """
    Generate a procedurally-generated character name.

    Args:
        prefix (str): Optional prefix for the name

    Returns:
        str: The generated character name
    """
    # Implementation
    pass

# Avoid
def cn(p=""):  # Unclear function and parameter names
    # Implementation
    pass
```

### Game Design Guidelines

- **Balance**: New features should not break game balance
- **Consistency**: Match the existing game's tone and style
- **Procedural**: Prefer procedural generation over hardcoded content
- **Seed-Based**: Ensure deterministic behavior with seeds
- **Save Compatible**: Don't break existing save files

### What to Avoid

- Breaking changes to save file format without migration
- Removing existing features without discussion
- Adding external dependencies without strong justification
- Hardcoding values that should be configurable
- Platform-specific code without cross-platform alternatives

## Commit Guidelines

### Commit Message Format

```
<type>(<scope>): <subject>

<body>

<footer>
```

### Types

- **feat**: New feature
- **fix**: Bug fix
- **docs**: Documentation changes
- **style**: Code style changes (formatting, etc.)
- **refactor**: Code refactoring
- **test**: Adding tests
- **chore**: Maintenance tasks

### Examples

```bash
feat(combat): add critical hit mechanic

Adds 10% chance for critical hits that deal 2x damage.
Applies to both player and enemies for balance.

Closes #42

---

fix(save): handle corrupted save files gracefully

Previously crashed when loading corrupted saves.
Now shows error message and returns to menu.

Fixes #38

---

docs(readme): add installation troubleshooting section

Added common issues and solutions for first-time players.
```

## Pull Request Process

1. **Update Documentation**
   - Update README.md if needed
   - Add entry to CHANGELOG.md
   - Update docstrings and comments

2. **Test Thoroughly**
   - Test on your platform
   - Test different seeds
   - Test save/load functionality
   - Test edge cases

3. **Create Pull Request**
   - Use a clear title
   - Reference related issues
   - Describe changes in detail
   - Include testing steps

**Pull Request Template:**
```markdown
## Description
Brief description of changes

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Breaking change
- [ ] Documentation update

## Testing
How was this tested?
- [ ] Tested on Windows
- [ ] Tested on Linux
- [ ] Tested on macOS
- [ ] Tested with various seeds
- [ ] Tested save/load functionality

## Checklist
- [ ] Code follows project style guidelines
- [ ] Self-reviewed the code
- [ ] Commented complex code sections
- [ ] Updated documentation
- [ ] Added entry to CHANGELOG.md
- [ ] No new warnings introduced
- [ ] Tested thoroughly

## Screenshots (if applicable)
Add screenshots of new features

## Related Issues
Fixes #(issue number)
```

4. **Code Review**
   - Be open to feedback
   - Make requested changes
   - Discuss disagreements respectfully

5. **Merge**
   - Maintainer will merge when approved
   - Your contribution will be credited

## Development Ideas

### Easy Contributions (Good First Issues)

- Add new random adventure scenarios
- Add new NPC dialogue options
- Create new procedurally-generated names
- Add color schemes
- Improve error messages
- Fix typos in text

### Medium Contributions

- Add new special locations
- Create new boss characters
- Implement achievement system
- Add character stats display
- Improve combat UI
- Add difficulty levels

### Advanced Contributions

- Refactor universe generation
- Optimize performance
- Add automated testing
- Create level generation system
- Implement universe history tracking
- Add mod support

## Questions?

Feel free to:
- Open an issue for questions
- Start a discussion in GitHub Discussions
- Contact the maintainer

## Recognition

Contributors will be:
- Listed in the README credits section
- Mentioned in release notes
- Credited in CHANGELOG.md

Thank you for contributing to Cosmic Chronicles!
