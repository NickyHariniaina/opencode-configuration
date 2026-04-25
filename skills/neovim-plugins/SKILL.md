---
name: neovim-plugin
description: Create and maintain Neovim plugins using Lua with clean, modular design
license: MIT
compatibility: opencode
metadata:
  audience: developers
  workflow: neovim
---

## What I do

* Create Neovim plugins using Lua
* Structure plugins with clean, modular architecture
* Define commands, keymaps, and autocommands
* Integrate with Neovim APIs (`vim.api`, `vim.fn`, etc.)
* Debug and improve existing plugins
* Ensure compatibility with modern Neovim (0.9+)

## When to use me

Use this when building or modifying a Neovim plugin in Lua.

Ask clarifying questions if:

* The plugin manager is unclear (lazy.nvim, packer, etc.)
* The plugin scope or purpose is not well defined
* There are specific performance or UX constraints

## How I behave

* Prefer simple, minimal, and fast implementations
* Follow Lua best practices and idiomatic Neovim patterns
* Keep modules small and reusable
* Avoid unnecessary dependencies
* Do not explain unless asked—focus on implementation

## Common tasks

### Plugin structure

* Use a clean layout:
  * `lua/myplugin/init.lua`
  * `lua/myplugin/config.lua`
  * `lua/myplugin/commands.lua`
* Separate logic into modules

### Commands

* Create user commands with `vim.api.nvim_create_user_command`
* Keep commands focused and predictable

### Keymaps

* Use `vim.keymap.set`
* Support buffer-local mappings when needed

### Autocommands

* Use `vim.api.nvim_create_autocmd`
* Group with augroups for clarity

### Configuration

* Provide a `setup()` function
* Allow user overrides with defaults

### Performance

* Lazy-load when possible
* Avoid blocking operations
* Minimize startup impact

## Output format

* Provide ready-to-use Lua code
* Use modular structure (multiple files if needed)
* Keep snippets concise and copy-pasteable

## Safety checks

* Do not break Neovim API compatibility
* Avoid global state pollution
* Ensure plugin can be safely required
* Prevent unnecessary performance overhead

## Example prompts

* "Create a Neovim plugin that toggles a terminal"
* "Add a command to this plugin"
* "Refactor this plugin to be modular"
* "Convert this Vimscript plugin to Lua"
* "Add lazy loading to this plugin"

---
