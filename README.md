# Workshop Guide

A simple workshop guideline page built with AWS Cloudscape Design System.

## Structure

```
.
├── index.html          # Main page with Cloudscape components
├── content/            # Markdown content files
│   ├── introduction.md
│   ├── prerequisites.md
│   ├── module1.md
│   ├── module2.md
│   └── cleanup.md
└── README.md
```

## Usage

1. Update the configuration in `index.html` (lines 28-50) to match your workshop structure
2. Edit or add markdown files in the `content/` directory
3. Serve the files with a local web server:

```bash
python3 -m http.server 8000
```

4. Open http://localhost:8000 in your browser

## Customization

- Edit `config` object in `index.html` to add/remove sections and modules
- Update markdown files in `content/` directory with your workshop content
- Modify styles in the `<style>` section for custom branding
