# Contributing to MCP Playwright

🎉 **Thank you for considering contributing to MCP Playwright!** 

We're excited to have you join our community of developers building the future of AI-powered browser automation.

## 🚀 Quick Start for Contributors

1. **Fork** the repository
2. **Clone** your fork: `git clone https://github.com/YOUR_USERNAME/mcp-playwright.git`
3. **Install** dependencies: `npm install`
4. **Run** tests: `npm test`
5. **Create** a feature branch: `git checkout -b feature/amazing-feature`

## 🎯 Ways to Contribute

### 🐛 Bug Reports
Found a bug? Help us squash it!
- Use the [Bug Report Template](.github/ISSUE_TEMPLATE/bug_report.md)
- Include steps to reproduce
- Provide browser/OS information
- Add screenshots if applicable

### 💡 Feature Requests
Have an idea? We'd love to hear it!
- Use the [Feature Request Template](.github/ISSUE_TEMPLATE/feature_request.md)
- Explain the use case
- Describe the proposed solution
- Consider implementation complexity

### 📝 Documentation
Help make our docs amazing:
- Fix typos and improve clarity
- Add examples and tutorials
- Translate documentation
- Create video tutorials

### 🧪 Testing
Improve our test coverage:
- Add unit tests for new features
- Create integration tests
- Test edge cases
- Performance testing

## 📋 Development Workflow

### Setting Up Your Environment

```bash
# Clone the repository
git clone https://github.com/MostafaRaafat91/mcp-playwright.git
cd mcp-playwright

# Install dependencies
npm install

# Install Playwright browsers
npm run install:browsers

# Run tests to verify setup
npm test

# Start development server
npm run dev
```

### Making Changes

1. **Create a Branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

2. **Write Code**
   - Follow our coding standards (see below)
   - Add tests for new functionality
   - Update documentation as needed

3. **Test Your Changes**
   ```bash
   npm run test          # Run all tests
   npm run test:unit     # Unit tests only
   npm run test:e2e      # E2E tests only
   npm run lint          # Check code style
   ```

4. **Commit Your Changes**
   ```bash
   git add .
   git commit -m "feat: add amazing new feature"
   ```

5. **Push and Create PR**
   ```bash
   git push origin feature/your-feature-name
   ```

## 📏 Coding Standards

### Code Style
- Use **TypeScript** for new code
- Follow **Prettier** formatting (run `npm run format`)
- Use **ESLint** rules (run `npm run lint`)
- Write **descriptive variable names**

### Commit Messages
We follow [Conventional Commits](https://conventionalcommits.org/):

```
type(scope): description

feat(browser): add support for Firefox mobile
fix(auth): resolve login timeout issue
docs(readme): update installation guide
test(e2e): add checkout flow tests
```

### Testing Guidelines
- **Unit tests** for individual functions
- **Integration tests** for MCP server communication
- **E2E tests** for complete workflows
- **Minimum 80% coverage** for new code

## 🏗️ Architecture Overview

```
src/
├── index.js           # Main MCP server entry point
├── browser/           # Browser management
├── tools/             # MCP tool implementations
├── utils/             # Shared utilities
└── types/             # TypeScript definitions

tests/
├── unit/              # Unit tests
├── integration/       # Integration tests
└── e2e/               # End-to-end tests
```

## 🎨 Adding New MCP Tools

1. **Create the tool definition** in `src/tools/`
2. **Add to tool registry** in `src/index.js`
3. **Write comprehensive tests**
4. **Update documentation**

Example:
```javascript
// src/tools/newTool.js
export async function newTool(params) {
  // Implementation
  return { success: true, data: result };
}

// Add to src/index.js tools array
{
  name: "new_tool",
  description: "Does something amazing",
  inputSchema: {
    type: "object",
    properties: {
      param1: { type: "string", description: "Parameter description" }
    },
    required: ["param1"]
  }
}
```

## 🎖️ Recognition

Contributors get:
- 🏆 **Credit** in our README
- 🎖️ **Contributor badge** on Discord
- 📧 **Early access** to new features
- 🎁 **Swag** for significant contributions

## 📞 Getting Help

- 💬 **Discord**: [Join our community](https://discord.gg/mcpplaywright)
- 🐛 **Issues**: [GitHub Issues](https://github.com/MostafaRaafat91/mcp-playwright/issues)
- 📧 **Email**: mostafa.raafat91@gmail.com
- 🐦 **Twitter**: [@M_H1191](https://twitter.com/M_H1191)

## 📝 License

By contributing, you agree that your contributions will be licensed under the MIT License.

---

<div align="center">

**🚀 Ready to contribute? [Create your first PR!](https://github.com/MostafaRaafat91/mcp-playwright/compare)**

*Together, we're building the future of AI-powered automation* ❤️

</div>