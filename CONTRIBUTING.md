# Contributing to dircontextgen 🛠️

We love your input! Whether you're squashing bugs 🐛, suggesting features 💡, or improving docs 📚, here's how to get involved:

## Development Process 🌱

1. **Fork & Branch**  
   ```bash
   git clone https://github.com/your-username/dircontextgen.git
   git checkout -b fix/that-annoying-bug
   ```

2. **Code Safely**  
   - Test changes with `pytest -v` (see test data in `tests/test_data/`)
   - Mark slow tests with `@pytest.mark.slow`
   - Keep that coverage at 100% for new code 🔒

3. **Quality Checks**  
   ```bash
   black .  # Auto-formatting
   mypy .   # Type checking
   pylint dircontextgen/  # Code smells
   ```

4. **Open PR** - We'll review faster than Claude reads your docs! 🚀

## Hot Dev Tips 🔥

### Environment Setup
```bash
# 1. Clone and enter
git clone https://github.com/yourusername/dircontextgen.git
cd dircontextgen

# 2. Magic environment
python -m venv venv
source venv/bin/activate  # venv\Scripts\activate on Windows

# 3. Install with extras
pip install -e ".[dev]"
pre-commit install  # Auto-format on commit!
```

### Project Map 🗺️
```
dircontextgen/
├── core.py          # Brain of the operation
├── cli.py           # Fancy command-line interface
└── utils/
    ├── file_handling.py  # Knows binaries from texts
    ├── ignore_patterns.py # .gitignore whisperer
    └── tree_generation.py # Makes pretty folder trees
```

## Code Culture 💻
- **Type Everything** - Even your coffee orders ☕ (Python 3.7+)
- **Black Rules** - 88 chars, no exceptions!
- **Test Like Mad** - If it moves, test it. If it doesn't, test why.

## Bug Reports 🐞
Good reports include:
1. What you did (`dircontextgen --tree-only ./project`)
2. What happened ("Included node_modules 😱")
3. What should've happened ("Respect .gitignore plz")

Pro tip: Run with `--verbose` and include the output!

---

**License Note**: All contributions fall under [Apache 2.0](LICENSE) - same friendly terms as before!