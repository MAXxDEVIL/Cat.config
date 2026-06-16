
## Initialize fish to kitty

```

shell /usr/bin/fish  

```





```

set -x STARSHIP_CONFIG "$HOME/.config/starship.toml"

# Initialize Starship for Fish
starship init fish | source

if status is-interactive
# Commands to run in interactive sessions can go here
end

# opencode
set -gx PATH $HOME/.opencode/bin $PATH

# pnpm
set -gx PNPM_HOME "$HOME/.local/share/pnpm"

if not contains $PNPM_HOME $PATH
    set -gx PATH $PNPM_HOME $PATH
end

# node / npm / npx
set -gx PATH $HOME/.nvm/versions/node/v22.21.1/bin $PATH


```



