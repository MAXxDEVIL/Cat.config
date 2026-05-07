"$schema" = 'https://starship.rs/config-schema.json'
add_newline = false

format = """
[╭────────────────────────────────────────────────────Ｏ](bold #2170b5)
[│](bold #2170b5)[░▒▓](#2170b5)\
$os\
$username\
[](bg:#4da3ff fg:#2170b5)\
$directory\
[](fg:#4da3ff bg:#3b82f6)\
$git_branch\
$git_status\
[](fg:#3b82f6 bg:#2563eb)\
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
[](fg:#2563eb bg:#1e40af)\
$docker_context\
$conda\
$pixi\
[](fg:#1e40af bg:#172554)\
$time\
[ ](fg:#172554)\
$line_break$character
"""

palette = 'blue_theme'

[palettes.blue_theme]
color_fg0 = '#e6f1ff'
color_bg1 = '#172554'
color_bg3 = '#1e3a8a'
color_blue = '#3b82f6'
color_aqua = '#38bdf8'
color_green = '#60a5fa'
color_orange = '#2170b5'
color_purple = '#6366f1'
color_red = '#1d4ed8'
color_yellow = '#4da3ff'

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
format = '[[ $symbol( $context) ](fg:#7dd3fc bg:color_bg3)]($style)'

[conda]
style = "bg:color_bg3"
format = '[[ $symbol( $environment) ](fg:#7dd3fc bg:color_bg3)]($style)'

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
success_symbol = '[╰─](bold #2170b5)[❯](bold fg:#38bdf8)'
error_symbol = '[╰─](bold #2170b5)[✘](bold fg:#1d4ed8)'
vimcmd_symbol = '[❮](bold fg:#38bdf8)'
vimcmd_replace_one_symbol = '[❮](bold fg:color_purple)'
vimcmd_replace_symbol = '[❮](bold fg:color_purple)'
vimcmd_visual_symbol = '[❮](bold fg:#4da3ff)'


