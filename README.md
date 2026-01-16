# Multiline String Editor

Easily edit multiline strings that need to be encoded as single-line strings (for example, JSON strings that contain literal `\n` characters).

## How to Use

![how_to_use](./assets/how_to_use.gif)

1. Move caret to the target string.

![caret_on_target](./assets/caret_on_target.png)

2. Open command palette and select `Edit as multiline string`.

3. Edit opened `multiline.txt`.

## Developing

1. Clone the repo

```
git clone <this repository>
cd <this directory>
```

2. Requires Node.js >= 24 and npm. Install on your machine or use the Brewfile as described below:

```
brew bundle # ensures Node is installed
brew bundle sh # opens subshell with node, npm, etc. on $PATH
```

3. Install dependencies (just typescript and vscode)

```
npm install
```

4. Run the VS Code command `Debug: Start Debugging` on `src/extension.ts`. This will start a development window with the extension active.

5. You can refresh the development window (from within the development window) with `Cmd + Shift + P` -> `Developer: Reload Window`.

## Packaging

1. After installing dependencies, run:

```
npm run package
```

## Installing

1. After packaging, run:

```
code --install-extension ./multiline-string-editor-*.vsix
```
