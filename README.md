# NVim

<!--toc:start-->

- [NVim](#nvim)
  - [Vim Motions](#vim-motions)
  - [Modes](#modes)
  - [Ways to enter insert mode](#ways-to-enter-insert-mode)
  - [Normal Mode Actions](#normal-mode-actions)
    - [Normal Actions Plugins](#normal-actions-plugins)
    - [Ex Mode Visual Plugins](#ex-mode-visual-plugins)
  - [Macros](#macros)
  <!--toc:end-->

## Vim Motions

<!-- TODO: Populate explantation. -->

1. `hjkl` -> left, down, up, right.
2. `wW` -> beginning of next word (including symbols).
3. `eE` -> end of next word (including symbols).
4. `bB` -> beginning of previous word (including symbols)
5. `0_$` -> beginning of line, first non whitespace, end of line.
6. `Ctrl u`, `Ctrl d` -> half page up, half page down.
7. `fFtT` -> find right, find left (inclusive), find left, find right (exclusive).
8. `{}` -> Next newline up, next newline down.
9. `[]` -> Next reference left/up, right/down
10. `sS<chars>` -> Next chars left, next chars right, (Will highlight with jump characters).

## Modes

1. Insert (Regular typing). CMP menu C-n C-p to navigate and Enter to select
2. Ex (Select after action). d -> goes to Ex mode and then af executes d on the
   hovered outer function.
3. Visual / Visual Line (Highlight) -> Works with most Ex mode options in
   reverse. (Highlight and d to cut.)
4. Normal (Most movement occurs here).
5. Replace (r enters Ex mode and then goes to replace mode after selection is
   made. Same Visual rules apply)
6. Command Mode (:) Type vim commands or add ! and type bash commands.

There are more that you can enter.

## Ways to enter insert mode

- `a or A` -> Insert at end of current cursor, Insert at end of current line.
- `i or I` -> insert at start of current cursor, Insert at start of current line.
- `o or O` -> Create and insert to a new line below, to a new line above.
- `<Esc>` -> Exit insert mode.

## Normal Mode Actions

The above insert options are only available in normal mode.
: to enter command mode

Motion commands:

- `v` -> Enter Visual mode. (Motion commands in Visual and Ex mode are the same
  as normal)
- `V` -> Enter Visual line mode. (Same as v except you highlight entire lines at
  a time.)
- `Ctrl v` -> Enter Visual Block mode. (`I` will insert w/e you type on all lines.)
- `d` -> Cut in Ex mode. dd cuts the current line
- `x` -> Cut current cursor selection
- `p` -> Paste after cursor line
- `P` -> Paste before cursor line
- `y` -> Copy Current selection in V or enter Ex mode for copy yy grabs the
  current line.
- `<num>hjkl` -> Move num
- `g<num>` -> Go to line number
- `gg` -> Go to top of file
- `G` -> Go to end of file

### Normal Actions Plugins

- `K`-> Show documentation for selected code
- `gd` -> Go to Definition
- `]t \[t` -> Go to next TODO, previous TODO
- `]d \[d` -> Go to next diagnostic (error), previous
- `u` -> Undo
- `Ctrl r` -> Redo
- `<Leader>...` -> Honestly tons of stuff I will just go over the ones I use regularly
- `<L>bb` -> next buffer
- `<L>-` -> Split horizontal
- `<L>qq` -> quit all
- `<L>|` -> Split vertical
- `<L><Space>` -> Search files
- `<L>xx` -> Show all diagnostics
- `Ctrl /` -> Toggle Terminal
- `<L>ca` -> Code actions. (Automatically fix known errors / grammars.)
- `<L>cr` -> Rename the selected variable
- `<L>us` -> Toggle Spelling corrections.
- `Alt j` -> Move current selection (or line of cursor) down
- `Alt k` -> Move current selection up

### Ex Mode Visual Plugins

- `af` -> Select entire function + definition
- `if` -> Entire function without definition
- `ac` -> Entire class with definition
- `ic` -> Entire class without definition
- `as` -> entire scope including {} in c-like languages
- `is` -> entire scope excluding {} in c-like languages

  (Visual Only)

- `Ctrl Space` -> Increment logical selection up syntax tree
- `BackSpace` -> Increment down syntax tree.
  Many more that I don't often use.

## Macros

- q -> any key will start a macro recording.

Do anything you want to repeat. Press q to end the recording and then
call with @key or num@key to repeat the action one or num times.
