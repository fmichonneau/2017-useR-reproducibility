# Instructor notes for useR tutorial

## First activity: plot life expectancy for Canada 1950-1960

Here, it seems that everyone will be using R, and it is going to be helpful. Everyone should be able to reproduce someone else code easily. Pointing out that if they were to use a different software it might make this exercise more difficult.

The "without talking with each other" is to emulate what typically happens when you inherit a project from someone who is not part of the company/lab.

## File organization

Placing the manuscript at the root of the directory that contains all the other artifacts makes it easy to deal with working directory and relative paths. All the files are below relative to manuscript.

Placing the tests into a `tests/` folder makes it easy to run all the tests at once using `test_dir()` from **`testthat`** for instance.

## Rmd demo

The `rr-demo.Rmd` file hosted under `material` folder, contains a basic Rmd file that illustrate a few concepts covered in the lesson:

* The use of parameters to change things in only 1 place
* The use of R functions within parameters with the `!r` notation
* The use of functions to generate plots, making it easier to do:
    - type checking
    - reduce code repetition
* Use `knitr::kable` to generate nicely formatted (simple) tables within Rmarkdown documents

As an activity, participants can modify the script in multiple ways:

* Easy: change their names
* Easy: change the countries (either simple variables `params$country_1` or `country_3`)
* Moderate: add trend lines in the plots
* Advanced: write tests on the data (potentially first inline the Rmd file, and later as testthat tests in a separate folder)

## Git

Demo only

## Where archive and publish?

Supplementary materials gets grayed out because it's not very stable in the long run.
