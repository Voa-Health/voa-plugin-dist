# voa-plugin-dist

Public distribution repository for the **Voa** clinical documentation plugin
(`plugin.js`). This repo holds only the built artifact — the source lives in the
private [`Voa-Health/voa-integrations`](https://github.com/Voa-Health/voa-integrations)
repository and is automatically published here on every release.

## Usage

Include the plugin in your EHR / host application via [jsDelivr](https://www.jsdelivr.com/):

### Pinned version (recommended for production)

```html
<script src="https://cdn.jsdelivr.net/gh/Voa-Health/voa-plugin-dist@vX.Y.Z/plugin.js"></script>
```

Replace `vX.Y.Z` with a concrete version from the
[Releases page](https://github.com/Voa-Health/voa-plugin-dist/releases). Pinned
URLs are immutable and aggressively cached by jsDelivr.

### Latest version (development / staging)

```html
<script src="https://cdn.jsdelivr.net/gh/Voa-Health/voa-plugin-dist@latest/plugin.js"></script>
```

`@latest` resolves to the current `main` branch HEAD. jsDelivr revalidates this
URL periodically (up to ~12 hours of caching). **Use a pinned version in
production** to avoid unexpected updates and to ensure deterministic behavior.

## Changelog

This repository's [Releases page](https://github.com/Voa-Health/voa-plugin-dist/releases)
is the **public changelog** for the Voa plugin. Each release corresponds to a
`voa-integrations` version and documents the changes shipped in that `plugin.js`.

## Integration documentation

Full integration docs — installation, configuration, events, structured output,
and model selection — live at
[docs.voa.health](https://docs.voa.health) (plugin section).

## License & support

This distribution is provided by [Voa Health](https://voa.health). For
integration support or to report issues, please contact your Voa account manager
or open a ticket at the relevant support channel. Issues in this repository are
not monitored — the source is private.
