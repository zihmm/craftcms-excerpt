# CraftCMS Excerpt
An easy to use CraftCMS plugin to get an excerpt Twig functionality. The text gets truncated at a given position, but close to the last word. This prevents ugly middle-cutted wor... ;)

### Installation

1. Upload the `excerpt` directory to `craft/plugins/excerpt/` on your server.
2. Enable the plugin under Craft Admin > Settings > Plugins

### Use
You can use it as a simple Twig filter with the `charcount` as first and an optional `read more` second argument.

**Adds simple dots at the end**
```
{{ entry.body | excerpt(140, '...' }} 
```

**Adds a link at the end**
```
{{ entry.body | excerpt(140, '<a href="' ~ entry.url ~ '">read more...</a>') }} 
```

## License

This work is licenced under the MIT license.