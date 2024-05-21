# Personal ZMK config

## Build

In development container, run:

```bash
cd app
west build -d build/left -b "nice_nano_v2" -- -DSHIELD="corne_left" -DZMK_CONFIG="/workspaces/zmk-config/config"
west build -d build/right -b "nice_nano_v2" -- -DSHIELD="corne_right" -DZMK_CONFIG="/workspaces/zmk-config/config"
```

Make sure that zmk-config is correctly mounted in the container.

## Other notes

- For advanced build scripts, see https://github.com/urob/zmk-config/blob/main/readme.md
