# zsh-pyenv-virtualenvwrapper-lazy

A zsh plugin for lazy loading of pyenv-virtualenvwrapper.

Lazily loading pyenv itself creates confusion inside IDE terminals that source the virtualenv when the terminal starts. In this scenario, when `python` is run, pyenv lazily loads and breaks out of the current virtualenv. The user thinks they are in the virtualenv when they aren't. So this plugin loads pyenv eagerly, and virtualenvwrapper lazily.

## Installation

Using [antibody](https://github.com/getantibody/antibody):

```shell
antibody bundle tekumara/zsh-pyenv-virtualenvwrapper-lazy
```

Manually:

```shell
git clone https://github.com/tekumara/zsh-pyenv-virtualenvwrapper-lazy ~/.zsh-pyenv-virtualenvwrapper-lazy

# add the following to ~/.zshrc
source ~/.zsh-pyenv-virtualenvwrapper-lazy/pyenv-vew-lazy.plugin.zsh
```
