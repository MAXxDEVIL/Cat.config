```
## CAVA Blue Bars (No Blue Background)

[general]
live-config = 1
framerate = 60
autosens = 1
sensitivity = 100

bars = 0
bar_width = 2
bar_spacing = 1
center_align = 1
max_height = 100

lower_cutoff_freq = 50
higher_cutoff_freq = 10000
sleep_timer = 0


[input]
method = pulse
source = auto


[output]
method = noncurses
orientation = bottom
channels = stereo
mono_option = average
reverse = 0
synchronized_sync = 1
show_idle_bar_heads = 1


[color]
background = default          # keep terminal background (no blue)
foreground = '#2170b5'        # main blue bars

gradient = 1
gradient_color_1 = '#2170b5'
gradient_color_2 = '#2f80d1'
gradient_color_3 = '#3c8fed'
gradient_color_4 = '#4da3ff'
gradient_color_5 = '#6bb8ff'
gradient_color_6 = '#8accff'
gradient_color_7 = '#a8ddff'
gradient_color_8 = '#c6ecff'

blend_direction = 'up'


[smoothing]
noise_reduction = 77


[eq]
1 = 1
2 = 1
3 = 1
4 = 1
5 = 1


```