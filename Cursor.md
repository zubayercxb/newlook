# Newlook

Instructions for Cursor agents working in this repository.

## Project

Newlook is a new codebase. The workspace starts empty. Do not invent product features, frameworks, or folder structure unless the task asks for them. Once code exists, follow the patterns already in the tree.

## Working agreements

- Change only what the task requires.
- Match the naming, types, and structure of surrounding code.
- Do not add dependencies, config, or extra docs unless the task needs them.
- Prefer editing existing files over creating new ones.
- Keep functions and components focused. Name them for what they do.
- When a UI change is requested, verify the affected flow in the browser before calling it done.
- Do not commit, push, or open a pull request unless asked.

## Stack

- Language and runtime: JavaScript on Node.js. Do not add TypeScript, a web framework, or another runtime unless the task asks for it.
- Package manager: npm. Use `package.json` and `package-lock.json`. Do not switch to yarn, pnpm, or bun unless asked.
- Module system: ESM (`"type": "module"`). Use `import` / `export`. Match that style in every new file.
- App entry: `src/index.js` once the app exists. Keep `package.json` `"main"` and any `start` script pointed at that file.
- Scripts: `npm start` runs the app. `npm test` runs tests. Add a script only when the task needs it.
- Tests: Node.js built-in test runner (`node --test`). Colocate tests as `*.test.js` next to the module they cover.

## Conventions

Add project-specific rules below as the codebase grows. Keep each rule short and concrete.

- Prefer `async` / `await`. Reject or throw failures the caller can handle. Do not swallow errors.
- Use the `node:` prefix for built-in modules (`node:fs`, `node:path`).
- Read configuration from environment variables. Do not commit secrets or a filled-in `.env`.
