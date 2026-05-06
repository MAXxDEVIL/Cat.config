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
            "format": "\u001b[38;5;33m┌──────────────────────Hardware──────────────────────┐"
        },
        {
            "type": "host",
            "key": " PC",
            "keyColor": "#2170b5"
        },
        {
            "type": "cpu",
            "key": "│ ├",
            "keyColor": "#2170b5"
        },
        {
            "type": "gpu",
            "key": "│ ├󰍛",
            "keyColor": "#2170b5"
        },
        {
            "type": "memory",
            "key": "│ ├󰍛",
            "keyColor": "#2170b5"
        },
        {
            "type": "custom",
            "format": "\u001b[38;5;33m└────────────────────────────────────────────────────┘"
        },

        "break",
        {
            "type": "custom",
            "format": "\u001b[38;5;33m┌──────────────────────Software──────────────────────┐"
        },
        {
            "type": "os",
            "key": "󰣇 OS",
            "keyColor": "#2170b5"
        },
        {
            "type": "kernel",
            "key": "│ ├",
            "keyColor": "#2170b5"
        },
        {
            "type": "packages",
            "key": "│ ├󰏖",
            "keyColor": "#2170b5"
        },
        {
            "type": "shell",
            "key": "└ └",
            "keyColor": "#2170b5"
        },

        "break",
        {
            "type": "de",
            "key": " DE",
            "keyColor": "#2170b5"
        },
        {
            "type": "lm",
            "key": "│ ├",
            "keyColor": "#2170b5"
        },
        {
            "type": "wm",
            "key": "│ ├",
            "keyColor": "#2170b5"
        },
        {
            "type": "wmtheme",
            "key": "└ └󰉼",
            "keyColor": "#2170b5"
        },
        {
            "type": "custom",
            "format": "\u001b[38;5;33m└────────────────────────────────────────────────────┘"
        },

        "break",
        {
            "type": "custom",
            "format": "\u001b[38;5;33m┌────────────────────Uptime / Age────────────────────┐"
        },
        {
            "type": "command",
            "key": "  OS Age ",
            "keyColor": "#2170b5",
            "text": "birth_install=$(stat -c %W /); current=$(date +%s); time_progression=$((current - birth_install)); days_difference=$((time_progression / 86400)); echo $days_difference days"
        },
        {
            "type": "uptime",
            "key": "  Uptime ",
            "keyColor": "#2170b5"
        },
        {
            "type": "custom",
            "format": "\u001b[38;5;33m└────────────────────────────────────────────────────┘"
        }
    ]
}

```
