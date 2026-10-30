# taiho-wang.github.io

Personal academic website of Tai-Ho Wang, Professor of Mathematics at Baruch College, CUNY.

Live at **https://taiho-wang.github.io/**

## How this site works

The whole site is one file, `index.html`, plus the portrait in `images/`. GitHub Pages publishes whatever is on the `main` branch, usually within a minute of a push.

## Add a paper

In `index.html`, find `<ol id="pub-list"`, copy the first `<li …>…</li>` block, paste it directly above it, and edit:

```html
<li data-topic="amm" data-year="2026"><span class="p-dot t-amm" aria-hidden="true"></span><div class="p-body"><a class="p-title" href="https://arxiv.org/abs/XXXX.XXXXX" target="_blank" rel="noopener">Paper title<svg …></svg></a><p class="p-meta">with Coauthor One and Coauthor Two<br>Preprint, arXiv</p></div><span class="p-year">2026</span></li>
```

- `data-topic` (and the `t-…` class on the dot) is one of `amm`, `exec`, `vol`, `prob`, `stats`. It decides the color and which filter shows the paper.
- `data-year` places the paper in the per-year chart.

The topic counts and the per-year chart update themselves from the list, so nothing else needs changing.

## Other edits

Contact details, positions and education are plain text in `index.html`: search for the text and edit it in place. The career timeline chart under "Academic experiences" uses `left:` and `width:` percentages on a 1990–2027 scale; asking Claude to update it is the easy route.

After editing: commit and push (in GitHub Desktop: write a short summary, click **Commit to main**, then **Push origin**).
