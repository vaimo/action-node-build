# GitHub Action for Node.js Build

This action is used to build Node.js projects.

**Author:** Patryk Waluś (patryk.walus@vaimo.com)

## Supported Versions

- **v1**
    - Build action for Node.js projects.

## Usage

```yaml
- name: Build Node.js Project
  uses: vaimo/action-node-build@v1
  with:
    # Environment variables as a string (Optional)
    # If specified, the action will create a .env file in the project root.
    env-vars: ${{ secrets.ENV_VARS }}
```
