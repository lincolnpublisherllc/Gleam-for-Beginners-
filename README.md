README — Gleam Code Extract (Chapter-by-Chapter)
What this is

This repository contains code snippets extracted from “Gleam for Beginners: How to Harness the BEAM VM with a Type-Safe Language for Concurrent Systems.” Snippets are grouped by the chapter they came from. File names are ordered so you can follow along as you read. 

Gleam for Beginners

If you just want the files, download the zip:

gleam_code_extract.zip

A manifest.csv is included inside the zip. It lists every snippet with chapter, filename, language, line count, and source detection method.

Folder structure
gleam_code_extract/
  Chapter 01 .../         # one folder per chapter title as it appears in the book
    code_01.gleam
    code_02.gleam
    ...
  Chapter 02 .../
    code_01.gleam
    ...
  ...
  manifest.csv            # master index of all snippets

File naming

Files are named in reading order: code_01, code_02, and so on.

Default extension is .gleam. If a fenced block specified a language (for example ```python), the file uses the matching extension:

.py, .rs, .js, .ts, .ex, .exs, .erl, .toml, .yml, .json, .html, .sql, .sh, .md.

Requirements

Gleam and the BEAM toolchain

Install Gleam: see official docs or use Homebrew on macOS brew install gleam-lang/tap/gleam.

Install Erlang/OTP for BEAM.

Optional: VS Code with the Gleam extension for syntax highlighting and formatting.

How to run the samples

Most examples are short console programs.

Create a new Gleam project:

gleam new demo
cd demo


Drop one or more .gleam files from a chapter folder into src/ and fix module names if needed:

Rename the file to match the module, for example hello.gleam with pub fn main() inside.

Or update the first line to declare the module name that matches the file.

Run:

gleam run


If a snippet is a function only, import it from your main module and call it there. Some exercises include multiple functions in one file. Keep them together.

Using manifest.csv

Open manifest.csv to quickly locate a snippet:

chapter: where it was found

filename: exact file inside the chapter folder

language: detected language for the snippet

lines and bytes: quick size check

source: how it was detected (fenced, style/monospace, or table style/monospace)

Tip: Filter by chapter to gather all code used in that part of the book.

Conventions and notes

Snippets come directly from the book. Formatting is preserved where possible.

Some code blocks in books rely on surrounding context. If a snippet refers to a module or alias not shown in the same block, check earlier files in the same chapter.

If a chapter mixes languages, the extensions will reflect that. Only Gleam code will compile under Gleam.

If any file seems incomplete or you need combined files per chapter, say the word and I will stitch them together.

Known limitations

If a code block was embedded in special layout elements, spacing may need a quick tidy.

If a snippet relied on preceding definitions from prose rather than a visible block, you may need to add those helpers manually.

Attribution

All source text and code originate from the book cited above. This extract is for learning and reference by the book’s owner. Please follow the book’s license terms and the publisher’s policies. 

Gleam for Beginners
