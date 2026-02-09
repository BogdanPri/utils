# hfmt-cli

<p align="left">
  <img src="https://badges.fw-web.space/github/license/BogdanPri/header-cli?style=flat-square">
  <img src="https://badges.fw-web.space/github/languages/code-size/BogdanPri/header-cli?style=flat-square">
  <img alt="GitHub top language" src="https://badges.fw-web.space/github/languages/top/BogdanPri/header-cli?style=flat-square">
</p>

A simple CLI utility for generating formatted text headers.

## 📦 Requirements

* Python >= 3.9

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

* work in progress
