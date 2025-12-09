# Advanced Dummy Data Generator

A fast, flexible CLI tool to generate **lots of small dummy files** up to a target size (in MB).  
Useful for testing file systems, backup tools, storage performance, or any app that needs a large number of random files.

---

## Features

- 🚀 **Fast**: Uses `os.urandom` with single-shot writes for small files.
- 📁 **Single output folder**: All files are generated in one directory.
- 🧩 **Multiple file types**:
  - `txt, log, csv, json, xml, png, pdf, zip`
- 🎯 **Target size in MB**:
  - Provide `--target-mb` or use the interactive size menu.
- 📊 **Approximate file count**:
  - Use `--approx-files` and the script auto-tunes file size ranges around `target_mb / approx_files`.
- 🎛️ **Fine-grained control**:
  - `--ext` to pick specific extensions.
  - `--min-size-kb` / `--max-size-kb` to override global file size range.
- 🔍 **Dry-run mode**:
  - Compute and print stats **without actually creating files**.
- 🎲 **Reproducible runs**:
  - `--seed` to fix the random generator seed.

---

## Requirements

- Python **3.8+**
- No external dependencies (only the Python standard library).

---

## Installation

Clone the repository:

```bash
git clone https://github.com/pankajjjat/Dummy-Data-Generator.git
cd Dummy-Data-Generator-main
