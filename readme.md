# Dainty – Panda Theme

Twenty-five variations of Panda Theme with adjusted chroma and lightness levels.

## Provenance and attribution

This repository is a local, maintained distribution of
[Alexander Te's `dainty-panda-theme-vscode`](https://github.com/alexanderte/dainty-panda-theme-vscode).
The original Panda Theme was created by Alexander Te. The theme was imported
into [Dainty for Visual Studio Code](https://dainty.site/vscode), processed in
the Lab color space, and exported into these variations. This project does not
claim authorship of the original theme, source package, or color processing.

## Screenshots

### Dainty – Panda Theme (chroma 2, lightness 3)

![Dainty – Panda Theme (chroma 2, lightness 3)](https://github.com/alexanderte/dainty-panda-theme-vscode/raw/master/assets/dainty-panda-theme-2-3.png)

### Dainty – Panda Theme (chroma 3, lightness 1)

![Dainty – Panda Theme (chroma 3, lightness 1)](https://github.com/alexanderte/dainty-panda-theme-vscode/raw/master/assets/dainty-panda-theme-3-1.png)

### Dainty – Panda Theme (chroma 4, lightness 0)

![Dainty – Panda Theme (chroma 4, lightness 0)](https://github.com/alexanderte/dainty-panda-theme-vscode/raw/master/assets/dainty-panda-theme-4-0.png)

## Install

The distributable VSIX is checked in at
`releases/dainty-panda-theme-vscode-1.0.2-local.1.vsix`. In Visual Studio Code
or Cursor, open the Extensions view, select **… → Install from VSIX…**, choose
that file, and reload when prompted. From a terminal, the equivalent command is
`code --install-extension releases/dainty-panda-theme-vscode-1.0.2-local.1.vsix`
(use `cursor --install-extension` for Cursor).

To rebuild the VSIX locally, install dependencies and run:

```sh
yarn install
npx --yes @vscode/vsce package --no-yarn --no-dependencies
```

Move the generated VSIX into `releases/` and use a versioned filename before
tagging a new local release. The `repository` URL in `package.json` identifies
the original upstream source; add a new remote explicitly before publishing
this local history.

## Local release

The first local snapshot is tagged `v1.0.2-local.1`. Tags and checked-in VSIX
files provide a reproducible installation source even when no hosting remote
is configured. When publishing, choose the destination account and remote
explicitly, then push the branch and tag and attach the VSIX to the release.

## Included variations

### Chroma

| Value | `_all.chroma` |
| ----- | ------------- |
| 0     | -10           |
| 1     | -5            |
| 2     | 0             |
| 3     | 5             |
| 4     | 10            |

### Lightness

| Value | `_all.lightnessStart` |
| ----- | --------------------- |
| 0     | -15                   |
| 1     | -10                   |
| 2     | -5                    |
| 3     | 0                     |
| 4     | 5                     |
