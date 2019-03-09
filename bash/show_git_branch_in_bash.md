# How to show the git branch in the bash shell 

## Instructions

Sometimes it can be a little bit confusing in which branch in git you are, with this extension to your ```.bashrc``` you can show the git branch you are currently in when you are navigating through a directory directly in the shell. 

```
force_color_prompt=yes
color_prompt=yes
parse_git_branch() {
 git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/(\1)/'
}
if [ "$color_prompt" = yes ]; then
 PS1='${debian_chroot:+($debian_chroot)}\[\033[01;32m\]\u@\h\[\033[00m\]:\[\033[01;34m\]\w\[\033[01;31m\]$(parse_git_branch)\[\033[00m\]\$ '
else
 PS1='${debian_chroot:+($debian_chroot)}\u@\h:\w$(parse_git_branch)\$ '
fi
unset color_prompt force_color_prompt
```

## Pictures

![picture of the git branch in the shell](../media/show_git_branch.png)
