# Contributing to JittoGen

Thank you for your interest in contributing to JittoGen. This document provides guidelines and information for contributors.

## Code of Conduct

By participating in this project, you agree to abide by our Code of Conduct. We are committed to providing a welcoming and inclusive environment for all contributors.

## Getting Started

### Development Setup

1. Fork the repository on GitHub
2. Clone your fork locally:
```bash
git clone https://github.com/your-username/jittogen.git
cd jittogen
```

3. Install dependencies:
```bash
npm install
```

4. Create a branch for your feature:
```bash
git checkout -b feature/your-feature-name
```

5. Set up environment variables:
```bash
cp .env.example .env.local
```

### Development Workflow

1. Make your changes in your feature branch
2. Test your changes thoroughly
3. Run the linter and fix any issues:
```bash
npm run lint
npm run lint:fix
```

4. Run tests:
```bash
npm test
```

5. Commit your changes with a descriptive message:
```bash
git commit -m "feat: add new MEV strategy detection"
```

6. Push to your fork:
```bash
git push origin feature/your-feature-name
```

7. Create a Pull Request on GitHub

## Contribution Guidelines

### Types of Contributions

We welcome several types of contributions:

- **Bug fixes**: Fix issues in existing functionality
- **Feature additions**: Add new features or capabilities
- **Documentation**: Improve or add documentation
- **Performance improvements**: Optimize existing code
- **Security enhancements**: Improve security measures
- **Testing**: Add or improve test coverage

### Coding Standards

#### TypeScript/JavaScript
- Use TypeScript for all new code
- Follow ESLint configuration
- Use meaningful variable and function names
- Add JSDoc comments for public APIs
- Prefer functional programming patterns where appropriate

#### React/Next.js
- Use functional components with hooks
- Follow React best practices
- Use proper TypeScript types for props
- Implement proper error boundaries
- Optimize for performance (memo, useMemo, useCallback)

#### Styling
- Use Tailwind CSS for styling
- Follow existing design patterns
- Ensure responsive design
- Maintain accessibility standards

### Commit Message Format

We use conventional commits for clear commit history:

```
type(scope): description

[optional body]

[optional footer]
```

Types:
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation changes
- `style`: Code style changes (formatting, etc.)
- `refactor`: Code refactoring
- `test`: Adding or updating tests
- `chore`: Maintenance tasks

Examples:
```
feat(trading): add sandwich attack detection
fix(wallet): resolve balance fetching issue
docs(readme): update installation instructions
```

### Pull Request Process

1. **Description**: Provide a clear description of what your PR does
2. **Testing**: Include information about how you tested your changes
3. **Screenshots**: Add screenshots for UI changes
4. **Breaking Changes**: Clearly document any breaking changes
5. **Related Issues**: Reference any related GitHub issues

### Pull Request Template

```markdown
## Description
Brief description of changes

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Breaking change
- [ ] Documentation update

## Testing
- [ ] Unit tests pass
- [ ] Integration tests pass
- [ ] Manual testing completed

## Screenshots (if applicable)

## Checklist
- [ ] Code follows project style guidelines
- [ ] Self-review completed
- [ ] Code is commented where necessary
- [ ] Documentation updated
- [ ] No new warnings introduced
```

## Development Guidelines

### Security Considerations

When contributing to JittoGen, keep these security aspects in mind:

- Never commit private keys or sensitive data
- Validate all user inputs
- Use secure communication for API calls
- Follow authentication best practices
- Implement proper error handling without exposing sensitive information

### Performance Guidelines

- Optimize database queries
- Use appropriate caching strategies
- Minimize bundle size
- Implement proper loading states
- Use React optimization techniques

### Testing Requirements

- Write unit tests for new functions
- Add integration tests for API endpoints
- Test error scenarios
- Ensure cross-browser compatibility
- Test responsive design on different screen sizes

## Project Structure

```
jittogen/
├── app/                    # Next.js app directory
│   ├── api/               # API routes
│   ├── globals.css        # Global styles
│   ├── layout.tsx         # Root layout
│   └── page.tsx          # Home page
├── components/            # React components
│   ├── ui/               # UI components
│   └── ...               # Feature components
├── lib/                  # Utility functions
├── public/               # Static assets
├── scripts/              # Build and utility scripts
├── docs/                 # Documentation
└── tests/                # Test files
```

## Issue Reporting

### Bug Reports

When reporting bugs, please include:

1. **Description**: Clear description of the issue
2. **Steps to Reproduce**: Detailed steps to reproduce the bug
3. **Expected Behavior**: What should happen
4. **Actual Behavior**: What actually happens
5. **Environment**: Browser, OS, Node.js version
6. **Screenshots**: If applicable
7. **Console Errors**: Any error messages

### Feature Requests

For feature requests, please provide:

1. **Problem Statement**: What problem does this solve?
2. **Proposed Solution**: How should it work?
3. **Alternatives**: Other solutions considered
4. **Use Cases**: Who would benefit from this feature?
5. **Implementation Ideas**: Technical approach (if applicable)

## Documentation

### Code Documentation

- Add JSDoc comments for all public functions
- Include parameter and return type information
- Provide usage examples for complex functions
- Document any side effects or important behavior

### User Documentation

- Update README.md for new features
- Add or update user guides
- Include configuration examples
- Document API changes

## Community

### Communication Channels

- **GitHub Issues**: Bug reports and feature requests
- **GitHub Discussions**: General questions and ideas
- **Discord**: Real-time community chat
- **Twitter**: Updates and announcements

### Getting Help

If you need help with contributing:

1. Check existing documentation
2. Search GitHub issues
3. Ask in GitHub Discussions
4. Join our Discord server

## Recognition

Contributors will be recognized in:

- README.md contributors section
- Release notes for significant contributions
- Special recognition for major features or fixes

## License

By contributing to JittoGen, you agree that your contributions will be licensed under the MIT License.

Thank you for contributing to JittoGen and helping make MEV trading more accessible!
```
