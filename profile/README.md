<h1 align="center">
  <img src="https://veridelta.github.io/veridelta/assets/veridelta-symbol.png" alt="" height="64" align="middle">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://veridelta.github.io/veridelta/assets/veridelta-wordmark-dark.png">
    <img src="https://veridelta.github.io/veridelta/assets/veridelta-wordmark.png" alt="Veridelta" height="40" align="middle">
  </picture>
</h1>

Veridelta compares two datasets on their primary keys and reports every row that differs under the rules you declare. Nothing is forgiven unless a rule says so, and the exit code tells CI whether the datasets match.

![A terminal prints a five-line veridelta.yaml and two three-row CSV files, validates the configuration, runs the comparison, shows one added, one removed, and one changed row, and prints the exit code for CI, 1, beside what 0, 1, and 3 mean.](https://veridelta.github.io/veridelta/assets/demo.gif)

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
