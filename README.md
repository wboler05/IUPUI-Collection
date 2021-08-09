# IUPUI Collection

This repo tracks a collection of repositories used during my graduate studies at IUPUI.  It contains a collection of tutorials, code, snippets, documentation, and even my PhD project.  

The collection repo relies on two packages for functionality, one which can be ignored if need be.  First, we rely on [vcstool](https://github.com/dirk-thomas/vcstool) to `import` and `export` libraries.  For you as the user, the most that you need to do is execute the `import` command, and never touch it again (unless to grab new repos). 

Second, the `vcstool` is tracked automatically for you via the `pipenv` tool.  This repo contains a `Pipfile` that simply tracks `vcstool`.  You do not need `pipenv` to load the repos, but this is provided to offer an ease of use.  If you decide not to use pipenv, you must install the correct `vcstool` package (not `vcstools` with a `s`). 

## Setup

1. Install `Pipenv`, however you choose. The following installs using your environment's `pip`, but your method may differ. 
```bash
python -m pip install pipenv
```
2. Install the `Pipenv` environment from the `Pipfile`:
```bash
# Execute install in the code directory
pipenv install
```
3. Execute repository imports using `vcs` from `vcstool`: 
```bash
pipenv run vcs < iupui.repos
```

## Access Issues

If you're having issues cloning a particular repo, it's most likely because you do not have access to the repo.  Please contact me for the correct access in this case. 

For all other issues, please make an issue on Github!