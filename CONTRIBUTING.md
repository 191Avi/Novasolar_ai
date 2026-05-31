# 🤝 Contributing to NovaSolar AI

<div align="center">

![Contributors Welcome](https://img.shields.io/badge/Contributors-Welcome-brightgreen?style=for-the-badge&logo=github)
![Open Source](https://img.shields.io/badge/Open%20Source-Love-red?style=for-the-badge&logo=opensourceinitiative)
![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-blue?style=for-the-badge&logo=git)

**Thank you for your interest in contributing to NovaSolar AI!**
Every contribution — big or small — helps push the boundaries of AI in renewable energy. 🌍

</div>

---

## 📋 Table of Contents

- [Code of Conduct](#-code-of-conduct)
- [How Can I Contribute?](#-how-can-i-contribute)
- [Getting Started](#-getting-started)
- [Development Workflow](#-development-workflow)
- [Pull Request Process](#-pull-request-process)
- [Style Guidelines](#-style-guidelines)
- [Areas We Need Help With](#-areas-we-need-help-with)
- [Community](#-community)

---

## 📜 Code of Conduct

This project follows a simple principle: **be kind, be constructive, be collaborative**.

- Respect all contributors regardless of experience level
- Give constructive feedback, not criticism
- Focus on what's best for the project and the planet 🌱
- Help newcomers feel welcome

---

## 💡 How Can I Contribute?

### 🐛 Reporting Bugs
Found something broken? Please [open an issue](https://github.com/191Avi/Novasolar_ai/issues/new) with:
- A clear title and description
- Steps to reproduce the bug
- Expected vs actual behavior
- Screenshots if applicable
- Your environment (OS, Python version, etc.)

### 🌟 Suggesting Features
Have an idea? [Open a feature request](https://github.com/191Avi/Novasolar_ai/issues/new) with:
- A clear description of the feature
- Why it would benefit the project
- Any relevant examples or references

### 🔧 Code Contributions
- Fix bugs from the [issues list](https://github.com/191Avi/Novasolar_ai/issues)
- Implement new features
- Improve model accuracy
- Add tests and documentation
- Refactor existing code

### 📚 Non-Code Contributions
You don't need to write code to contribute!
- Improve documentation
- Write tutorials or blog posts about NovaSolar AI
- Share the project on social media
- Star the repo ⭐
- Report bugs and suggest improvements

---

## 🚀 Getting Started

### 1. Fork & Clone

```bash
# Fork the repo on GitHub, then:
git clone https://github.YOUR_USERNAME/Novasolar_ai.git
cd Novasolar_ai
```

### 2. Set Up Development Environment

```bash
# Create a virtual environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Install development dependencies
pip install -r requirements-dev.txt  # if available
```

### 3. Create a Branch

```bash
# Always branch from main
git checkout main
git pull origin main
git checkout -b feature/your-feature-name
# or
git checkout -b fix/bug-description
```

---

## 🔄 Development Workflow

### Branch Naming Convention

| Type | Format | Example |
|------|--------|---------|
| Feature | `feature/description` | `feature/lstm-optimization` |
| Bug Fix | `fix/description` | `fix/data-pipeline-error` |
| Documentation | `docs/description` | `docs/update-api-guide` |
| Research | `research/description` | `research/transformer-model` |
| Refactor | `refactor/description` | `refactor/model-training` |

### Commit Message Format

We follow [Conventional Commits](https://www.conventionalcommits.org/):

```
type(scope): short description

[optional body]
[optional footer]
```

**Types:**
- `feat` — New feature
- `fix` — Bug fix
- `docs` — Documentation changes
- `style` — Code style changes (formatting, etc.)
- `refactor` — Code refactoring
- `test` — Adding or updating tests
- `chore` — Build process or auxiliary tool changes
- `research` — Research experiments and results

**Examples:**
```bash
git commit -m "feat(forecasting): add 48-hour prediction window to LSTM model"
git commit -m "fix(iot): resolve MQTT connection timeout on Raspberry Pi"
git commit -m "docs(readme): add installation troubleshooting section"
git commit -m "research(models): benchmark Transformer vs LSTM accuracy"
```

---

## 📝 Pull Request Process

1. **Ensure your branch is up to date** with `main`
   ```bash
      git fetch origin
         git rebase origin/main
            ```

            2. **Run tests** before submitting (when test suite is available)
               ```bash
                  python -m pytest tests/
                     ```

                     3. **Update documentation** if your changes affect how the system works

                     4. **Fill out the PR template** completely

                     5. **Link related issues** in your PR description using `Closes #123`

                     6. **Wait for review** — maintainer will review within 48-72 hours

                     7. **Address feedback** — make requested changes and push to the same branch

                     ### PR Checklist
                     - [ ] My code follows the project's style guidelines
                     - [ ] I have commented my code where necessary
                     - [ ] I have updated relevant documentation
                     - [ ] My changes don't break existing functionality
                     - [ ] I have tested my changes locally

                     ---

                     ## 🎨 Style Guidelines

                     ### Python Code Style
                     - Follow [PEP 8](https://pep8.org/) conventions
                     - Use meaningful variable and function names
                     - Maximum line length: **100 characters**
                     - Use type hints where possible
                     - Add docstrings to all functions and classes

                     ```python
                     def predict_solar_output(
                         irradiance_data: np.ndarray,
                             temperature: float,
                                 horizon_hours: int = 24
                                 ) -> np.ndarray:
                                     """
                                         Predict solar energy output using LSTM model.

                                             Args:
                                                     irradiance_data: Historical solar irradiance readings (W/m²)
                                                             temperature: Current ambient temperature (°C)
                                                                     horizon_hours: Prediction horizon in hours (default: 24)

                                                                         Returns:
                                                                                 np.ndarray: Predicted energy output in kWh
                                                                                     """
                                                                                         # implementation here
                                                                                         ```

                                                                                         ### Machine Learning Guidelines
                                                                                         - Document model architecture clearly
                                                                                         - Log all experiments with MLflow or similar
                                                                                         - Save model checkpoints regularly
                                                                                         - Always validate on a held-out test set
                                                                                         - Report standard metrics: MAE, RMSE, R², MAPE

                                                                                         ---

                                                                                         ## 🌍 Areas We Need Help With

                                                                                         We especially welcome contributions in these areas:

                                                                                         | Area | Skills Needed | Priority |
                                                                                         |------|---------------|----------|
                                                                                         | 🤖 **LSTM Model Optimization** | Python, TensorFlow/PyTorch | 🔴 High |
                                                                                         | 📡 **IoT Data Pipeline** | MQTT, Raspberry Pi, Python | 🔴 High |
                                                                                         | 🛠️ **Predictive Maintenance AI** | ML, Anomaly Detection | 🔴 High |
                                                                                         | 📊 **Dashboard UI** | React/Vue, D3.js, CSS | 🟡 Medium |
                                                                                         | 🧪 **Unit Tests** | pytest, unittest | 🟡 Medium |
                                                                                         | 📚 **Documentation** | Technical Writing | 🟢 Always Open |
                                                                                         | 🌐 **Translations** | Any Language | 🟢 Always Open |
                                                                                         | 🔬 **Research Review** | ML, Energy Systems | 🟢 Always Open |

                                                                                         ---

                                                                                         ## 💬 Community

                                                                                         Have questions? Want to discuss ideas?

                                                                                         - 📧 **Email**: [avijitsahaa236@gmail.com](mailto:avijitsahaa236@gmail.com)
                                                                                         - 🐛 **Issues**: [GitHub Issues](https://github.com/191Avi/Novasolar_ai/issues)
                                                                                         - 🌐 **LinkedIn**: [Avijit Saha Apu](https://linkedin.com/in/avijitsahaapu)

                                                                                         ---

                                                                                         ## 🙏 Recognition

                                                                                         All contributors will be:
                                                                                         - Listed in the **Contributors** section of the README
                                                                                         - Credited in release notes
                                                                                         - Mentioned in any related research papers (for significant technical contributions)

                                                                                         <div align="center">

                                                                                         **Thank you for helping make solar energy smarter! ☀️🤖**

                                                                                         *Every star, every fork, every PR brings us closer to a sustainable energy future.*

                                                                                         </div>
