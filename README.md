# helm-open-github.el
*helm-open-github.el* is utilities for opening github url.
This is inspired by URL below.

* http://shibayu36.hatenablog.com/entry/2013/01/18/211428

## screenshot

![open-github-from-commit](image/open-github-from-commit.png)


## Dependency

* Emacs 23.4 or higher
* [helm](https://github.com/emacs-helm/helm)
* [gh](https://github.com/sigma/gh.el)


## Basic Usage

### `helm-open-github-from-commit`

Open commit page from *commit id*

### `helm-open-github-from-file`

Open file page from *file name*

### `helm-open-github-from-issues`

Open issue page from *issue ID*


## Customize

### `helm-open-github-commit-limit`

Issue number shown by `helm-open-github-from-commit`.(Default is 100)


## Sample Configuration

```elisp
(require 'helm-open-github)
(global-set-key (kbd "C-c o f") 'helm-open-github-from-file)
(global-set-key (kbd "C-c o c") 'helm-open-github-from-commit)
(global-set-key (kbd "C-c o i") 'helm-open-github-from-issues)
```
