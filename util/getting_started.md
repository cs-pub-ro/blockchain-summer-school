# 🚀 Getting Started

Welcome to the Blockchain Summer School! This guide will help you set up your development environment and get ready for an exciting journey into blockchain technology.

## 📋 Prerequisites

### Required Knowledge
- **Basic Programming**: Familiarity with at least one programming language (Python, JavaScript, Rust, or similar)
- **Command Line**: Comfort with terminal/command prompt operations
- **Git**: Basic understanding of version control (we'll cover this if needed)

### Recommended Knowledge (Optional)
- **Web Development**: HTML, CSS, JavaScript basics
- **Cryptography**: Basic understanding of public/private keys
- **Distributed Systems**: Familiarity with client-server architecture

## 💻 System Requirements

### Minimum Requirements
- **Operating System**: Windows 10+, macOS 10.15+, or Linux (Ubuntu 18.04+)
- **RAM**: 8GB minimum, 16GB recommended
- **Storage**: 10GB free space
- **Internet**: Stable broadband connection

### Recommended Setup
- **RAM**: 16GB or more
- **Storage**: SSD with 20GB+ free space
- **Processor**: Multi-core processor (Intel i5/AMD Ryzen 5 or better)

## 🛠 Development Environment Setup

### Step 1: Install Core Tools

#### 1.1 Git & GitHub
```bash
# Install Git (if not already installed)
# Windows: Download from https://git-scm.com/
# macOS: brew install git
# Ubuntu/Debian: sudo apt-get install git

# Verify installation
git --version
```

#### 1.2 Node.js & npm
```bash
# Install Node.js (includes npm)
# Download from https://nodejs.org/ (LTS version recommended)

# Verify installation
node --version
npm --version
```

#### 1.3 Python 3
```bash
# Windows: Download from https://python.org/
# macOS: brew install python3
# Ubuntu/Debian: sudo apt-get install python3 python3-pip

# Verify installation
python3 --version
pip3 --version
```

### Step 2: Install Blockchain-Specific Tools

#### 2.1 Rust Toolchain
```bash
# Install Rust
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

# Add to PATH (restart terminal after installation)
source ~/.cargo/env

# Verify installation
rustup --version
cargo --version

# Add WebAssembly target for MultiversX
rustup target add wasm32-unknown-unknown
```

#### 2.2 MultiversX Tools
```bash
# Install mxpy (MultiversX CLI)
pipx install multiversx-sdk-cli --force

# Install sc-meta (Smart Contract Meta)
cargo install multiversx-sc-meta --locked

# Verify installations
mxpy --version
sc-meta --version
```

#### 2.3 Ethereum Development Tools
```bash
# Install Hardhat
npm install --save-dev hardhat

# Verify installation
npx hardhat --version
```

### Step 3: Install Wallets & Extensions

#### 3.1 MetaMask
- **Browser Extension**: [Chrome](https://chrome.google.com/webstore/detail/metamask/nkbihfbeogaeaoehlefnkodbefgpgknn) | [Firefox](https://addons.mozilla.org/en-US/firefox/addon/ether-metamask/)
- **Mobile App**: [iOS](https://apps.apple.com/app/metamask/id1438144202) | [Android](https://play.google.com/store/apps/details?id=io.metamask)

#### 3.2 MultiversX Wallet
- **Browser Extension**: [DeFi Wallet](https://defi-wallet.multiversx.com/)
- **Mobile App**: [xPortal](https://xportal.com/)

### Step 4: Install Code Editor

#### Recommended: Visual Studio Code
- **Download**: [https://code.visualstudio.com/](https://code.visualstudio.com/)
- **Recommended Extensions**:
  - Solidity (for Ethereum smart contracts)
  - Rust Analyzer (for Rust development)
  - Hardhat for VS Code
  - GitLens
  - Live Share (for collaboration)

## 🎯 Learning Paths

### 🟢 Beginner Track (0-2 months experience)
**Estimated Time**: 4-6 hours/week
1. **Week 1-2**: Introduction to Blockchain & Setup
   - Complete environment setup
   - Read: [Introduction Chapter](../chapters/introduction/)
   - Practice: Create your first wallet

2. **Week 3-4**: Smart Contracts Basics
   - Read: [Smart Contracts Chapter](../chapters/smart-contracts/)
   - Practice: Deploy a simple "Hello World" contract

3. **Week 5-6**: dApps & Tokens
   - Read: [dApps Chapter](../chapters/dApps/) & [Tokens Chapter](../chapters/tokens/)
   - Practice: Create a simple token

### 🟡 Intermediate Track (2-6 months experience)
**Estimated Time**: 6-8 hours/week
1. **Week 1-2**: Advanced Smart Contracts
   - Read: [Security Chapter](../chapters/security/)
   - Practice: Build a secure voting system

2. **Week 3-4**: DeFi & Money Protocols
   - Read: [Money Chapter](../chapters/money/)
   - Practice: Implement a simple DEX

3. **Week 5-6**: Cross-Chain & Interoperability
   - Read: [Composability Chapter](../chapters/composability/)
   - Practice: Build a cross-chain bridge

### 🔴 Advanced Track (6+ months experience)
**Estimated Time**: 8-12 hours/week
1. **Week 1-2**: Protocol Development
   - Read: [Protocol Chapter](../chapters/protocol/)
   - Practice: Implement consensus mechanisms

2. **Week 3-4**: Security & CTF
   - Read: [Security Chapter](../chapters/security/)
   - Practice: Solve CTF challenges

3. **Week 5-6**: Research & Innovation
   - Read: [VM Chapter](../chapters/vm/)
   - Practice: Contribute to open-source projects

## 📚 First Steps

### 1. Clone the Repository
```bash
git clone https://github.com/cs-pub-ro/blockchain-summer-school.git
cd blockchain-summer-school
```

### 2. Join the Community
- **Discord**: [Join our Discord server](https://discord.gg/blockchain-summer-school)
- **GitHub Discussions**: [Ask questions here](https://github.com/cs-pub-ro/blockchain-summer-school/discussions)
- **Office Hours**: Check the schedule for live Q&A sessions

### 3. Complete the Setup Verification
Run our setup verification script:
```bash
# Navigate to the verification script
cd chapters/introduction/lab/content/setup/

# Run verification (if available)
./verify-setup.sh
```

### 4. Start with the Introduction
Begin your journey with the [Introduction Chapter](../chapters/introduction/):
- Read the lecture slides
- Complete the lab exercises
- Set up your first wallet
- Make your first transaction

## 🆘 Troubleshooting

### Common Issues

#### Rust Installation Problems
```bash
# If rustup installation fails
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- --default-toolchain stable

# If cargo is not found
export PATH="$HOME/.cargo/bin:$PATH"
```

#### mxpy Installation Issues
```bash
# If pipx is not installed
python3 -m pip install --user pipx
python3 -m pipx ensurepath

# If mxpy installation fails
pipx install multiversx-sdk-cli --force --include-deps
```

#### Node.js/npm Issues
```bash
# Clear npm cache
npm cache clean --force

# Update npm
npm install -g npm@latest
```

#### MetaMask Connection Issues
- Ensure you're on the correct network (Testnet/Mainnet)
- Check if MetaMask is unlocked
- Try refreshing the page
- Clear browser cache if needed

### Getting Help

#### Before Asking for Help
1. **Check the documentation**: Most issues are covered in the setup guides
2. **Search existing issues**: Use GitHub search to find similar problems
3. **Verify your setup**: Run the verification script
4. **Check system requirements**: Ensure your system meets the minimum requirements

#### How to Ask for Help
When asking for help, please include:
- **Operating System**: Windows/macOS/Linux version
- **Error Message**: Copy the exact error message
- **Steps Taken**: What you've already tried
- **Expected vs Actual**: What you expected to happen vs what happened

#### Support Channels
1. **GitHub Issues**: For technical problems and bugs
2. **Discord**: For quick questions and community support
3. **Email**: `costin.carabas@upb.ro` for urgent matters
4. **Office Hours**: For live troubleshooting sessions

## 🎓 Success Tips

### Time Management
- **Consistent Schedule**: Dedicate 2-3 hours, 3-4 times per week
- **Break Down Tasks**: Don't try to learn everything at once
- **Practice Regularly**: Code daily, even if just for 30 minutes

### Learning Strategies
- **Hands-on Practice**: Don't just read - build something
- **Join Study Groups**: Collaborate with other students
- **Document Your Progress**: Keep a learning journal
- **Ask Questions**: Don't hesitate to ask for clarification

### Project Development
- **Start Small**: Begin with simple projects and gradually increase complexity
- **Version Control**: Use Git from day one
- **Documentation**: Write clear README files for your projects
- **Testing**: Always test your smart contracts thoroughly

## 🏆 Next Steps

Once you've completed the setup:

1. **Choose Your Track**: Decide which learning path fits your experience level
2. **Set Goals**: Define what you want to achieve by the end of the program
3. **Join a Team**: Find teammates for the final project (optional)
4. **Stay Updated**: Follow blockchain news and developments
5. **Build Portfolio**: Start building projects for your portfolio

---

**Ready to start?** Begin with the [Introduction Chapter](../chapters/introduction/) and happy coding! 🚀

*Need help? Check our [FAQ](FAQ.md) or reach out to the community.* 