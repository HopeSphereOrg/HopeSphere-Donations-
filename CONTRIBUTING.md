# Contributing to HopeSphere Donations

Thank you for your interest in contributing to the HopeSphere Donations project! Please follow these guidelines to ensure a smooth workflow.

## ⚙️ Prerequisites
Before contributing, ensure you have the following installed:
- **Node.js** >= 16
- **npm** or **yarn**
- **Git**
- **Payment API keys** (for testing, stored securely in environment variables)

## 🛠 Setting Up the Project
1. **Fork the repository** (Click the "Fork" button on GitHub).
2. **Clone your fork** to your local machine:
   ```bash
   git clone https://github.com/YourUsername/HopeSphere-Donations.git
   ```
   Navigate into the project folder:
   ```bash
   cd HopeSphere-Donations
   ```
3. **Install Dependencies**
   Using npm:
   ```bash
   npm install
   ```
   Using yarn:
   ```bash
   yarn install
   ```

## 💳 Handling Donations
### Supported Payment Methods
- Stripe
- PayPal
- Cryptocurrency wallets (BTC, ETH, USDT)

### Processing Donations
- All donations must be recorded in the transaction logs.
- New payment providers must be reviewed for security and compliance before integration.
- Refund policies should follow platform standards and be documented.

### Reporting Donations
- If applicable, a public donation report should be updated periodically.
- Internal logs must store transaction IDs, amounts, and timestamps but should never store sensitive payment details.

## 🔒 Security Guidelines
### Payment Security Measures
- Use **secure API storage**: Payment API keys must be stored in `.env` files and never pushed to repositories.
- Follow **PCI DSS compliance**: Ensure adherence to security standards for handling payment transactions.
- Implement **fraud detection**: Limit excessive donation attempts and flag suspicious transactions.
- All transactions must be processed over **HTTPS with TLS 1.2+ encryption**.

## 📜 Code Standards for Financial Transactions
- Ensure **proper error handling** in payment flows.
- Maintain **comprehensive logging** without storing sensitive data.
- Transactions must be **atomic** to prevent incomplete donations.
- Implement **unit tests** to validate payment flows before deployment.

## 🌱 Creating a New Branch
Always create a separate branch for your feature or bug fix:
```bash
git checkout -b feature-name
```

## 🚀 Pushing Changes
Push your branch to GitHub:
```bash
git push origin feature-name
```
Then go to GitHub and open a Pull Request (PR) to merge your changes.

## 🎨 Code Style & Formatting
Follow ESLint and Prettier rules. Run linters before committing:
```bash
npm run lint
```

## 📌 Commit Message Format
Use the Conventional Commits format:
```bash
git commit -m "feat: add donation tracking feature"
```
Examples:
- ✅ `feat: integrate PayPal API`
- ✅ `fix: resolve incorrect transaction logging`
- ✅ `chore: update dependencies`

## 🤝 Contribution Guidelines
✔️ Open an issue before starting work on a feature.
✔️ Assign yourself to an issue to prevent duplicate work.
✔️ Keep PRs small and focused on a single feature or fix.
✔️ Follow the code review process before merging.

## 🏆 Contributor Recognition
We appreciate all contributions! Top contributors will be featured in the Hall of Fame and get early access to new features.

## ❓ Need Help?
If you have any questions, feel free to reach out via:
- GitHub Discussions
- Discord Community
- Email: hopesphere@proton.me

