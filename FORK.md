# Weeb glass home

My own build of the [cleanyourtv](https://github.com/Gathin23/cleanyourtv) launcher, kept on the `personal` branch.
Built and used on a Xiaomi MiTV-AXSO2, Android TV 9, firmware PI.6432. It adds no permission and no network use.

What it adds, each off until a theme turns it on:

| Key | What it does |
|---|---|
| `wallpaper_accents` | The focus highlight and the greeting take each wallpaper's colour, from `wallpapers/accents.txt` |
| `clock_glass` | The clock, greeting and date in one frosted capsule |
| `wallpaper_button` | A top bar button: next picture, stay on this one, and the minutes between changes |
| `tile_menu` with `fill_dock` false | Holding OK on a dock tile also offers Remove from dock |

This build ships in English only, to keep the APK small.

## Build and install

Follow the launcher steps in this repo's `README.md`, then push the theme:

    launcher/build-and-install.sh
    TV_HOST=<tv ip> tools/theme.sh themes/weeb

Copy `themes/weeb` to a folder outside the checkout if you want to use your own pictures, so they are never committed.

The five pictures in `themes/weeb` were made with Google Gemini; see `themes/weeb/CREDITS.md`.
