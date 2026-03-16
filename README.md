# Neovim Keybinds Reference

This file is a quick reference for the keybinds that matter most in this config.

## First things first

- `<leader>` is `Space`
- After pressing `<leader>`, wait a moment and `which-key` will show available mappings
- Use `<leader>fk` to search keymaps from inside Neovim

## Daily drivers

| Key | What it does | Context |
| --- | --- | --- |
| `<leader>ff` | Find files | Normal |
| `<leader>fs` | Live grep in cwd | Normal |
| `<leader>fr` | Recent files | Normal |
| `<leader>fc` | Grep word under cursor | Normal |
| `<leader>ee` | Toggle file explorer | Normal |
| `<leader>ef` | Reveal current file in explorer | Normal |
| `gd` | Go to definition | LSP buffer |
| `gR` | Find references | LSP buffer |
| `K` | Hover docs | LSP buffer |
| `<leader>ca` | Code actions | LSP buffer |
| `<leader>rn` | Rename symbol | LSP buffer |
| `<leader>d` | Line diagnostics popup | LSP buffer |
| `[d` / `]d` | Previous or next diagnostic | LSP buffer |
| `<leader>mp` | Format file or selection | Normal / Visual |
| `<leader>l` | Trigger linting | Normal |
| `<leader>lg` | Open LazyGit | Normal |
| `<leader>wr` | Restore session for cwd | Normal |
| `<leader>ws` | Save session | Normal |

## Window and tab management

| Key | What it does |
| --- | --- |
| `<leader>sv` | Split vertically |
| `<leader>sh` | Split horizontally |
| `<leader>se` | Make splits equal size |
| `<leader>sx` | Close current split |
| `<leader>sm` | Maximize or restore current split |
| `<C-h>` | Move to left split or tmux pane |
| `<C-j>` | Move to split below or tmux pane |
| `<C-k>` | Move to split above or tmux pane |
| `<C-l>` | Move to right split or tmux pane |
| `<C-\>` | Jump to previous split or tmux pane |
| `<leader>to` | New tab |
| `<leader>tx` | Close current tab |
| `<leader>tn` | Next tab |
| `<leader>tp` | Previous tab |
| `<leader>tf` | Open current buffer in a new tab |

## File explorer

Global explorer keys:

| Key | What it does |
| --- | --- |
| `<leader>ee` | Toggle NvimTree |
| `<leader>ef` | Toggle explorer focused on current file |
| `<leader>ec` | Collapse explorer |
| `<leader>er` | Refresh explorer |

Inside NvimTree:

| Key | What it does |
| --- | --- |
| `<CR>` or `o` | Open file or directory |
| `<C-v>` | Open in vertical split |
| `<C-x>` | Open in horizontal split |
| `<C-t>` | Open in new tab |
| `a` | Create file or directory |
| `r` | Rename |
| `d` | Delete |
| `c` | Copy |
| `x` | Cut |
| `p` | Paste |
| `-` | Go to parent directory |
| `g?` | Show full NvimTree help |

## Search and picking

Global Telescope keys:

| Key | What it does |
| --- | --- |
| `<leader>ff` | Find files |
| `<leader>fr` | Recent files |
| `<leader>fs` | Search text in cwd |
| `<leader>fc` | Search word under cursor |
| `<leader>ft` | Find TODO comments |
| `<leader>fk` | Search available keymaps |

Inside Telescope:

| Key | What it does |
| --- | --- |
| `<C-j>` | Next result in insert mode |
| `<C-k>` | Previous result in insert mode |
| `<CR>` | Open selection |
| `<C-v>` | Open in vertical split |
| `<C-x>` | Open in horizontal split |
| `<C-q>` | Send selected results to quickfix and open Trouble |
| `<C-t>` | Open Telescope results in Trouble |
| `<C-/>` | Show picker mappings in insert mode |
| `?` | Show picker mappings in normal mode |

## LSP and diagnostics

These only exist after an LSP attaches to the current buffer.

| Key | What it does |
| --- | --- |
| `gd` | Go to definition |
| `gD` | Go to declaration |
| `gR` | Show references with Telescope |
| `gi` | Show implementations with Telescope |
| `gt` | Show type definitions with Telescope |
| `K` | Hover documentation |
| `<leader>ca` | Code action |
| `<leader>rn` | Rename symbol |
| `<leader>D` | Buffer diagnostics with Telescope |
| `<leader>d` | Line diagnostics float |
| `[d` | Previous diagnostic |
| `]d` | Next diagnostic |
| `<leader>rs` | Restart LSP |

## Trouble and TODOs

| Key | What it does |
| --- | --- |
| `<leader>xw` | Workspace diagnostics |
| `<leader>xd` | Document diagnostics |
| `<leader>xq` | Quickfix list |
| `<leader>xl` | Location list |
| `<leader>xt` | TODOs in Trouble |
| `]t` | Next TODO comment |
| `[t` | Previous TODO comment |
| `<leader>ft` | TODOs in Telescope |

Inside Trouble, press `?` for its local help.

## Editing helpers

Formatting and linting:

| Key | What it does |
| --- | --- |
| `<leader>mp` | Format file or selected range |
| `<leader>l` | Run linter now |

Substitute plugin:

| Key | What it does |
| --- | --- |
| `<leader>r` | Substitute with a motion |
| `<leader>rr` | Substitute current line |
| `<leader>R` | Substitute to end of line |
| Visual `<leader>r` | Substitute selected text |

Comment plugin defaults kept by this config:

| Key | What it does |
| --- | --- |
| `gcc` | Toggle comment on current line |
| `gc` + motion | Comment a motion, like `gcj` or `gcap` |
| Visual `gc` | Comment selection |
| `gco` | Add comment below and enter insert mode |
| `gcO` | Add comment above and enter insert mode |
| `gcA` | Add comment at end of line and enter insert mode |

Treesitter incremental selection:

| Key | What it does |
| --- | --- |
| `<C-Space>` | Start or expand selection |
| `<BS>` | Shrink selection |

Completion menu in insert mode:

| Key | What it does |
| --- | --- |
| `<C-Space>` | Open completion menu |
| `<C-j>` | Next suggestion |
| `<C-k>` | Previous suggestion |
| `<C-b>` | Scroll docs up |
| `<C-f>` | Scroll docs down |
| `<C-e>` | Close completion menu |
| `<CR>` | Confirm selected item |

## Sessions and startup

| Key | What it does |
| --- | --- |
| `<leader>wr` | Restore saved session for current cwd |
| `<leader>ws` | Save session for current cwd |

On the Alpha dashboard:

| Key | What it does |
| --- | --- |
| `e` | New file |
| `q` | Quit Neovim |
| `SPC ee` | Toggle file explorer |
| `SPC ff` | Find file |
| `SPC fs` | Live grep |
| `SPC wr` | Restore session |

## Good questions to ask later

When you come back, useful prompts would be:

- "How do I rename a symbol in this config?"
- "How do I search for text across the project?"
- "How do I open a file in a vertical split from Telescope?"
- "How do I create or rename files in NvimTree?"
- "How do I format just the selected lines?"
- "How do I use Trouble vs Telescope for diagnostics?"
- "What is the fastest way to jump between splits and tabs here?"

## If you forget everything

Start with these:

- `Space` then wait for `which-key`
- `<leader>fk` to search mappings
- `g?` inside NvimTree
- `?` inside Telescope normal mode
- `?` inside Trouble
