# CipherBlog

> **Privacy-preserving blog platform powered by Zama FHEVM**

CipherBlog enables confidential blog publishing using Zama's Fully Homomorphic Encryption Virtual Machine. Your blog posts and content remain encrypted during storage, processing, and retrieval—complete privacy protection.

---

## The Blogging Privacy Challenge

Traditional blogging platforms can read and index your content. **CipherBlog eliminates this** by encrypting all blog posts with FHE, ensuring only you and authorized readers can decrypt the content.

### Current Blogging Issues

- ❌ Content readable by platform operators
- ❌ Search indexing exposes private posts
- ❌ Centralized storage risks
- ❌ Limited content control

### CipherBlog Solution

- ✅ Posts encrypted with Zama FHE
- ✅ Processing without decryption
- ✅ Decentralized blockchain storage
- ✅ Complete author control

---

## Zama FHEVM for Private Blogging

### Why FHE Matters for Blogs

**FHEVM** (Fully Homomorphic Encryption Virtual Machine) enables blog post processing, search, and categorization while content remains encrypted. Your thoughts stay private.

### How CipherBlog Protects Content

```
┌──────────────┐
│ Blog Post    │
│ Content      │
└──────┬───────┘
       │
       ▼ FHE Encryption
┌──────────────┐
│ Encrypted    │
│ Blog Post    │
└──────┬───────┘
       │
       ▼
┌──────────────────────┐
│  FHEVM Blog          │
│  Contract            │
│  (CipherBlog)        │
│  ┌──────────────┐    │
│  │ Store        │    │ ← Encrypted storage
│  │ Encrypted    │    │
│  │ Post         │    │
│  │ Process      │    │
│  └──────────────┘    │
└──────┬───────────────┘
       │
       ▼
┌──────────────────────┐
│ Zama FHE Runtime     │
│ Blog Content         │
│ Processing           │
└──────┬───────────────┘
       │
       ▼
┌──────────────┐
│ Encrypted    │
│ Blog Storage │
│ (Only author │
│  can decrypt)│
└──────────────┘
```

### Privacy Features

- 🔐 **Encrypted Posts**: All blog content encrypted with FHE
- 🔒 **Private Publishing**: Posts stored without decryption
- ✅ **Selective Sharing**: Author controls who can decrypt
- 🌐 **Decentralized**: No single point of content control

---

## Getting Started

```bash
# Clone repository
git clone https://github.com/chomplicit/CipherBlog
cd CipherBlog

# Install dependencies
npm install

# Setup environment
cp .env.example .env.local
# Configure your settings

# Deploy contracts
npm run deploy:sepolia

# Start application
npm run dev
```

**Requirements**: MetaMask, Sepolia ETH, Node.js 18+

---

## How Private Blogging Works

### Publishing Flow

1. **Encrypt Post**: Your blog post encrypted with FHE before publishing
2. **Submit Encrypted**: Encrypted content submitted to blockchain
3. **FHEVM Storage**: Smart contract stores encrypted post
4. **Encrypted Retrieval**: Posts retrieved without decryption
5. **Private Reading**: Only authorized readers can decrypt
6. **Verifiable**: Publication timestamp verifiable without revealing content

### Privacy Model

| Aspect | Traditional Blog | CipherBlog |
|-------|-----------------|------------|
| **Storage** | Plaintext on servers | Encrypted on blockchain |
| **Processing** | Content analyzed | Encrypted processing |
| **Search** | Indexed content | Encrypted search |
| **Access** | Server can read | Only author/readers read |
| **Control** | Platform control | Author sovereignty |

---

## Technology Architecture

### Core Stack

| Component | Technology | Purpose |
|-----------|-----------|---------|
| **Encryption** | Zama FHE | Fully homomorphic encryption |
| **Blockchain** | Ethereum Sepolia | Decentralized post storage |
| **Smart Contracts** | Solidity + FHEVM | Encrypted blog operations |
| **Frontend** | React + TypeScript | Blog interface |
| **Build Tool** | Hardhat | Development environment |

### Zama FHEVM Integration

- **Post Encryption**: FHE encryption before publishing
- **Encrypted Storage**: Blog posts stored encrypted on blockchain
- **Privacy-Preserving**: No content visibility to platform
- **Verifiable Publishing**: Transparent publication timestamps

---

## Use Cases

### Personal Blogging

- Private diary entries
- Confidential personal thoughts
- Encrypted journal writing
- Secure personal documentation

### Professional Content

- Confidential business blogs
- Secure corporate documentation
- Private team blogs
- Encrypted professional content

### Academic Publishing

- Confidential research notes
- Private academic journals
- Encrypted research documentation
- Secure knowledge sharing

---

## Development

### Building

```bash
npm run build:contracts    # Build smart contracts
npm run build:frontend     # Build frontend
npm run build              # Build all components
```

### Testing

```bash
npm test                   # Run all tests
npm run test:contracts     # Contract tests only
npm run test:frontend      # Frontend tests only
```

### Deployment

```bash
npm run deploy:sepolia     # Deploy to Sepolia testnet
npm run deploy:local       # Deploy to local network
```

---

## Security & Privacy

### Privacy Guarantees

- 🔐 **Post Content**: Always encrypted, never decrypted by system
- 🔒 **Metadata Protection**: Minimal metadata exposure
- ✅ **Selective Access**: Author controls read permissions
- 🌐 **Decentralized Storage**: No centralized content storage

### Security Features

- **FHE Encryption**: Military-grade encryption for all posts
- **Zero-Knowledge Publishing**: Content processing without access
- **Blockchain Immutability**: Posts cannot be altered
- **Transparent Verification**: Publication proof without content reveal

### Best Practices

- 🔒 Use Sepolia testnet for development
- 🔒 Never commit private keys
- 🔒 Verify contract addresses before publishing
- 🔒 Use hardware wallets for production
- 🔒 Understand gas costs for FHE operations

---

## Contributing

Contributions welcome! Priority areas:

- 🔬 FHE performance optimization for blog content
- 🛡️ Security audits for publishing protocols
- 📖 Documentation improvements
- 🎨 UI/UX for blogging interface
- 🌐 Internationalization

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

---

## Resources

- **Zama**: [zama.ai](https://www.zama.ai/)
- **FHEVM Documentation**: [docs.zama.ai/fhevm](https://docs.zama.ai/fhevm)
- **Ethereum Sepolia**: [sepolia.etherscan.io](https://sepolia.etherscan.io/)

---

## License

MIT License - See [LICENSE](LICENSE) file for details.

---

## Acknowledgments

Built with [Zama FHEVM](https://github.com/zama-ai/fhevm) - Privacy-preserving blogging on blockchain.

---

**Repository**: https://github.com/chomplicit/CipherBlog  
**Issues**: https://github.com/chomplicit/CipherBlog/issues  
**Discussions**: https://github.com/chomplicit/CipherBlog/discussions

---

_Powered by Zama FHEVM | Private Blogging | Encrypted Content Publishing_
