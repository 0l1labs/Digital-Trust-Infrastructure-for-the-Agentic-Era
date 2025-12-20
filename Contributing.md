# Contributing to Nomad Trust Layer

Thank you for your interest in contributing to Nomad Trust Layer! This document provides guidelines for contributing to our AI agent verification infrastructure powered by zero-knowledge proofs.

## Code of Conduct

This project adheres to a Code of Conduct that all contributors are expected to follow. Please read [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) before contributing.

## How to Contribute

### Reporting Bugs

If you find a bug, please create an issue with:

* **Clear title** - Describe the problem concisely
* **Steps to reproduce** - Detailed steps to trigger the bug
* **Expected behavior** - What should happen
* **Actual behavior** - What actually happens
* **Environment** - OS, browser, Node version, etc.
* **Screenshots** - If applicable

### Suggesting Enhancements

We welcome feature suggestions! Please create an issue with:

* **Use case** - Why is this needed?
* **Proposed solution** - How should it work?
* **Alternatives** - Other approaches considered?
* **Additional context** - Screenshots, mockups, examples

### Pull Requests

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature/amazing-feature`
3. **Make your changes**
4. **Test thoroughly**
5. **Commit with clear messages**: `git commit -m 'Add amazing feature'`
6. **Push to your fork**: `git push origin feature/amazing-feature`
7. **Open a Pull Request**

#### PR Guidelines

* **Description** - Explain what and why
* **Testing** - Describe how you tested
* **Screenshots** - If UI changes
* **Breaking changes** - Call out any breaking changes
* **Link issues** - Reference related issues

### Development Setup
```bash
# Clone your fork
git clone https://github.com/YOUR-USERNAME/Nomad-Genesis-Channel
cd Nomad-Genesis-Channel

# Add upstream remote
git remote add upstream https://github.com/NomadTrustLayer/Nomad-Genesis-Channel

# Install dependencies (if applicable)
npm install  # or pip install -r requirements.txt

# Create feature branch
git checkout -b feature/your-feature-name
```

### Coding Standards

**General:**
* Write clear, self-documenting code
* Add comments for complex logic
* Follow existing code style
* Keep functions small and focused

**Python:**
* Follow PEP 8 style guide
* Use type hints where applicable
* Write docstrings for functions/classes

**JavaScript/TypeScript:**
* Follow Airbnb style guide (or project-specific ESLint config)
* Use meaningful variable names
* Write JSDoc comments for functions

**Circom (ZK Circuits):**
* Comment circuit logic thoroughly
* Explain constraints clearly
* Document signal purposes
* Include test cases for all circuits

**Solidity (Smart Contracts):**
* Follow Solidity style guide
* Use NatSpec documentation
* Write comprehensive tests
* Gas optimization is important
* Security-first mindset

### Testing

**All contributions should include tests:**

* **Unit tests** - Test individual functions
* **Integration tests** - Test component interactions
* **Circuit tests** - Verify ZK circuit correctness and constraint satisfaction
* **Contract tests** - Verify smart contract behavior and edge cases
* **AI agent integration tests** - Test proof generation and verification workflows
```bash
# Run tests (example commands)
npm test
pytest
hardhat test
forge test
```

### Documentation

**Update documentation when:**
* Adding new features
* Changing existing behavior
* Fixing bugs that affect usage
* Improving explanations

**Documentation includes:**
* README.md updates
* Code comments
* API documentation
* Technical specifications
* Integration guides

## Open Source Scope

### What's Open Source

**These components are open source (MIT License):**

* ✅ ZK circuit code (Circom)
* ✅ Smart contract code (Solidity)
* ✅ Frontend proof generation libraries (JavaScript/TypeScript)
* ✅ Genesis Channel routing logic
* ✅ Public API client libraries
* ✅ Documentation and examples

### What's Proprietary

**These remain proprietary:**

* ❌ API backend services
* ❌ Enterprise integration code
* ❌ Customer data and analytics
* ❌ Internal operational tools (beyond public channel holder dashboard)

## Security Contributions

**Found a security vulnerability?**

* **DO NOT** create a public issue
* **Email:** security@nomadtrust.io
* See [SECURITY.md](SECURITY.md) for full policy

We take security seriously and will respond promptly to responsible disclosures.

## Communication Channels

* **GitHub Issues** - Bug reports, feature requests
* **GitHub Discussions** - General questions, ideas
* **Discord** - Community chat: [discord.gg/nomadtrustlayer](https://discord.gg/nomadtrustlayer)
* **Twitter** - [@nomadtrustlayer](https://twitter.com/nomadtrustlayer)

## Recognition

Contributors will be:

* Listed in [CONTRIBUTORS.md](CONTRIBUTORS.md)
* Mentioned in release notes (for significant contributions)
* Invited to community events
* Considered for future opportunities

## Questions?

Not sure where to start? Have questions about contributing?

* Check existing issues for "good first issue" label
* Ask in GitHub Discussions
* Reach out on Discord
* Email: team@nomadtrust.io

## License

By contributing to Nomad Trust Layer, you agree that your contributions will be licensed under the MIT License (for code) and CC BY-SA 4.0 (for documentation).

See [LICENSE](LICENSE) for details.

---

**Thank you for contributing to the AI agent verification infrastructure!** 🚀
