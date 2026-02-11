# hfmt-cli

A simple CLI utility for generating formatted text headers with borders and boxes.

<p align="center">
  <a href="https://github.com/BogdanPri/hfmt-cli/raw/main/hfmt_demo.gif">
    <img src="https://github.com/BogdanPri/hfmt-cli/blob/87c8a5ae43697cad9d350d6cf7240f50816a71ff/hfmt_demo.gif"/>
  </a>
</p>

<p align="center">
  <a href="https://pypi.org/project/hfmt-cli/"><img src="https://badge.fury.io/py/hfmt-cli.svg" alt="PyPI version"></a>
  <a href="https://opensource.org/license/BSD-3-Clause"><img src="https://badges.fw-web.space/github/license/BogdanPri/hfmt-cli"></a>
  <a href="https://github.com/BogdanPri/hfmt-cli"><img src="https://img.shields.io/badge/github-hfmt&hyphen;cli-blue?logo=github"></a>
  <img src="https://badges.fw-web.space/github/languages/code-size/BogdanPri/hfmt-cli">
  <!-- <img alt="GitHub top language" src="https://badges.fw-web.space/github/languages/top/BogdanPri/hfmt-cli"> -->
</p>

## 📦 Requirements

* Python ≥ 3.9

## 🛠 Usage

Run with a positional argument: 

```console
$ hfmt "project title"
################################## project title ###################################
```


Run with flags:
```console
$ hfmt --head "build complete" --style multi --char "=" --width 60 --upper --align left
============================================================
= BUILD COMPLETE 
============================================================
```

```console
$ hfmt --border-only --width 50
##################################################
```

Run with box mode:
```console
$ hfmt --title --width auto --box double "welcome back"
╔══════════════╗
║ Welcome Back ║
╚══════════════╝
```

### ⚙️ Options

`hfmt-cli` supports the following value flags:

| Flag | Description | Default |
|------|-------------|---------|
| `head` (positional) | Header text | — |
| `-H, --head` | Header text (alternative flag form) | — |
| `-s, --style` | Border style (`single`, `multi`) | `single` |
| `-c, --char` | Character to use for the border | `#` |
| `-w, --width` | Width of the rows | `84` or `auto` |
| `-a, --align` | Header justification | `center` or `left` |
| `-b, --box` | Surround header by a box (overrides other flags) | `none` |

`hfmt-cli` supports the following value toggles:

| Toggle | Description |
|--------|-------------|
| `-U, --upper` | Converts header to "UPPER_CASE" |
| `-L, --lower` | Converts header to "lower_case" |
| `-T, --title` | Converts header to "Title_Case" |
| `-S, --swapcase` | Converts header to "sWAP_cASE" |
| `--border-only` | Returns only a border of characters with no header |

## 🚀 Installation

Install via [`pipx`](https://github.com/pypa/pipx) (recommended)
```console
pipx install hfmt-cli
```

Install via `pip`:
```console
pip install hfmt-cli
```
