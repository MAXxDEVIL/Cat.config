```


"$schema" = 'https://starship.rs/config-schema.json'
add_newline = false

format = """
[╭────────────────────────────────────────────────────Ｏ](bold #9b59b6)
[│](bold #9b59b6)[░▒▓](#9b59b6)\
$os\
$username\
[](bg:#9b59b6 fg:#9b59b6)\
$directory\
[](fg:#9b59b6 bg:#9b59b6)\
$git_branch\
$git_status\
[](fg:#9b59b6 bg:#9b59b6)\
$c\
$cpp\
$rust\
$golang\
$nodejs\
$php\
$java\
$kotlin\
$haskell\
$python\
[](fg:#9b59b6 bg:#9b59b6)\
$docker_context\
$conda\
$pixi\
[](fg:#9b59b6 bg:#9b59b6)\
$time\
[ ](fg:#9b59b6)\
$line_break$character
"""

palette = 'blue_theme'

[palettes.blue_theme]
color_fg0 = '#e6f1ff'
color_bg1 = '#9b59b6'
color_bg3 = '#9b59b6'
color_blue = '#9b59b6'
color_aqua = '#9b59b6'
color_green = '#9b59b6'
color_orange = '#9b59b6'
color_purple = '#9b59b6'
color_red = '#9b59b6'
color_yellow = '#9b59b6'

[os]
disabled = false
style = "bg:color_orange fg:color_fg0"

[os.symbols]
Windows = "󰍲"
Ubuntu = "󰕈"
SUSE = ""
Raspbian = "󰐿"
Mint = "󰣭"
Macos = "󰀵"
Manjaro = ""
Linux = "󰌽"
Gentoo = "󰣨"
Fedora = "󰣛"
Alpine = ""
Amazon = ""
Android = ""
Arch = "🜲"
CachyOS = "󰣇"
Artix = "󰣇"
EndeavourOS = ""
CentOS = ""
Debian = "󰣚"
Redhat = "󱄛"
RedHatEnterprise = "󱄛"
Pop = ""

[username]
show_always = true
style_user = "bg:color_orange fg:color_fg0"
style_root = "bg:color_orange fg:color_fg0"
format = '[ $user ]($style)'

[directory]
style = "fg:color_fg0 bg:color_yellow"
format = "[ $path ]($style)"
truncation_length = 3
truncation_symbol = "…/"

[git_branch]
symbol = ""
style = "bg:color_aqua"
format = '[[ $symbol $branch ](fg:color_fg0 bg:color_aqua)]($style)'

[git_status]
style = "bg:color_aqua"
format = '[[($all_status$ahead_behind )](fg:color_fg0 bg:color_aqua)]($style)'

[nodejs]
symbol = ""
style = "bg:color_blue"
format = '[[ $symbol( $version) ](fg:color_fg0 bg:color_blue)]($style)'

[c]
symbol = " "
style = "bg:color_blue"
format = '[[ $symbol( $version) ](fg:color_fg0 bg:color_blue)]($style)'

[cpp]
symbol = " "
style = "bg:color_blue"
format = '[[ $symbol( $version) ](fg:color_fg0 bg:color_blue)]($style)'

[rust]
symbol = ""
style = "bg:color_blue"
format = '[[ $symbol( $version) ](fg:color_fg0 bg:color_blue)]($style)'

[golang]
symbol = ""
style = "bg:color_blue"
format = '[[ $symbol( $version) ](fg:color_fg0 bg:color_blue)]($style)'

[php]
symbol = ""
style = "bg:color_blue"
format = '[[ $symbol( $version) ](fg:color_fg0 bg:color_blue)]($style)'

[java]
symbol = ""
style = "bg:color_blue"
format = '[[ $symbol( $version) ](fg:color_fg0 bg:color_blue)]($style)'

[kotlin]
symbol = ""
style = "bg:color_blue"
format = '[[ $symbol( $version) ](fg:color_fg0 bg:color_blue)]($style)'

[haskell]
symbol = ""
style = "bg:color_blue"
format = '[[ $symbol( $version) ](fg:color_fg0 bg:color_blue)]($style)'

[python]
symbol = ""
style = "bg:color_blue"
format = '[[ $symbol( $version) ](fg:color_fg0 bg:color_blue)]($style)'

[docker_context]
symbol = ""
style = "bg:color_bg3"
format = '[[ $symbol( $context) ](fg:#9b59b6 bg:color_bg3)]($style)'

[conda]
style = "bg:color_bg3"
format = '[[ $symbol( $environment) ](fg:#9b59b6 bg:color_bg3)]($style)'

[pixi]
style = "bg:color_bg3"
format = '[[ $symbol( $version)( $environment) ](fg:color_fg0 bg:color_bg3)]($style)'

[time]
disabled = false
time_format = "%R"
style = "bg:color_bg1"
format = '[[  $time ](fg:color_fg0 bg:color_bg1)]($style)'

[line_break]
disabled = false

[character]
disabled = false
success_symbol = '[╰─](bold #9b59b6)[❯](bold fg:#9b59b6)'
error_symbol = '[╰─](bold #9b59b6)[✘](bold fg:#9b59b6)'
vimcmd_symbol = '[❮](bold fg:#9b59b6)'
vimcmd_replace_one_symbol = '[❮](bold fg:color_purple)'
vimcmd_replace_symbol = '[❮](bold fg:color_purple)'
vimcmd_visual_symbol = '[❮](bold fg:#9b59b6)'



```
