# Configuring Kdiff3 for use with Git

Install the latest version of Kdiff3:
`http://kdiff3.sourceforge.net/`

Edit `c:\Users\<username>\.gitconfig` and add:
```
[merge]
    tool = kdiff3
[mergetool "kdiff3"]
    cmd = \"C:\\\\Program Files (x86)\\\\KDiff3\\\\kdiff3\" $BASE $LOCAL $REMOTE -o $MERGED
```

Once configured, typing `git mergetool` will fire up Kdiff3 and highlight the merge conflicts. 
	
Instructions derived from:
`http://jebaird.com/2013/07/08/setting-up-kdiff3-as-the-default-merge-tool-for-git-on-windows.html`

For BeyondCompare, see:
`http://www.scootersoftware.com/support.php?zz=kb_vcs#githubwindows`