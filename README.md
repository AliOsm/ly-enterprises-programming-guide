# Libyan Enterprises Programming Guide

![GitHub](https://img.shields.io/github/license/aliosm/ly-enterprises-programming-guide?style=flat-square)

**Libyan Enterprises Programming Guide** is a unified guide for programming standards that crafted specially for Libyan
enterprises.

## Why Creating This Guide?

**TODO**

## Contribute

### Pre-requisites

**Libyan Enterprises Programming Guide** is written in [mdBook](https://github.com/rust-lang/mdBook),
though the following softwares are required:
- [Install](https://www.rust-lang.org/tools/install) Rust programming language and Cargo
- Install mdBook by running `cargo install mdbook`

**Note**: The previous steps tested on `Ubuntu 20.04` OS. A specific steps need to be added for other OSs.

### Overall Steps

1. Fork this repo
1. Clone the fork to your machine
1. Open an issue with the chapter/section you want to add/update
1. Agree on a general writing proposal
1. Create a new branch and commit your changes
1. Open a pull request linking to the issue

### Make Changes

#### Guide Configuration

All [mdBook configuration](https://rust-lang.github.io/mdBook/format/config.html) are available wihtin `book.toml` file.

#### Guide Content

The content of this guide is lies in `src` folder.
Each chapter has its own file named with its name and ends with `.md` extension (e.g `المقدمة.md`).
To edit any of the contents, you can edit the files in `src` folder directly.
mdBook uses Markdown, specifically [CommonMark](https://commonmark.org/) specification.
So, make sure to follow the mentioned specifications.

**Note**: The content of this guide it written in Arabic language. Why? Currently, I have two reasons:
- Remind the writer about why we are creating this guide.
- Make it easy for our audiences to understand and benefit from it.

#### Theme Style

The theme style is exists under `theme` folder.
It is the default mdBook theme except for the RTL support (review this [commit](https://github.com/AliOsm/ly-enterprises-programming-guide/commit/30d905338e0ae208ccb973d217845667a4a7364c)).
The RTL support needs to be revisited by an expert in future (maybe you ?.?)
and it could be contributed to mdBook repository directly in future after creating a mature enought RTL theme.

### Test Changes

Once you finish the changes on the configuration, content or the theme,
you can run `mdbook build -o` and the guide will open on your browser so you can review it before publishing new PRs.
For more information, review mdBook documentation from [here](https://rust-lang.github.io/mdBook/cli/index.html).
