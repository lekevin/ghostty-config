# Ghostty configuration

Personal Ghostty settings. The repository lives in the macOS Ghostty configuration folder so edits to `config.ghostty` are tracked directly, without copying files.

## Save changes to GitHub

After editing and saving the config:

```sh
cd "$HOME/Library/Application Support/com.mitchellh.ghostty"
git diff -- config.ghostty
git add config.ghostty
git commit -m "Update Ghostty settings"
git push
```

GitHub updates when you commit and push; saving the file alone does not upload it. Press Command+Shift+Comma in Ghostty to reload settings.

## Restore on another Mac

If the destination already exists, back it up before cloning:

```sh
git clone git@github.com:lekevin/ghostty-config.git "$HOME/Library/Application Support/com.mitchellh.ghostty"
```
