# CAFE Docs Content

Documentation content for the FFXIV CAFE community.

## About

This repository contains the source content for CAFE Docs. Pages are written in AsciiDoc and are built/published by the separate `cafe-docs` repository.

## Structure

```text
modules/ROOT/
  pages/      AsciiDoc documentation pages
  discord/    Optional Discord layout sidecars
  partials/   Reusable AsciiDoc snippets
  images/     Images and assets
  nav.adoc    Site navigation
```

## Editing Docs

The easiest way to edit is through the online editor on the docs site:

1. Open the page you want to edit.
2. Click `Edit this Page`.
3. Log in with Discord.
4. Edit the page and preview your changes.
5. Submit the PR from the editor.

You can also edit files directly in GitHub or clone this repository locally.

## AsciiDoc Pages

AsciiDoc pages live in:

```text
modules/ROOT/pages/
```

When adding or moving pages, update:

```text
modules/ROOT/nav.adoc
```

Use relative xrefs for internal links:

```asciidoc
xref:user-guide/joining-raids.adoc[Joining Raids]
```

## Discord Layouts

Some pages also have a custom Discord layout. These are stored as sidecar JSON files under:

```text
modules/ROOT/discord/
```

Example:

```text
modules/ROOT/pages/start-here/the-rules.adoc
modules/ROOT/discord/start-here/the-rules.json
```

If a sidecar exists, Discord publishing uses that layout instead of deriving the Discord message from the AsciiDoc page.

The editor can submit PRs that change the AsciiDoc page, the Discord sidecar, or both. The Discord editor uses a block builder for Components v2 layouts, with raw JSON available only as an advanced view.

## Related Repositories

- `cafe-docs` - build system, editor, and Discord publisher
- `cafe-docs-source` - this content repository

## License

MIT License - see LICENSE file for details.

## Community

Join us on Discord: [CAFE](https://discord.gg/c-a-f-e)
