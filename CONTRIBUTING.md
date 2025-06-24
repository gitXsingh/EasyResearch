# Contributing to PaperTeller

Thank you for your interest in contributing to PaperTeller! This document provides guidelines and information for contributors.

## 🤝 How to Contribute

### Reporting Bugs
- Use the GitHub issue tracker
- Include detailed steps to reproduce the bug
- Provide your operating system and environment details
- Include error messages and logs

### Suggesting Features
- Check existing issues to avoid duplicates
- Describe the feature clearly and its benefits
- Consider implementation complexity

### Code Contributions
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Add tests if applicable
5. Commit your changes (`git commit -m 'Add amazing feature'`)
6. Push to the branch (`git push origin feature/amazing-feature`)
7. Open a Pull Request

## 🛠️ Development Setup

### Backend Development
```bash
cd backend
python -m venv venv
venv\Scripts\activate  # Windows
# or
source venv/bin/activate  # Mac/Linux
pip install -r requirements.txt
pip install -r requirements_training.txt  # For AI model development
```

### Frontend Development
```bash
cd frontend
npm install
npm start
```

### Running Tests
```bash
# Backend tests
cd backend
python -m pytest

# Frontend tests
cd frontend
npm test
```

## 📝 Code Style

### Python (Backend)
- Follow PEP 8 style guide
- Use type hints where appropriate
- Add docstrings to functions and classes
- Keep functions small and focused

### JavaScript/React (Frontend)
- Use ESLint and Prettier
- Follow React best practices
- Use functional components with hooks
- Keep components small and reusable

## 🧪 Testing

### Backend Testing
- Write unit tests for new functions
- Test API endpoints
- Include integration tests for AI features

### Frontend Testing
- Test component rendering
- Test user interactions
- Test API integration

## 📚 Documentation

- Update README.md for new features
- Add inline code comments
- Update API documentation
- Include usage examples

## 🔒 Security

- Don't commit API keys or sensitive data
- Use environment variables for configuration
- Validate all user inputs
- Follow security best practices

## 🚀 Pull Request Process

1. **Fork and Clone**: Fork the repo and clone locally
2. **Create Branch**: Create a feature branch
3. **Make Changes**: Implement your feature/fix
4. **Test**: Ensure all tests pass
5. **Document**: Update documentation as needed
6. **Commit**: Use clear, descriptive commit messages
7. **Push**: Push to your fork
8. **Submit PR**: Create a pull request with clear description

### Pull Request Guidelines
- Use a clear title and description
- Reference related issues
- Include screenshots for UI changes
- Ensure CI/CD checks pass
- Request reviews from maintainers

## 🏷️ Commit Message Format

Use conventional commit format:
```
type(scope): description

[optional body]

[optional footer]
```

Types:
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation changes
- `style`: Code style changes
- `refactor`: Code refactoring
- `test`: Adding tests
- `chore`: Maintenance tasks

## 🎯 Areas for Contribution

### High Priority
- Bug fixes
- Performance improvements
- Security enhancements
- Documentation improvements

### Medium Priority
- New AI model integrations
- UI/UX improvements
- Additional file format support
- Testing coverage

### Low Priority
- Code refactoring
- Minor UI tweaks
- Additional language support

## 📞 Getting Help

- Open an issue for questions
- Join our discussions
- Check existing documentation
- Review existing issues and PRs

## 🙏 Recognition

Contributors will be recognized in:
- README.md contributors section
- Release notes
- Project documentation

Thank you for contributing to PaperTeller! 🎉 