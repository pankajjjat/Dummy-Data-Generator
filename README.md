# Dummy Payload Forge 🛠️

> Ultra-flexible dummy data generator for stress testing, filesystem benchmarking, backup tools, indexing engines, and automation pipelines.

Dummy Payload Forge is a CLI tool that can create **thousands (or millions) of files** with customizable:

- total dataset size (MB/GB),
- file extensions,
- per-file size range,
- approximate file count.

Perfect for testing how your system behaves under **realistic, messy, file-heavy workloads**.

---

## ✨ Features

- ⚡ **Fast generation**
  - Uses `os.urandom` and single-shot writes optimized for many small files.
- 📂 **Single output folder**
  - Everything is created in one directory for easy cleanup and testing.
- 🧩 **Multiple file types**
  - Built-in support:
    - `txt`, `log`, `csv`, `json`, `xml`, `png`, `pdf`, `zip`
- 🎯 **Target size in MB/GB**
  - Define total dataset size via `--target-mb`  
  - Or pick from an interactive preset menu.
- 📊 **Approximate file count**
  - Use `--approx-files` and the tool auto-tunes size range around `target_mb / approx_files`.
- 🎛️ **Fine-grained control**
  - `--ext` → choose specific extensions.
  - `--min-size-kb` / `--max-size-kb` → global per-file size range.
- 🧪 **Dry-run mode**
  - Show plan & stats **without** touching the filesystem.
- 🎲 **Reproducible runs**
  - `--seed` → deterministic file size patterns (useful for benchmarks).
- 🖼️ **Demo screenshot**
  - See the CLI experience at a glance.

---

## 📸 Demo

Place your screenshot image in the repo (example: `assets/demo-cli.png`) and it will show up here:

![Dummy Payload Forge CLI Demo](assets/demo-cli.png)

> If you use a different path/file name, just update the image URL above.

---

## 📦 Requirements

- Python **3.8+**
- No external dependencies (standard library only).

---

## 🔧 Installation

Clone the repository:

```bash
git clone https://github.com/pankajjjat/Dummy-Data-Generator.git
cd Dummy-Data-Generator
