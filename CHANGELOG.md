## v0.11.0 (2023-05-17)

### Feat

- Nav bar links to project GitHub
- **projects**: allow overriding toc template path
- **projects**: mapping between project versions
- **projects**: allow overriding and disabling external mappings from conf.py
- **intersphinx**: Support intersphinx base urls in toc.yml
- **intersphinx**: support single strings for project
- **intersphinx**: add version replacement in the yaml
- **intersphinx**: Allow overriding branch name via environment variable
- fetch intersphinx config from a remote file

### Fix

- **rocm_footer.css**: Fix overlap with sidebar
- **renameVersionLinks.js**: Wait for RTD injection

### Refactor

- Still get PR branch using pygithub
- Use RTD environment variables
- Remove edit button, simplify get_branch
- **__init__.py**: remove deprecated and unused method
- **projects**: rename external_intersphinx to projects
- **doxygen**: Copy only doxygen folder from data

## v0.10.3 (2023-05-15)

### Fix

- **article-info**: hotfix non-html builds breaking

## v0.10.2 (2023-05-15)

### Fix

- Fix python typing, formatting, PEP8

## v0.10.1 (2023-05-11)

### Fix

- **sidebar**: fix rtd version selector not appearing on the sidebar for small screens
- **sidebar**: fix page jump when sidebar is opened, animate header
- **header**: don't show scroll-bar on menu when its not needed
- **article-info**: Use app.outdir for html directory
- allow overriding path to external toc path
- **custom.css**: restore cookie settings button styling

### Refactor

- **core.py**: fix mypy errors
- **article-info**: Simplify article-info handling

## v0.10.0 (2023-05-09)

### Feat

- Bring into compliance with AMD styling

### Fix

- Fix header on narrow screens
- Remove left side menu & buttons
- Fix lengths on shorter breadcrumbs
- Add zero width spaces when testing width
- deprecate disable_main_doc_link
- fix breadcrumbs and scrolling
- update ROCm Documentation url
- Tighten secondary nav
- Improve transitioning on resize

### Refactor

- Add links to header
- Merge remote-tracking branch 'upstream/develop' into HEAD

## v0.9.2 (2023-05-05)

### Fix

- check for existing article info before inserting

## v0.9.1 (2023-05-04)

### Fix

- **core.py**: use older version of pretty format in git log command

## v0.9.0 (2023-05-03)

### Feat

- **core.py**: set default publish date as time article was last modified
- **core.py**: set default read time by counting visible words in html output

### Refactor

- add back linkify
- merge with develop branch
- get file modification time using git
- import article info via importlib.resources
- convert myst_enable_extensions to set and add configunion helper
- **core.py**: explicitly cast to list

## v0.8.0 (2023-05-02)

### Feat

- Rename versioned doc links with version number

### Fix

- Remove unintended CSS changes

## v0.7.1 (2023-04-26)

## v0.7.0 (2023-04-26)

### Feat

- **core.py**: set specific page settings first before setting general settings
- **core.py**: add ability to set article info for all pages
- allow substitutions for author, date, and read time in article info
- add article info for linux and windows
- **core.py**: add article info with supported os info

### Fix

- **deps**: Fix search highlight in doxysphinx by updating sphinx version

### Refactor

- use consistent formatting for init and remove empty list from core
- **core.py**: move linkcheck configs to core from init

## v0.6.0 (2023-04-18)

### Feat

- use different link color based on theme
- increase font size

### Fix

- **header**: direct GitHub header link to ROCm

## v0.5.0 (2023-04-14)

### Feat

- **__init__.py**: add version numbers

### Fix

- ensure compatibility for 3.8 through 3.11
- **dependabot.yml**: remove extra spaces

## v0.4.0 (2023-04-13)

### BREAKING CHANGE

- users of the non-legacy API have to set `html_theme` to `rocm_docs_theme` to maintain the current behaviour.

### Fix

- **legacy**: fix builds without doxygen
- **extension**: no longer set the html_theme by default in the extension
- **legacy**: restore custom theme on readthedocs

## v0.3.0 (2023-04-13)

### Feat

- move automatic doxygen and doxysphinx to an extension
- move core settings to a sphinx extension

### Fix

- restore cookie permissions / analytics script

### Refactor

- various formatting and type fixes in util.py

## v0.2.2 (2023-04-13)

### Fix

- various stlysheet fixes

## v0.2.1 (2023-04-13)

### Fix

- update links in header and footer (#87)

## v0.0.1 (2023-03-13)
