```

"$schema" = 'https://starship.rs/config-schema.json'
add_newline = false

format = """
[╭────────────────────────────────────────────────────Ｏ](bold #926ee4)
[│](bold #926ee4)[░▒▓](#926ee4)\
$os\
$username\
[](bg:#926ee4 fg:#926ee4)\
$directory\
[](fg:#926ee4 bg:#6f50b5)\
$git_branch\
$git_status\
[](fg:#6f50b5 bg:#3b347a)\
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
[](fg:#3b347a bg:#302b45)\
$docker_context\
$conda\
$pixi\
[](fg:#302b45 bg:#44365f)\
$time\
[ ](fg:#44365f)\
$line_break$character"""

palette = 'purple_theme'

[palettes.purple_theme]
color_fg0 = '#f3edff'
color_bg1 = '#926ee4'
color_bg3 = '#302b45'
color_blue = '#6f8cff'
color_aqua = '#55d6be'
color_green = '#62d6a5'
color_orange = '#f0ad70'
color_purple = '#b69aff'
color_red = '#ff718b'
color_yellow = '#f2cf75'

[os]
disabled = false
style = "bg:color_bg1 fg:#ffffff"

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
style_user = "bg:color_bg1 fg:#ffffff"
style_root = "bg:color_red fg:#ffffff"
format = '[ $user ]($style)'

[directory]
style = "fg:color_fg0 bg:color_bg1"
format = "[ $path ]($style)"
truncation_length = 3
truncation_symbol = "…/"

[git_branch]
symbol = ""
style = "bg:color_aqua"
format = '[[ $symbol $branch ](fg:#172d36 bg:color_aqua)]($style)'

[git_status]
style = "bg:color_aqua"
format = '[[($all_status$ahead_behind )](fg:#172d36 bg:color_aqua)]($style)'

[nodejs]
symbol = ""
style = "bg:color_blue"
format = '[[ $symbol( $version) ](fg:#151b38 bg:color_blue)]($style)'

[c]
symbol = " "
style = "bg:color_blue"
format = '[[ $symbol( $version) ](fg:#151b38 bg:color_blue)]($style)'

[cpp]
symbol = " "
style = "bg:color_blue"
format = '[[ $symbol( $version) ](fg:#151b38 bg:color_blue)]($style)'

[rust]
symbol = ""
style = "bg:color_blue"
format = '[[ $symbol( $version) ](fg:#151b38 bg:color_blue)]($style)'

[golang]
symbol = ""
style = "bg:color_blue"
format = '[[ $symbol( $version) ](fg:#151b38 bg:color_blue)]($style)'

[php]
symbol = ""
style = "bg:color_blue"
format = '[[ $symbol( $version) ](fg:#151b38 bg:color_blue)]($style)'

[java]
symbol = ""
style = "bg:color_blue"
format = '[[ $symbol( $version) ](fg:#151b38 bg:color_blue)]($style)'

[kotlin]
symbol = ""
style = "bg:color_blue"
format = '[[ $symbol( $version) ](fg:#151b38 bg:color_blue)]($style)'

[haskell]
symbol = ""
style = "bg:color_blue"
format = '[[ $symbol( $version) ](fg:#151b38 bg:color_blue)]($style)'

[python]
symbol = ""
style = "bg:color_blue"
format = '[[ $symbol( $version) ](fg:#151b38 bg:color_blue)]($style)'

[docker_context]
symbol = ""
style = "bg:color_bg3"
format = '[[ $symbol( $context) ](fg:color_purple bg:color_bg3)]($style)'

[conda]
style = "bg:color_bg3"
format = '[[ $symbol( $environment) ](fg:color_purple bg:color_bg3)]($style)'

[pixi]
style = "bg:color_bg3"
format = '[[ $symbol( $version)( $environment) ](fg:color_fg0 bg:color_bg3)]($style)'

[time]
disabled = false
time_format = "%R"
style = "bg:#44365f"
format = '[[  $time ](fg:color_fg0 bg:#44365f)]($style)'

[line_break]
disabled = false

[character]
disabled = false
success_symbol = '[╰─](bold #926ee4)[❯](bold #926ee4)'
error_symbol = '[╰─](bold #ff718b)[✘](bold #ff718b)'
vimcmd_symbol = '[❮](bold #926ee4)'
vimcmd_replace_one_symbol = '[❮](bold #b69aff)'
vimcmd_replace_symbol = '[❮](bold #b69aff)'
vimcmd_visual_symbol = '[❮](bold #926ee4)'


```
