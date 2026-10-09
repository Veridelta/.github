<h1 align="center">
  <img src="https://veridelta.github.io/veridelta/assets/veridelta-symbol.png" alt="" height="64" align="middle">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://veridelta.github.io/veridelta/assets/veridelta-wordmark-dark.png">
    <img src="https://veridelta.github.io/veridelta/assets/veridelta-wordmark.png" alt="Veridelta" height="40" align="middle">
  </picture>
</h1>

Veridelta compares two datasets on their primary keys and reports every row that differs under the rules you declare. Nothing is forgiven unless a rule says so, and the exit code tells CI whether the datasets match.

[![A frame of the three-minute demo, with a play button. veridelta suggest proposes a rule for letter case, rounding, and missing notes, each with how many differing rows it explains.](https://raw.githubusercontent.com/Veridelta/veridelta-media/main/posters/demo-120-poster.png)](https://github.com/Veridelta/veridelta-media/releases/tag/demo-120)

[Watch the three-minute demo](https://github.com/Veridelta/veridelta-media/releases/tag/demo-120): Sam rewrites a nightly export of 40 accounts, Veridelta explains the noise with evidence, the one real defect fails his pull request, and the fixed export passes.

```bash
pip install veridelta
veridelta run legacy.csv modern.csv --key id
```

| Repository | What it holds |
| :--- | :--- |
| [veridelta](https://github.com/Veridelta/veridelta) | The Python package and command line, the GitHub Action, and the MCP server for agents. |
| [veridelta-media](https://github.com/Veridelta/veridelta-media) | The demo videos, made with Remotion from real terminal output. |

Veridelta is in alpha. Its tests run on generated data, with drift seeded on purpose, and nobody but its maintainer is known to have run it yet. [Status](https://veridelta.github.io/veridelta/#status) says more. Issues and discussions are welcome.

[Docs](https://veridelta.github.io/veridelta/) · [PyPI](https://pypi.org/project/veridelta/) · [Discussions](https://github.com/Veridelta/veridelta/discussions)
