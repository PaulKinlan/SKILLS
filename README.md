# SKILLS

A collection of structured skill sets for AI assistants and development projects. These skills can be imported into Claude projects or other AI development environments to provide domain-specific expertise.

## Available Skill Sets

### 🌐 Modern Web Development

Comprehensive skills for building modern web applications with best practices across multiple disciplines.

**Path**: `modern-web-development/`

**Sub-Skills**:
- **Accessibility** (`accessibility/`) - WCAG compliance, ARIA, semantic HTML, keyboard navigation, screen reader support
- **Performance** (`performance/`) - Core Web Vitals, loading optimization, bundle optimization, caching strategies
- **Security** (`security/`) - OWASP Top 10, secure authentication, XSS/CSRF prevention, security headers
- **Best Practices** (`best-practices/`) - Code quality, design patterns, documentation, CI/CD, error handling
- **Testing** (`testing/`) - Unit testing, integration testing, E2E testing, TDD, test coverage

### 🧩 Chrome Extensions

Expert knowledge in developing Chrome browser extensions using Manifest V3.

**Path**: `chrome-extensions/`

**Covers**:
- Extension architecture and components
- Service workers and background scripts
- Content scripts and page interaction
- Chrome APIs (runtime, storage, tabs, scripting)
- Security best practices
- Publishing to Chrome Web Store
- Migration from Manifest V2 to V3

## Usage

### Install as Claude Code Plugin (Recommended)

Install directly from the marketplace using Claude Code:

```bash
# Add this marketplace
/plugin marketplace add PaulKinlan/SKILLS

# Install the plugin
/plugin install web-development-skills@PaulKinlan/SKILLS
```

Or install for your entire project team:

```bash
/plugin install web-development-skills@PaulKinlan/SKILLS --scope project
```

Once installed, all skills are automatically available to Claude Code:
- `modern-web-dev` - Modern web development best practices
- `chrome-extensions-development` - Chrome extension development
- `web-accessibility` - Web accessibility (WCAG, ARIA)
- `web-performance` - Performance optimization
- `web-security` - Web security best practices
- `web-best-practices` - Code quality and design patterns
- `web-testing` - Testing strategies and frameworks

### Manual Import (Alternative)

If you prefer to import skills manually:

1. Clone or download this repository
2. In your Claude project (Claude Code or similar), reference the skill folders you need
3. The AI will have access to the structured knowledge in each skill set

### Directory Structure

```
SKILLS/
├── modern-web-development/
│   ├── README.md
│   ├── accessibility/
│   │   └── README.md
│   ├── performance/
│   │   └── README.md
│   ├── security/
│   │   └── README.md
│   ├── best-practices/
│   │   └── README.md
│   └── testing/
│       └── README.md
└── chrome-extensions/
    └── README.md
```

## Contributing

Each skill is documented in its own README.md file with:
- Core competencies
- Best practices
- Common patterns
- Tools and resources
- Examples and code snippets

To add a new skill:
1. Create a new directory
2. Add a comprehensive README.md
3. Follow the existing documentation structure
4. Include practical examples and best practices

## License

See [LICENSE](LICENSE) file for details.