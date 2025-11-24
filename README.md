# Quick Automate Labs Guide

A comprehensive workshop guide built with AWS Cloudscape Design System for Amazon Quick Suite - Quick Automate hands-on labs.

## Overview

This project provides an interactive, self-paced learning experience for AWS Quick Automate. It features a responsive web interface with markdown-based content management, image galleries with lightbox viewing, and seamless navigation between modules.

## Features

- 🎨 AWS Cloudscape Design System styling
- 📱 Responsive layout that scales with screen size
- 🖼️ Image lightbox for full-size viewing
- 📋 Copy buttons for inline code snippets
- 🔄 Previous/Next navigation with auto-scroll to top
- 📝 Markdown-based content management with HTML support
- 🎬 Video embedding support (HTML5 and iframe)
- 💬 Block quotes and comment support
- 🌐 Ready for AWS Amplify deployment

## Project Structure

```
.
├── index.html                    # Main page with Cloudscape components
├── content/                      # Markdown content files
│   ├── introduction.md           # Workshop introduction
│   ├── prerequisites.md          # Prerequisites overview
│   ├── prerequisites-step1.md    # S3 & IAM Access Setup
│   ├── prerequisites-step2.md    # Amazon S3 connector configuration
│   ├── prerequisites-step3.md    # Amazon Bedrock connector configuration
│   ├── prerequisites-step4.md    # Microsoft Outlook connector (Optional)
│   ├── module1.md                # Module 1 - Quick Automate Getting Started
│   ├── module2.md                # Module 2 - Advanced workflows
│   └── fnol.md                   # Advanced Module (Optional)
├── images/                       # Image and GIF assets (50+ images)
└── README.md                     # This file
```

## Content Modules

### Getting Started
- Introduction to AWS Quick Automate

### Prerequisites
- S3 & IAM Access Setup
- Amazon S3 connector configuration
- Amazon Bedrock connector configuration
- Microsoft Outlook connector setup (optional)

### Modules
- **Module 1**: Amazon Quick Automate Getting Started
- **Module 2**: Advanced automation workflows and deployment

### Optional
- Advanced Module with FNOL (First Notice of Loss) examples

## Local Development

### Prerequisites
- Python 3.x
- Web browser (Chrome, Firefox, Safari, Edge)

### Setup

1. Clone the repository:
```bash
git clone https://github.com/inarongrit/quick-automate-labs-guide.git
cd quick-automate-labs-guide
```

2. Start a local web server:
```bash
python3 -m http.server 8000
```

3. Open http://localhost:8000 in your browser

## Markdown Features Supported

### Text Formatting
- **Bold**: `**text**`
- **Italic**: `*text*`
- **Code**: `` `code` `` (includes copy button)
- **Code blocks**: ` ```language ... ``` `

### Content Elements
- **Links**: `[text](url)`
- **Images**: `![alt](path)` or `<img src="path" style="width: 50%;" alt="alt">`
- **Lists**: `- item` or `1. item`
- **Block quotes**: `> quote`
- **Comments**: `<!-- hidden comment -->`

### Media
- **Videos**: `<video width="640" height="360" controls><source src="video.mp4" type="video/mp4"></video>`
- **YouTube embeds**: `<iframe width="640" height="360" src="https://www.youtube.com/embed/VIDEO_ID"></iframe>`
- **GIFs**: Same as images, supports `.gif` format

### Image Sizing
Use HTML for responsive sizing:
```html
<img src="images/your-image.png" style="width: 50%; height: auto;" alt="Description">
```

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
4. Use HTML for custom sizing: `<img src="images/image.png" style="width: 50%;" alt="Description">`

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

### AWS Amplify CLI

```bash
amplify init
amplify publish
```

## Recent Updates

- ✅ Auto-scroll to top on page navigation
- ✅ Block quote support for notes and callouts
- ✅ Video embedding capabilities (HTML5 and iframe)
- ✅ Image resizing with HTML syntax
- ✅ HTML comment support for hidden content
- ✅ Comprehensive Module 2 with workflow examples
- ✅ 50+ high-quality screenshots and GIFs
- ✅ Performance metrics and deployment guides

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contributing

To contribute to this workshop guide:

1. Create a new branch for your changes
2. Make your updates to markdown files or images
3. Test locally with `python3 -m http.server 8000`
4. Commit with descriptive messages
5. Push to GitHub and create a pull request

## Support

For issues or questions about the workshop content, please open an issue on GitHub.

---

**Last Updated**: November 24, 2025
**Version**: 1.0
**Status**: Production Ready
