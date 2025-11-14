# header-cli

A simple CLI utility for generating formatted text headers.

## 📦 Requirements

* Python >= 3.9

## 🛠 Usage

Run with a positional argument: 

```console
$ header-cli "Project Title"
################################ - PROJECT TITLE - #################################
```

Run with flags:
```console
$ header-cli -H "build complete" -s multi -c "=" -w 60
============================================================
= - BUILD COMPLETE - 
============================================================
```

### ⚙️ Options

`header-cli` supports the following flags:

| Flag | Description | Default |
|------|-------------|---------|
| `head` (positional) | Header text | — |
| `-H, --head` | Header text (alternative flag form) | — |
| `-s, --style` | Border style (`single`, `multi`) | `single` |
| `-c, --char` | Character to use for the border | `#` |
| `-w, --width` | Width of the rows | `84` |

## 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/your-username/utils.git
cd utils
```

### Unix

Make files executable:

```bash
chmod +x header-cli
```

Additionaly, you can copy any app to a location in your PATH:

```bash
cp header-cli ~/.local/bin/header-cli
```

### Windows

Copy `header-cli` to a location of your choice. Then, create a batch file to call it from the terminal:

e.g. `header-cli.bat`:
```cmd
@echo off
python C:\path\to\header-cli %*
```
Then, copy `header-cli.bat` to a location in your PATH.
