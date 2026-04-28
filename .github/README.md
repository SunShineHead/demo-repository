# OASIS

![CI](https://github.com/<your-user>/OASIS/actions/workflows/oasis-elite-ci.yml/badge.svg)

Production-grade Python project.

## Install

```bash
pip install -e .[dev]
Run
oasis
Test
pytest
Lint
ruff check .
black --check .
License

MIT


---

## File: `src/oasis/__init__.py`

```python
__version__ = "0.1.0"
File: src/oasis/cli.py
def main():
    print("OASIS is running.")
File: tests/test_cli.py
from oasis.cli import main


def test_main(capsys):
    main()
    captured = capsys.readouterr()
    assert "OASIS is running." in captured.out
