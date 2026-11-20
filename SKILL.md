---
name: wmux-surface-focus
trigger: Use before creating a new wmux surface (terminal tab), and after it is created.
---

# wmux surface focus

Creating a surface moves focus to it, and the new surface inherits focus from whichever pane was already focused. Other agents' panes can be disturbed by that.

## Procedure

1. Before creating: read the current workspace, and select your own workspace and pane.
2. Create the surface in your own workspace (pass the workspace id explicitly).
3. After creating: select your own surface again, so the human's screen stays on your pane.
4. Verify with the current-workspace command before and after.

## Checks

- The surface list shows your surface as active after step 3.
- No other agent's pane gained focus because of you.

Source: summoner's standing rule, 2026-11-20 (the wmux focus rule). Topic: wmux focus. Status: draft, not published.
