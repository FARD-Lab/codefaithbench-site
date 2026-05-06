# CodeFaithBench | Project Site

Recruiting site for **CodeFaithBench**, a research project at FARD Lab (UBC Okanagan) on the faithfulness of LLM explanations for code reasoning.

**Live:** https://fard-lab.github.io/codefaithbench-site/

---

## Stack

Plain HTML + Tailwind CSS (via CDN) + small custom CSS layer.
Edit a `.html` file → push to `main` → GitHub Pages redeploys in ~60 seconds.

## Files

```
.
├── index.html          # Landing page
├── team.html           # PI, students, open positions
├── join.html           # Recruiting details and contact
├── assets/
│   ├── styles.css      # Custom styles (CSS variables for colors)
│   └── favicon.svg
├── .nojekyll           # Tells GitHub Pages to skip Jekyll processing
└── README.md
```

## Local preview

Any static file server works:

```bash
python3 -m http.server 8000
# or
npx serve .
```

Open http://localhost:8000.

## Editing

**Update text:** Open the relevant `.html` file and edit between tags. Tailwind utility classes can stay.

**Add a team member:** In `team.html`, copy a `<div class="card">…</div>` block under "Student Researchers" and edit the name, role, and bio.

**Add a new page:** Copy any existing `.html` file as your starting point; nav, footer, and styling are already wired up. Then add the page to the nav block in *all* existing files (search for `nav-link` to find them).

**Change the color palette:** Edit the CSS variables at the top of `assets/styles.css`. The site uses slate (backgrounds) + amber (accents).

**Update the "Last updated" date:** Bump the year in the footer of each HTML file.

## License

Site content © FARD Lab. Code under MIT. Feel free to adapt the structure for your own project.
