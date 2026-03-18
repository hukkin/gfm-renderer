# gfm-renderer

[![PyPI version](https://img.shields.io/pypi/v/gfm-renderer.svg)](https://pypi.org/project/gfm-renderer/)
[![License](https://img.shields.io/pypi/l/gfm-renderer.svg)](https://github.com/hukkin/gfm-renderer/blob/master/LICENSE)

A Python library for rendering GitHub Flavored Markdown (GFM) with proper line break handling.

## Features

- **Proper line break rendering**: Handles soft line breaks in paragraphs and list items correctly
- **GitHub Flavored Markdown support**: Full compatibility with GFM syntax
- **Task list support**: Renders checkboxes in task lists

## Installation

```bash
pip install gfm-renderer
```

## Usage

```python
from gfm_renderer import render

markdown_text = """
First line, first,
second line.

- First line, first,
  second line.

---

- [ ] First line, first,
  second line.
"""

html_output = render(markdown_text)
print(html_output)
```

## Examples

### Soft Line Breaks in Paragraphs

**Input:**
```markdown
First line, first,
second line.
```

**Output:** Renders as a single paragraph with proper line break handling.

### Soft Line Breaks in Lists

**Input:**
```markdown
- First line, first,
  second line.
```

**Output:** Renders as a single list item with proper line break handling.

### Task Lists

**Input:**
```markdown
- [ ] First line, first,
  second line.
```

**Output:** Renders as an unchecked task list item with proper line break handling.

## License

MIT License. See [LICENSE](LICENSE) for details.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
