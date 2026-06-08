# Contributing to DisasterAlert

Thank you for your interest in contributing! We welcome all forms of contributions—code, documentation, bug reports, and feature ideas.

---

## 🤲 Ways to Contribute

### 1. **Report Bugs**
Found an issue? Open a [bug report](https://github.com/yourusername/disaster-alert/issues/new?template=bug_report.md) with:
- Clear description of the problem
- Steps to reproduce
- Expected vs. actual behavior
- Python version & environment details

### 2. **Suggest Enhancements**
Have an idea? Open a [feature request](https://github.com/yourusername/disaster-alert/issues/new?template=feature_request.md) with:
- Clear description of the feature
- Use case & motivation
- Potential implementation approach

### 3. **Improve Documentation**
- Fix typos in README or docstrings
- Add usage examples
- Clarify complex sections
- Create tutorials

### 4. **Submit Code**
Implement fixes or new features (see [Development Setup](#development-setup) below)

### 5. **Improve Models**
- Experiment with new architectures (transformers, ensemble methods)
- Optimize hyperparameters
- Add cross-validation improvements
- Benchmark against new datasets

---

## 🛠️ Development Setup

### 1. Fork & Clone
```bash
git clone https://github.com/yourusername/disaster-alert.git
cd disaster-alert
```

### 2. Create a Feature Branch
```bash
git checkout -b feature/your-feature-name
```

Use descriptive names like:
- `feature/bert-integration`
- `fix/preprocessing-bug`
- `docs/api-examples`

### 3. Set Up Environment
```bash
python -m venv venv
source venv/bin/activate  # macOS/Linux
# or
venv\Scripts\activate     # Windows

pip install -r requirements.txt
pip install pytest black flake8  # Development tools
```

### 4. Make Changes
- Follow PEP 8 style guidelines
- Write clear, documented code
- Add comments for complex logic
- Test your changes locally

### 5. Format & Lint (Optional but Recommended)
```bash
black notebooks/nlp_disaster_tweet_classification.ipynb
flake8 --max-line-length=100
```

### 6. Test Your Code
```bash
pytest  # If unit tests are present
# Or manually run notebook cells
```

### 7. Commit & Push
```bash
git add .
git commit -m "Clear, descriptive commit message"
git push origin feature/your-feature-name
```

### 8. Open a Pull Request
- Provide a clear title and description
- Link related issues (`Fixes #123`)
- Describe the changes and why they matter
- Include before/after performance metrics if applicable

---

## 📋 Contribution Guidelines

### Code Style
- **Python:** Follow [PEP 8](https://www.python.org/dev/peps/pep-0008/)
- **Naming:** Use snake_case for functions/variables, PascalCase for classes
- **Docstrings:** Use clear, concise docstrings following NumPy style

Example:
```python
def preprocess_text(text, remove_urls=True):
    """
    Clean and tokenize tweet text.
    
    Parameters
    ----------
    text : str
        Raw tweet text
    remove_urls : bool, optional
        Whether to remove URLs (default=True)
    
    Returns
    -------
    str
        Cleaned, tokenized text
    """
    # Implementation here
    pass
```

### Commit Messages
- Start with a verb: "Add," "Fix," "Improve," "Update," "Remove"
- Keep subject line under 50 characters
- Provide detailed explanation in body (if needed)

Examples:
- ✅ `Add BERT tokenizer for improved performance`
- ✅ `Fix file path issue in preprocessing pipeline`
- ❌ `update code`
- ❌ `Changes`

### Pull Request Checklist
- [ ] Code follows project style guidelines
- [ ] Documentation is clear and complete
- [ ] No new warnings or errors introduced
- [ ] Changes are tested locally
- [ ] Commit history is clean (no merge commits)
- [ ] Related issues are linked

---

## 🎯 Priority Areas

We're especially interested in contributions for:

1. **Transformer Integration** — Add BERT/RoBERTa models
2. **Multi-language Support** — Extend beyond English tweets
3. **API Service** — FastAPI wrapper for production deployment
4. **Real-time Streaming** — Integration with Kafka/streaming pipelines
5. **Dashboard** — Web UI for monitoring model performance
6. **Unit Tests** — Improve test coverage (especially preprocessing)

---

## 📚 Resources

- [Kaggle Competition](https://www.kaggle.com/competitions/nlp-getting-started)
- [NLTK Documentation](https://www.nltk.org/)
- [scikit-learn Guide](https://scikit-learn.org/stable/)
- [Git Workflow Guide](https://guides.github.com/introduction/flow/)

---

## ❓ Questions?

- **Documentation:** Check the [README](README.md) first
- **Issues:** Search [existing issues](https://github.com/yourusername/disaster-alert/issues)
- **Discussions:** Open a [discussion](https://github.com/yourusername/disaster-alert/discussions) for ideas
- **Contact:** Reach out via email or GitHub

---

## 🎉 Thank You!

Every contribution—no matter how small—makes DisasterAlert better. We appreciate your time and effort!

Happy coding! 🚨✨
