# Agent Instructions

## Project

- This is a single-page static site. The main source is [index.html](index.html); [logo.jpg](logo.jpg) is a local asset.
- Preserve the existing Indonesian copy, anchor-based navigation, inline Tailwind configuration, and vanilla JavaScript unless the task explicitly changes them.
- There is no package manager, build step, or automated test suite. Validate changes by opening `index.html` in a browser and checking the affected interaction in the console when relevant.

## Windows Credentials

- Never place passwords, API keys, access tokens, connection strings, or private certificates in `index.html`, client-side JavaScript, committed files, or URLs.
- Treat every value shipped to the browser as public. Frontend code may reference public endpoints, but authentication and privileged operations belong behind a server-side boundary.
- For local Windows tooling, prefer Windows Credential Manager, PowerShell SecretManagement, or environment variables supplied outside the repository. Do not print secrets in commands, logs, screenshots, or error messages.
- If a task requires a credential, ask the user to provide it through their secure local setup; do not ask them to paste it into a source file or chat.
- Do not commit `.env` files or generated credential stores. If local configuration becomes necessary, add an example file containing placeholders and document the required variable names without real values.

## Changes

- Keep edits focused and preserve the existing visual language and responsive behavior.
- Use relative asset paths and avoid introducing a framework or dependency for a small static-site change.