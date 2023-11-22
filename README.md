# xxh plugin to warpify a zsh subshell.

A plugin to automatically warpify a subshell.

[Warp](https://www.warp.dev/) is required.

```
xxh +I xxh-plugin-zsh-warpify-subshell+git+https://github.com/jloewe/xxh-plugin-zsh-warpify-subshell
```

## Fix for Warp autocompletions

For some reason, xxh doesn't set the SHELL environment variable to zsh.

To fix this, add the following argument to your command or xxhc config file:

```yml
# argument for xxh command
xxh <user@host> +e SHELL="${ZDOTDIR}/zsh-bin/bin/zsh"
```

```yml
# xxhc.config
# ...
  +e:
    - SHELL="${ZDOTDIR}/zsh-bin/bin/zsh"
```
