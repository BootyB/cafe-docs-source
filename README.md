# CAFE Docs Content

Documentation content for the FFXIV CAFE community.

## 📚 About

This repository contains the documentation source files (AsciiDoc) for CAFE. The content is built and published using [Antora](https://antora.org/) from the main [cafe-docs](https://github.com/BootyB/cafe-docs) repository.

## 📁 Structure

This is an Antora documentation component with the following structure:

- `antora.yml` - Component descriptor defining the component name, version, and navigation
- `modules/ROOT/` - Main documentation module
  - `pages/` - Documentation pages (AsciiDoc format)
  - `partials/` - Reusable content snippets
  - `images/` - Images and assets
  - `nav.adoc` - Navigation structure

## ✏️ Contributing

### Editing Documentation

The easiest way to edit documentation is through our **online editor** at https://cafe-docs.vercel.app/

- Click the "Edit" button on any documentation page
- Make your changes in the browser-based editor
- Preview your changes in real-time
- Submit your changes directly (requires GitHub authentication)

**Alternative methods:**

- Edit files directly on GitHub
- Clone this repository locally:
  ```bash
  git clone https://github.com/{your-org}/cafe-docs-content.git
  cd cafe-docs-content
  ```

### File Format

All documentation is written in [AsciiDoc](https://docs.asciidoctor.org/asciidoc/latest/). Key conventions:

- Use `.adoc` extension for all pages
- Follow the existing structure in `modules/ROOT/pages/`
- Update `modules/ROOT/nav.adoc` when adding new pages
- Use relative xrefs for internal links: `xref:user-guide/joining-raids.adoc[Joining Raids]`

### Preview Changes

**Online Editor (Recommended)**  
The built-in editor at https://cafe-docs.vercel.app/ provides instant preview as you type. Simply click "Edit" on any page to get started.

**Local Preview**  
To preview locally, you'll need to build with Antora. See the main [cafe-docs](https://github.com/BootyB/cafe-docs) repository for build instructions.

## 🔗 Related Repositories

- [cafe-docs](https://github.com/BootyB/cafe-docs) - Main documentation site builder and editor
- Build output is published to: https://cafe-docs.vercel.app/

## 📝 License

MIT License - see LICENSE file for details.

## 💬 Community

Join us on Discord: [CAFE](https://discord.gg/c-a-f-e)
