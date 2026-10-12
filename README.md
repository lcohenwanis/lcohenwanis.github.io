# lcohenwanis.github.io

Source for my personal website, <https://lcohenwanis.github.io>.

GitHub Pages builds the site with Jekyll every time something is pushed to
`main`. There is nothing to install: edit a file here, commit, and the live
site updates a minute or so later.

## Where things live

| To change | Edit |
| --- | --- |
| Papers | `_data/publications.yml` |
| Projects | `_data/projects.yml` |
| Jobs and the timeline chart | `_data/experience.yml` |
| Degrees | `_data/education.yml` |
| Email, GitHub, Google Scholar, ORCID, LinkedIn links | `_config.yml` |
| The intro and Research text | `index.html` |
| Colors, fonts, spacing | `assets/css/style.css` |
| Portrait | `assets/img/luc-cohen-wanis.jpg` (square, about 960 px) |

## Add a paper

Open `_data/publications.yml` and add an entry at the top of the list:

```yaml
- title: "Paper title"
  authors: "Luc Cohen-Wanis, Sam Zhang"
  venue: "Journal Name"
  year: 2027
  url: https://doi.org/10.0000/example
  pdf: https://arxiv.org/pdf/0000.00000    # optional
  code: https://github.com/lcohenwanis/example    # optional
  note: Preprint    # optional
```

The Papers section and its menu link stay hidden while the file has no
entries, and appear once it has one.

## Add a project

Open `_data/projects.yml` and add an entry:

```yaml
- name: "Project name"
  description: >-
    What the project asks, what data it uses, and what came out of it.
  url: https://github.com/lcohenwanis/example
  year: 2026    # optional
  tools: [Python, network analysis]    # optional
```

The Projects section works the same way as Papers: hidden until there is
something to show.

## Add or change a job

Each entry in `_data/experience.yml` becomes one bar in the timeline chart
and one item in the list under it. `start` and `end` are `"YYYY-MM"` in
quotes. Leave `end` out for a role you still hold. `kind` is `study`,
`industry` or `teaching` and sets the bar color.

## If the site doesn't update

Check the Actions tab of this repository. A red "pages build and deployment"
run usually means a YAML typo, most often indentation or a missing quote.

## Preview on your own computer (optional)

```sh
gem install jekyll
jekyll serve
```

Then open <http://localhost:4000>.

## Credits

Typefaces are Besley and Instrument Sans, both under the SIL Open Font
License (see `assets/fonts/`).
