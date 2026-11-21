# Graphite Amber

A dark skin for Hermes Agent with charcoal surfaces, warm amber controls, and ochre message bubbles. In Hermes Desktop and Webapp it also refines the chat layout, centers the composer in a new chat, and marks running sessions with an amber badge.

## Install

From this repository, run the following on the machine that runs Hermes (the gateway host if you use Webapp or connect Desktop to a remote gateway). For a named profile, use that profile's Hermes home and run the command in the same profile context.

```sh
skin_dir="${HERMES_HOME:-$HOME/.hermes}/skins"
mkdir -p "$skin_dir"
cp graphite-amber.yaml "$skin_dir/"
hermes skin use graphite-amber
```

In Desktop, you can also select `graphite-amber` in **Settings → Appearance**. Use dark mode for the full look. To switch back, run `hermes skin use default` in the same profile or select another theme in Appearance.

## Compatibility

- The palette is a Hermes skin; the layout overrides target the dark Desktop and Webapp interface, not the separate admin dashboard.
- No Hermes core changes or plugins are required. The separate Graphite Rail shortcut bar is not included.
- The CSS targets Hermes renderer markup. If an update changes that markup, some layout refinements may need updating.

## License

[MIT](LICENSE)
