# Multiline String Editor

Easily edit multiline strings that need to be encoded as single-line strings (for example, JSON strings that contain literal `\n` characters).

## How to Use

![how_to_use](./assets/how_to_use.gif)

1. Move caret to the target string.

![caret_on_target](./assets/caret_on_target.png)

2. Open command palette and select `Edit as multiline string`.

3. Edit opened `multiline.txt`.

## Developing

1. Clone the repository, and install its dependencies:

```
git clone <this repository>
cd <this directory>
bun install
```

2. Run the VS Code command `Debug: Start Debugging` on `src/extension.ts`. This will start a development window with the extension active.
3. You can refresh the development window (from within the development window) with `Cmd + Shift + P` -> `Developer: Reload Window`.

## Packaging

1. [Install `vsce`](https://code.visualstudio.com/api/working-with-extensions/publishing-extension#vsce).
2. Run `vsce package`.

See the [packaging documentation](https://code.visualstudio.com/api/working-with-extensions/publishing-extension#packaging-extensions) for more information.

You can then manually upload the packaged (`.vsix`) file to the VSCode Marketplace from https://marketplace.visualstudio.com/manage/publishers/<your-publisher>.
