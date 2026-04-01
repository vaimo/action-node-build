# GitHub Action for Node.js Build

This action is used to build Node.js projects.

**Author:** Patryk Walus (patryk.walus@vaimo.com)

## Supported Versions

- **v2**
    - Added configurable package manager support (npm, yarn, pnpm).
    - `package-manager` input is now required.
- **v1**
    - Build action for Node.js projects (yarn only).

## Usage

```yaml
- name: Build Node.js Project
  uses: vaimo/action-node-build@v2
  with:
    # Package manager to use. Supported values: npm, yarn, pnpm. (Required)
    package-manager: yarn

    # Environment variables as a string (Optional)
    # If specified, the action will create a .env file in the project root.
    env-vars: ${{ secrets.ENV_VARS }}
```
