# External assets for the D&D character-sheet typesetter

Files needed to build the in-browser typesetting of
[dnd-character-sheets](https://github.com/dnd-character-sheets/dnd-character-sheets.github.io)
that the build does not download from GitHub.  That repository's file
`in-browser/external-assets` names the commit of this repository that it
builds with, and its `in-browser/INSTALL.md` explains how to update it.

| Path | Contents | Source | SHA-256 |
|---|---|---|---|
| `lua-5.1.5.tar.gz` | Lua 5.1.5 | <https://www.lua.org/ftp/lua-5.1.5.tar.gz> | `2640fc56a795f29d28ef15e13c34a47e223960b0240e8cb0a82d9b0738695333` |
| `lyaml-6.2.9.tar.gz` | lyaml 6.2.9 | <https://github.com/gvvaughan/lyaml/archive/refs/tags/v6.2.9.tar.gz> | `515e81d21903c1e428b017f2fe9dffa4e29ae9881b0d49ddbe6ba625e3164fe3` |
| `texlive/` | the TeX Live files that the typesetter reads | TeX Live as packaged by Debian; `texlive/SOURCE` gives the version | — |

The tarballs are unmodified copies of their sources; Lua and lyaml are
distributed under the MIT license.  `texlive/` holds unmodified copies of
TeX Live files, laid out as in a TeX Live tree, each under its own
license (see the files themselves and <https://tug.org/texlive/copying.html>).
The main repository's `in-browser/refresh-texlive-snapshot` makes it.
