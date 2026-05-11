# IC PTE Poster

[![Poster preview](IC_PTE_Poster_preview.png)](IC_PTE_Poster.pdf)

[Open the poster PDF](IC_PTE_Poster.pdf)

Source files and rendered outputs for the poster:

**Spatial Distribution of Traumatic Brain Injury Contusions and Post-Traumatic Epilepsy**

## Contents

- `IC_PTE_Poster.Rmd`: main poster source.
- `IC_PTE_Poster_preview.png`: README preview image linked to the PDF.
- `IC_PTE_Poster.html`: rendered HTML poster.
- `IC_PTE_Poster.pdf`: rendered PDF poster.
- `IC_PTE_Poster_files/`: supporting HTML figure files.
- `packages.bib`: bibliography generated for the poster.
- `table1_demographics_poster.csv`: demographics table used in the poster.
- `poster_cosine_panels.csv`: cosine-similarity values used for poster panels.
- `glass_stat_*_5_epi.png`: glass-brain statistical map images used in the poster.

`IC_PTE_Poster_3columns.Rmd` is retained as an alternate layout/source draft.

## Render

Install the R packages used by the poster:

```r
install.packages(c(
  "posterdown",
  "rmarkdown",
  "knitr",
  "ggplot2",
  "dplyr",
  "readr",
  "patchwork",
  "png"
))
```

Render from R:

```r
rmarkdown::render("IC_PTE_Poster.Rmd")
```

Or from a shell:

```bash
Rscript -e 'rmarkdown::render("IC_PTE_Poster.Rmd")'
```

## Notes

- The poster was built with `posterdown::posterdown_html`.
- The HTML output is not self-contained, so keep `IC_PTE_Poster_files/` with
  `IC_PTE_Poster.html`.
- The included CSV files are analytic/poster inputs, not raw imaging data.

## Acknowledgment

Poster layout uses the `posterdown` R package:
<https://github.com/brentthorne/posterdown>

## License

MIT License. See `LICENSE`.
