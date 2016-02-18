# Checkout File from Branch to Revert Edits

A common issue in git repos with ipython notebooks is that the notebook metadata will change, even if no ends are made but the notebook is run. Instead of creating unnecessary merge conflicts, the easy solution is to revert a file back to the original.

```
git checkout [branch] [filename]
```

e.g.

```
git checkout origin 3_2_Equatorial_Coordinates.ipynb
```
