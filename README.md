# Quick Automate Labs Guide

A workshop guideline page built with AWS Cloudscape Design System for Amazon Quick Suite - Quick Automate hands-on labs.

## Features

- 🎨 AWS Cloudscape Design System styling
- 📱 Responsive layout that scales with screen size
- 🖼️ Image lightbox for full-size viewing
- 📋 Copy buttons for inline code snippets
- 🔄 Previous/Next navigation buttons
- 📝 Markdown-based content management
- 🌐 Ready for AWS Amplify deployment

## Structure

```
.
├── index.html              # Main page with Cloudscape components
├── content/                # Markdown content files
│   ├── introduction.md
│   ├── prerequisites.md
│   ├── prerequisites-step1.md
│   ├── prerequisites-step2.md
│   ├── prerequisites-step3.md
│   ├── module1.md
│   ├── module2.md
│   └── cleanup.md
├── images/                 # Image assets
└── README.md
```

## Local Development

1. Start a local web server:

```bash
python3 -m http.server 8000
```

2. Open http://localhost:8000 in your browser

## Customization

### Update Workshop Content

Edit markdown files in the `content/` directory with your workshop instructions.

### Configure Navigation

Update the `config` object in `index.html` (around line 54):

```javascript
const config = {
    title: "Workshop Title",        // Top navigation bar
    subtitle: "Workshop Subtitle",  // Sidebar header
    sections: [
        {
            title: "Section Name",
            items: [
                { title: "Page Title", file: "content/page.md" },
                { title: "Sub-item", file: "content/sub.md", indent: true }
            ]
        }
    ]
};
```

### Add Images

1. Place images in the `images/` directory
2. Reference in markdown: `![Description](images/your-image.jpg)`
3. Click images to view full-size in lightbox

### Markdown Features

- **Bold**: `**text**`
- **Italic**: `*text*`
- **Code**: `` `code` `` (includes copy button)
- **Code blocks**: ` ```language ... ``` `
- **Links**: `[text](url)`
- **Images**: `![alt](path)`
- **Lists**: `- item` or `1. item`
- **Quotes**: `> quote`

## Deployment

### AWS Amplify (Recommended)

1. Push code to GitHub
2. Go to AWS Amplify Console
3. Connect your GitHub repository
4. Deploy automatically on every push

### S3 + CloudFront

1. Upload files to S3 bucket
2. Enable static website hosting
3. Configure CloudFront distribution
4. Set up SSL certificate

## License

This project is licensed under the MIT License - see the LICENSE file for details.

