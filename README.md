# Modern Landing Page - Maintenance Guide

This guide will help you customize and maintain your landing page, even if you're new to web development. Follow these detailed instructions to make updates while preserving the design and functionality.

## Table of Contents
- [Updating Text and Styling](#updating-text-and-styling)
- [Managing Links](#managing-links)
- [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
- [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains your logo and navigation menu. To update:

1. **Logo Text**: Find this line and replace "Logo" with your company name:
```html
<a href="#" class="text-2xl font-bold text-gray-900">Logo</a>
```

2. **Navigation Items**: Locate the navigation menu and update text as needed:
```html
<div class="hidden md:flex space-x-8">
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Home</a>
    <!-- Update other menu items similarly -->
</div>
```

### Hero Section
The main headline and subtext are in the hero section:

1. **Main Headline**: Update this text:
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 tracking-tight">
    Welcome to Our Modern Platform
</h1>
```

2. **Subheading**: Modify this paragraph:
```html
<p class="mt-6 text-xl text-gray-600 max-w-3xl mx-auto">
    Discover a new way to transform your digital experience...
</p>
```

### Tailwind CSS Tips
- Font sizes use classes like `text-xl`, `text-2xl`, etc.
- Colors use format `text-{color}-{shade}` (e.g., `text-gray-600`)
- Spacing uses `m-` (margin) or `p-` (padding) with numbers (e.g., `mt-6`)
- Responsive classes start with screen sizes: `md:` or `lg:`

## Managing Links

### Navigation Menu Links
1. Locate the navigation section in the header:
```html
<div class="hidden md:flex space-x-8">
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Home</a>
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Features</a>
    <!-- Continue for other links -->
</div>
```

2. Replace `#` with your actual URLs:
```html
<a href="index.html">Home</a>
<a href="features.html">Features</a>
```

### Call-to-Action (CTA) Links
Update the "Get Started" button link:
```html
<a href="signup.html" class="inline-flex items-center px-8 py-3...">
    Get Started
</a>
```

## Adding Privacy and Terms Pages

### Footer Legal Links
1. Locate the legal section in the footer:
```html
<div>
    <h3 class="text-white text-lg font-semibold mb-4">Legal</h3>
    <ul class="space-y-2">
        <li><a href="#" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="#" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

2. Update the links to point to your policy pages:
```html
<li><a href="privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

### Creating Policy Pages
1. Create new files named `privacy.html` and `terms.html`
2. Copy the header and footer from `index.html` to maintain consistent styling
3. Add your policy content between the header and footer

## Troubleshooting

### Common Issues and Solutions

1. **Broken Layout**
   - Check that all Tailwind CSS classes are spelled correctly
   - Verify that the Tailwind CDN link is working
   - Ensure all HTML tags are properly closed

2. **Missing Styles**
   - Confirm the Inter font is loading:
   ```html
   <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
   ```

3. **Links Not Working**
   - Verify file names match exactly (case-sensitive)
   - Ensure files are in the correct directory
   - Test all links after updating

### Need Help?
- Double-check the Tailwind CSS documentation for class names
- Use browser developer tools (F12) to inspect elements
- Keep a backup copy of the original HTML before making changes

Remember to test your changes across different devices and screen sizes to ensure the responsive design remains intact.