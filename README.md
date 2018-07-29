# Package repositories

This GitHub repository offers ready to install builds of some of my [R](https://r-project.org) projects. More precisely, the [l10n](https://undocumeantit.github.io/repos/l10n/index.html) repository hosts various language support packages for the [sylly](https://github.com/unDocUMeantIt/sylly) package. While sylly itself was released on CRAN, unfortunately its language packages could not be published there as well.

## Installation

To directly install one of the language packages, i.e., [support for German](https://github.com/unDocUMeantIt/sylly.de), call:

```
install.packages("sylly.de", repo="https://undocumeantit.github.io/repos/l10n")
```

It is recommended to add `https://undocumeantit.github.io/repos/l10n` to your list of available R package repositories if you are using either the sylly package or [koRpus](https://github.com/unDocUMeantIt/koRpus), which depends on sylly and some of its language packages. For example, you can acheive this by adding the following to a local [`.Rprofile` file](http://www.statmethods.net/interface/customizing.html):

```
options(repos=c(getOption("repos"), l10n="https://undocumeantit.github.io/repos/l10n"))
```

That way, you will automatically receive stable updates once they're released here, and installation of packages is also more straight forward:

```
install.packages("sylly.de")
```

If you're running a Debian based operating system, you might be delighted to learn that [.deb packages are available](https://undocumeantit.github.io/repos/l10n/pckg/sylly.de/deb_repo.html) as well.

