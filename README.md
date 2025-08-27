# Decoded Ventures ERP API Documentation

This directory contains the API documentation for the Decoded Ventures ERP API, built with [Mintlify](https://mintlify.com/).

## 🚀 Features

- **Comprehensive API Documentation**: Complete coverage of all ERP API endpoints
- **Interactive Examples**: Code examples in multiple programming languages
- **Search & Navigation**: Easy-to-use search and navigation
- **Responsive Design**: Works on desktop and mobile devices
- **Dark/Light Mode**: Automatic theme switching
- **Version Control**: Track API changes and versions

## 📁 Structure

```
apps/api-docs/
├── mint.json              # Mintlify configuration
├── introduction.mdx       # Main introduction page
├── authentication.mdx     # Authentication guide
├── payments/              # Payment API documentation
│   ├── mpesa.mdx
│   ├── flick.mdx
│   └── flutterwave.mdx
├── modules/               # ERP module documentation
│   ├── finance.mdx
│   ├── sales.mdx
│   ├── hr.mdx
│   ├── support.mdx
│   ├── logistics.mdx
│   └── legal.mdx
├── agents/                # AI agents documentation
│   ├── overview.mdx
│   ├── voice.mdx
│   ├── sales.mdx
│   ├── finance.mdx
│   ├── hr.mdx
│   ├── support.mdx
│   ├── logistics.mdx
│   └── customer-success.mdx
├── integrations/          # Integration documentation
│   ├── credentials.mdx
│   ├── openai.mdx
│   ├── claude.mdx
│   ├── google-ai.mdx
│   ├── twilio.mdx
│   └── sendgrid.mdx
├── sdks/                  # SDK documentation
│   ├── javascript.mdx
│   ├── python.mdx
│   ├── php.mdx
│   └── java.mdx
├── examples/              # Code examples
│   ├── quickstart.mdx
│   ├── payment-integration.mdx
│   ├── ai-agents.mdx
│   └── webhooks.mdx
├── assets/                # Static assets
│   ├── logo/
│   │   ├── dark.svg
│   │   └── light.svg
│   ├── favicon.png
│   └── background.png
└── package.json
```

## 🛠️ Setup

### Prerequisites

- Node.js 18 or higher
- npm or yarn

### Installation

1. Install dependencies:
```bash
npm install
```

2. Start the development server:
```bash
npm run dev
```

3. Open your browser and navigate to `http://localhost:3000`

## 📝 Adding Documentation

### Creating New Pages

1. Create a new `.mdx` file in the appropriate directory
2. Add frontmatter with title and description:

```mdx
---
title: 'Page Title'
description: 'Page description for SEO'
---

# Page Title

Your content here...
```

3. Update the navigation in `mint.json` to include the new page

### Code Examples

Use code blocks with language specification:

```javascript
// JavaScript example
const api = new DecodedVenturesAPI({
  apiKey: 'your-api-key'
});
```

```python
# Python example
from decodedventures import DecodedVenturesAPI

api = DecodedVenturesAPI(api_key='your-api-key')
```

### API Endpoints

Document API endpoints with proper formatting:

```http
POST /api/endpoint
Content-Type: application/json
Authorization: Bearer YOUR_API_KEY

{
  "key": "value"
}
```

## 🚀 Deployment

### Local Build

```bash
npm run build
```

### Deploy to Mintlify

1. Install Mintlify CLI:
```bash
npm install -g mintlify
```

2. Login to Mintlify:
```bash
mintlify login
```

3. Deploy:
```bash
npm run deploy
```

### Continuous Deployment

The documentation is automatically deployed when changes are pushed to the main branch.

## 🎨 Customization

### Branding

Update the `mint.json` file to customize:

- **Colors**: Primary, light, and dark theme colors
- **Logo**: Dark and light mode logos
- **Favicon**: Browser favicon
- **Background**: Background image

### Navigation

Modify the `navigation` array in `mint.json` to organize pages into groups:

```json
{
  "navigation": [
    {
      "group": "Getting Started",
      "pages": [
        "introduction",
        "authentication"
      ]
    }
  ]
}
```

### Social Links

Add social media links in the `footerSocials` section:

```json
{
  "footerSocials": {
    "twitter": "https://twitter.com/decodedventures",
    "github": "https://github.com/decodedventures"
  }
}
```

## 📚 Documentation Standards

### Writing Guidelines

1. **Clear and Concise**: Write clear, easy-to-understand documentation
2. **Code Examples**: Provide working code examples in multiple languages
3. **Error Handling**: Document common errors and solutions
4. **Best Practices**: Include security and performance best practices
5. **Consistent Formatting**: Use consistent formatting and structure

### API Documentation

For each API endpoint, include:

- **HTTP Method and URL**
- **Request Headers**
- **Request Body** (if applicable)
- **Response Format**
- **Error Codes**
- **Code Examples**
- **Rate Limits**

### Code Examples

Provide examples in:

- JavaScript/TypeScript
- Python
- PHP
- Java
- cURL

## 🔧 Configuration

### Environment Variables

Create a `.env` file for local development:

```env
MINTLIFY_API_KEY=your_mintlify_api_key
```

### Mintlify Configuration

The `mint.json` file contains all Mintlify-specific configuration:

- **Site Information**: Name, description, branding
- **Navigation**: Page organization and structure
- **Social Links**: Footer social media links
- **Customization**: Colors, logos, and styling

## 🐛 Troubleshooting

### Common Issues

1. **Build Errors**: Check for syntax errors in MDX files
2. **Navigation Issues**: Verify page paths in `mint.json`
3. **Styling Problems**: Check color values and asset paths
4. **Deployment Failures**: Ensure Mintlify API key is valid

### Getting Help

- **Mintlify Docs**: [docs.mintlify.com](https://docs.mintlify.com)
- **GitHub Issues**: Create an issue in the repository
- **Support**: Contact support@decodedventures.com

## 📄 License

This documentation is licensed under the MIT License. See the LICENSE file for details.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test locally with `npm run dev`
5. Submit a pull request

## 📞 Support

- **Email**: support@decodedventures.com
- **Discord**: [Join our community](https://discord.gg/decodedventures)
- **Documentation**: [docs.decodedventures.com](https://docs.decodedventures.com)
