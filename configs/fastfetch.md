```

{
    "$schema": "https://github.com/fastfetch-cli/fastfetch/raw/dev/doc/json_schema.json",

    "logo": {
        "source": "/home/mr_cat/Pictures/imp/dra.png",
        "type": "kitty",
        "height": 16,
        "width": 32,
        "padding": {
            "top": 2,
            "left": 2
        }
    },

    "modules": [
        "break",
        {
            "type": "custom",
            "format": "\u001b[38;2;146;110;228m┌──────────────────────────────Hardware──────────────────────────────┐"
        },
        {
            "type": "host",
            "key": " PC",
            "keyColor": "#926ee4"
        },
        {
            "type": "cpu",
            "key": "│ ├",
            "keyColor": "#926ee4"
        },
        {
            "type": "gpu",
            "key": "│ ├󰍛",
            "keyColor": "#926ee4"
        },
        {
            "type": "memory",
            "key": "│ ├󰍛",
            "keyColor": "#926ee4"
        },
        {
            "type": "custom",
            "format": "\u001b[38;2;146;110;228m└────────────────────────────────────────────────────────────────────┘"
        },

        "break",
        {
            "type": "custom",
            "format": "\u001b[38;2;146;110;228m┌──────────────────────────────Software──────────────────────────────┐"
        },
        {
            "type": "os",
            "key": "󰣇 OS",
            "keyColor": "#926ee4"
        },
        {
            "type": "kernel",
            "key": "│ ├",
            "keyColor": "#926ee4"
        },
        {
            "type": "packages",
            "key": "│ ├󰏖",
            "keyColor": "#926ee4"
        },
        {
            "type": "shell",
            "key": "└ └",
            "keyColor": "#926ee4"
        },

        "break",
        {
            "type": "de",
            "key": " DE",
            "keyColor": "#926ee4"
        },
        {
            "type": "lm",
            "key": "│ ├",
            "keyColor": "#926ee4"
        },
        {
            "type": "wm",
            "key": "│ ├",
            "keyColor": "#926ee4"
        },
        {
            "type": "wmtheme",
            "key": "└ └󰉼",
            "keyColor": "#926ee4"
        },
        {
            "type": "custom",
            "format": "\u001b[38;2;146;110;228m└────────────────────────────────────────────────────────────────────┘"
        },

        "break",
        {
            "type": "custom",
            "format": "\u001b[38;2;146;110;228m┌────────────────────────────Uptime / Age────────────────────────────┐"
        },
        {
            "type": "command",
            "key": "  OS Age ",
            "keyColor": "#926ee4",
            "text": "birth_install=$(stat -c %W /); current=$(date +%s); time_progression=$((current - birth_install)); days_difference=$((time_progression / 86400)); echo $days_difference days"
        },
        {
            "type": "uptime",
            "key": "  Uptime ",
            "keyColor": "#926ee4"
        },
        {
            "type": "custom",
            "format": "\u001b[38;2;146;110;228m└────────────────────────────────────────────────────────────────────┘"
        }
    ]
}


```
