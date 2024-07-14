Tabindex

- interactable elements has tabindex by default
- tabindex = 0 to enable tabindex
- tabindex < 0 to disable tabindex
- NOT recommend tabindex > 0: browser prioritizes tabindex > 0, after jumping to all tabindex > 0, jump back to first tabindex = 0 

Flow

- jump to select button:
  - click / Enter / Space: open dropdown
  - KeyUp / KeyDown: open dropdown + jump to selected option, if none selected, jump to first option
- KeyUp / KeyDown: navigate through options
- can jump back and forth between: 
  - current focused option (not chosen option)
  - select button (prev)
  - normal button (next)
- click / Enter / Space: 
  - choose option
  - close dropdown + jump back to select button

Careful

- press Enter to choose option + **focus** select button in **same cycle** will trigger click event of select button -> opening dropdown again