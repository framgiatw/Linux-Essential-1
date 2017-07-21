# Exercise 02 Working With Shells

## Install ZSH through Oh My Zsh
https://github.com/robbyrussell/oh-my-zsh/wiki/Installing-ZSH

## Install Fish
https://fishshell.com/

## Set default shell
- Add shell path to `/etc/shells file`
- Change default shell with `chsh` command: For example `chsh -s /usr/local/bin/fish`

## Customize Shells

### References:
- https://wiki.archlinux.org/index.php/Bash/Prompt_customization
- https://www.digitalocean.com/community/tutorials/how-to-customize-your-bash-prompt-on-a-linux-vps

### Example

```
PS1="[\[\e[0;35m\]\u\[\e[m\]@\[\e[0;36m\]\h\[\e[m\] \[\e[1;34m\]\w\[\e[m\]\[\e[1;32m\]\$(parse_git_branch)\[\e[m\]]\$ "


parse_git_branch() {
git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/ (\1)/'
}
```

Break it down:
```
[
  \[\e[0;35m\] --> color escape code
    \u         --> current user
  \[\e[m\]
    @
  \[\e[0;36m\]
    \h         --> hostname
  \[\e[m\]

  \[\e[1;34m\]
    \w         --> current working directory
  \[\e[m\]

  \[\e[1;32m\]
    \$(parse_git_branch) --> show git branch
  \[\e[m\]
]
\$
```

### Let's customize
- Change host text to bold red
- Show clock
- Change username background to green, text to pink
- Add your name to prompt
- **Advanced:** add Ubuntu code name to prompt
