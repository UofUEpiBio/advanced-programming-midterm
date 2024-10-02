# Template project for Advanced Programming

The template project has the following files:

- `README.md`: this file.
- `.gitignore`: a file that tells git which files to ignore.
- `slides.qmd`: a presentation in quarto format.
- `report.qmd`: a report in quarto format.
- `.github/workflows/website.yaml`: The workflow that builds the html and pdf files. New dependencies can be added on the step "Install dependencies"; the following installs the R packages data.table and slurmR from CRAN:

    ```yaml
    - name: Install dependencies
    run: |
        install2.r data.table slurmR
    ```