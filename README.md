# 📚 Prompt Library - Gemini CLI Extension

A curated library of high-quality, professionally crafted prompts for common development tasks. Save time and improve your AI interactions with battle-tested prompt templates.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Gemini CLI](https://img.shields.io/badge/Gemini%20CLI-Extension-blue)](https://geminicli.com/)

## ✨ Features

- 🎯 **30+ Professional Prompts** - Carefully crafted for common development tasks
- 🚀 **Instant Access** - Simple slash commands for quick execution
- 📖 **Learn by Example** - See prompt engineering best practices in action
- 🎨 **Organized Categories** - Easy to browse and discover prompts
- 🔧 **Customizable** - Fork and adapt prompts to your needs
- 💡 **Educational** - Learn prompt engineering principles

## 📦 Installation

Install the extension using the Gemini CLI:

```bash
gemini extensions install involvex/prompt-library-extension
```

Or install from a local directory:

```bash
git clone https://github.com/involvex/prompt-library-extension.git
cd prompt-library-extension
gemini extensions link .
```

## 🚀 Quick Start

After installation, restart Gemini CLI and start using prompts:

```bash
# Review code for security issues
/code-review:security "your code here"

# Generate a README file
/docs:write-readme "describe your project"

# Create unit tests
/testing:generate-unit-tests "your function here"

# Explain a complex concept
/learning:explain-concept "recursion"

# Debug an error
/debugging:debug-error "paste your error here"
```

## 📋 Available Prompts

### 🔍 Code Review & Analysis
- `/code-review:security` - Deep security analysis
- `/code-review:performance` - Performance optimization
- `/code-review:best-practices` - Best practices review
- `/code-review:refactor` - Refactoring suggestions

### 📝 Documentation
- `/docs:write-readme` - Generate comprehensive README
- `/docs:write-api-docs` - Create API documentation
- `/docs:write-changelog` - Generate changelog
- `/docs:write-contributing` - Create contribution guidelines

### 🧪 Testing
- `/testing:generate-unit-tests` - Create unit tests
- `/testing:generate-e2e-tests` - Create end-to-end tests
- `/testing:edge-cases` - Identify edge cases
- `/testing:coverage-analysis` - Analyze test coverage

### 🐛 Debugging
- `/debugging:debug-error` - Diagnose and fix errors
- `/debugging:trace-issue` - Root cause analysis
- `/debugging:performance-profile` - Performance profiling

### 🏗️ Architecture & Design
- `/architecture:design-api` - Design RESTful APIs
- `/architecture:design-database` - Design database schemas
- `/architecture:system-design` - System architecture
- `/architecture:design-patterns` - Suggest design patterns

### 📚 Learning & Explanation
- `/learning:explain-concept` - Explain technical concepts
- `/learning:eli5` - Explain like I'm 5
- `/learning:compare-tech` - Compare technologies
- `/learning:roadmap` - Create learning paths

### ✍️ Writing & Communication
- `/writing:technical-blog` - Write technical posts
- `/writing:email` - Draft professional emails
- `/writing:presentation` - Create presentation outlines

### 🎨 Prompt Engineering
- `/prompts:improve` - Improve existing prompts
- `/prompts:create-template` - Create prompt templates
- `/prompts:best-practices` - Learn prompt tips

## 💡 Usage Examples

### Security Code Review

```bash
/code-review:security "
function loginUser(username, password) {
  const query = 'SELECT * FROM users WHERE username = ' + username;
  return db.execute(query);
}
"
```

**Output:** Comprehensive security analysis identifying SQL injection vulnerability, authentication issues, and providing secure code examples.

### Generate Unit Tests

```bash
/testing:generate-unit-tests "
function calculateDiscount(price, discountPercent) {
  return price - (price * discountPercent / 100);
}
"
```

**Output:** Complete test suite with happy paths, edge cases, boundary values, and error conditions.

### Explain Concept

```bash
/learning:explain-concept "closures in JavaScript"
```

**Output:** Multi-level explanation from ELI5 to technical details, with examples, use cases, and best practices.

### Design API

```bash
/architecture:design-api "A blog platform with posts, comments, users, and tags"
```

**Output:** Complete REST API design with endpoints, data models, authentication, and OpenAPI documentation.

## 🎯 Why Use This Extension?

### Save Time
- Pre-crafted prompts eliminate trial and error
- Instant access via simple commands
- Consistent, high-quality results

### Improve Quality
- Based on prompt engineering best practices
- Comprehensive, structured outputs
- Professional-grade results

### Learn Prompt Engineering
- See examples of effective prompts
- Understand what makes prompts work
- Build your own custom prompts

### Boost Productivity
- Quick access to common tasks
- Reduce context switching
- Focus on problem-solving, not prompt crafting

## 🛠️ Customization

### Adding Your Own Prompts

1. Create a new `.toml` file in the appropriate `commands/` subdirectory:

```bash
mkdir -p commands/mycategory
touch commands/mycategory/myprompt.toml
```

2. Write your prompt:

```toml
prompt = """
# My Custom Prompt

Your prompt content here with {{args}} for user input.
"""
```

3. Restart Gemini CLI to load the new prompt

### Modifying Existing Prompts

Fork the repository and edit any `.toml` file to customize prompts to your needs.

## 📚 Prompt Engineering Tips

Based on the prompts in this library, here are key principles:

### 1. **Be Specific**
```
❌ "Review this code"
✅ "Perform a security analysis focusing on input validation, SQL injection, and XSS vulnerabilities"
```

### 2. **Provide Structure**
Use clear sections, numbering, and formatting to guide the AI's response.

### 3. **Include Context**
Specify the language, framework, use case, and constraints.

### 4. **Request Examples**
Ask for code examples, not just explanations.

### 5. **Define Output Format**
Specify exactly how you want the response structured.

### 6. **Use Variables**
Make prompts reusable with `{{args}}` placeholders.

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Add New Prompts** - Share your best prompts
2. **Improve Existing Prompts** - Make them clearer and more effective
3. **Report Issues** - Found a bug or unclear prompt?
4. **Suggest Categories** - What prompt categories are missing?

### Contribution Guidelines

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/new-prompt`
3. Add your prompt in the appropriate category
4. Test it thoroughly
5. Submit a pull request with clear description

## 📖 Documentation

For more information about Gemini CLI extensions:
- [Gemini CLI Documentation](https://geminicli.com/docs/)
- [Extension Development Guide](https://geminicli.com/docs/extensions/)
- [Model Context Protocol](https://modelcontextprotocol.io/)

## 📄 License

MIT License - see [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Inspired by the Gemini CLI community
- Built on prompt engineering best practices
- Thanks to all contributors

## 📞 Support

- 🐛 [Report Issues](https://github.com/involvex/prompt-library-extension/issues)
- 💬 [Discussions](https://github.com/involvex/prompt-library-extension/discussions)

## 🗺️ Roadmap

- [ ] Add more prompt categories
- [ ] Interactive prompt builder
- [ ] Prompt analytics (most used, success rate)
- [ ] Community prompt sharing
- [ ] Multi-language support
- [ ] Prompt versioning
- [ ] A/B testing for prompts

---

## About me
My name is Harish Garg. I am a solo developer. I write at my blog [here](https://harishgarg.com/).

I also maintain a [MCP Resources Directory](https://www.mcpstack.org/) & a [coding ai tools directory](https://www.codeaidirectory.com/)

---

**Made with ❤️ for the Gemini CLI community**

Star ⭐ this repo if you find it useful!

