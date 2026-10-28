# Terax AI

Tauri desktop app mixing a terminal, code editor, source control, web previews, and agent sessions in one window. Fork of [crynta/terax-ai](https://github.com/crynta/terax-ai), reshaped around Codex as a workspace tab with persistent sessions, editor and terminal context sharing, and a permission layer over system paths.

## What this fork adds

* Codex workspace tab instead of floating windows
* Agent sessions that persist across reloads
* Agents can read open editor buffers, terminal history, and file selections
* Permission prompts before agents touch system paths or credentials
* Inline media and localhost web previews

API keys (OpenAI and compatible providers) are entered in settings, kept in the OS keyring, and redacted from logs.

## Build

```bash
pnpm install
pnpm tauri dev
```

Bundles: `pnpm build:deb`, `pnpm build:appimage`. Needs Rust, Node/pnpm, and Tauri system deps.

## Note

Temporary fork to mess around with. I will not be maintaining it.

## License

Licensed under Apache-2.0. See the `LICENSE` file for more details.
