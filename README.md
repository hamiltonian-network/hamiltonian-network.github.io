# Project page

Source for the project website. The page is generated from the run files by
`scripts/make_site.py` in the code repository — every number and every plotted
point is read from `results/*.jsonl`, so the page cannot drift from the runs.

To regenerate and republish:

```bash
python scripts/make_site.py          # in the code repository
cp docs/index.html /path/to/this/repo/index.html
git -C /path/to/this/repo commit -am "Update project page" && git push
```
