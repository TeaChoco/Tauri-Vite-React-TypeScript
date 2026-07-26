# Tauri + React + Typescript

This template should help get you started developing with Tauri, React and Typescript in Vite.

## Recommended IDE Setup

- [VS Code](https://code.visualstudio.com/) + [Tauri](https://marketplace.visualstudio.com/items?itemName=tauri-apps.tauri-vscode) + [rust-analyzer](https://marketplace.visualstudio.com/items?itemName=rust-lang.rust-analyzer)

---

### Windows
```sh
docker run --rm -v $(pwd):/app -w /app nailyudha/tauri:latest \
  bash -c "bun tauri build --runner cargo-xwin --target x86_64-pc-windows-msvc"
```

### Android
```sh
docker run --rm -v $(pwd):/app -w /app nailyudha/tauri:latest \
  bash -c "bun tauri android init && bun tauri android build --apk"
```

### Linux
```sh
docker run --rm -v $(pwd):/app -w /app nailyudha/tauri:latest \
  bash -c "bun i && bun tauri build"
```
