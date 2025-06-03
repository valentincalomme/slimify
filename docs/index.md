# Slimify

Python Build Slimmer: Only What You Need.

## Background

Python packages sometimes contain unnecessary files which bloat the size needed to be downloaded over the internet.

Slimify is a package that provides several utilities regarding build size.

- Ability to warn/fail a build if the resulting artifact contains unnecessary file
- Ability to estimate the size reduction of a particular package
- Ability to suggest how to reduce the size (i.e. add ignore statements etc.)
- Ability to add build hooks that reduce the size of the package (i.e. remove assert statements, pyminify, replace spaces with tabs, remove comments, obfuscate/remame methods and variables, remove empty lines, increase line length, remove type hints (optional), remove docstrings (optional)
- Pre-commit hook to verify total size of build to catch potential random increases
- Find missing wheels
