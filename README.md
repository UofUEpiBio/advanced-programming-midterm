# Template project for Advanced Programming [![Slides and report render](../../actions/workflows/check-qmd-render.yaml/badge.svg)](../../actions/workflows/check-qmd-render.yaml)

The template project has the following files:

- `README.md`: this file.
- `data/`: a folder for data files.
- `.gitignore`: a file that tells git which files to ignore.
- `slides.qmd`: a presentation in quarto format.
- `report.qmd`: a report in quarto format.
- `.github/workflows/check-qmd-render.yaml`: The workflow that builds the html and pdf files. New dependencies can be added on the step "Install dependencies"; the following installs the R packages data.table and slurmR from CRAN:

    ```yaml
    - name: Install dependencies
    run: |
        install2.r data.table slurmR
    ```

  This workflow should complete without errors before you submit your project.

## Instructions

1. Use the qmd files to write your report and slides.

2. Add any needed files (figures, C++, data, etc.) to the repository.

2. If needed, add additional dependencies to the workflow file.

3. Ensure the [report.pdf](report.pdf) and [slides.html](slides.html) files are generated.
