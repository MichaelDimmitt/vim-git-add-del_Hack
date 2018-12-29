# vim-git-add-del_Hack
When you "add -p <e (edit) flag>" and are doing a refactor.

1) Add deletions first "for a simplifying project commit"
2) Add additions "for code has moved to here commit"

## Implementation instructions, see #1 (plan)[#1]
1) vim plugin recognizes previous command contained 'git * -p'
2) plugin recognizes that it is in -e (edit) mode for -p command.
3) :add and :del ...
<br/>Text manipulation occurs to:
1) add(), remove the lines that contain + upon
2) del(), convert - to ' '
