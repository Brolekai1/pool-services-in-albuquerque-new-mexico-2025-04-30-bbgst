# Blue Desert Pool Landing Page - Maintenance Guide

This guide will help you maintain and customize the Blue Desert Pool landing page. It's designed for beginners with no prior coding experience.

## Table of Contents
- [Updating Text and Styling](#updating-text-and-styling)
- [Managing Links](#managing-links)
- [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
- [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains the company name and navigation menu:

```html
<a href="/" class="text-2xl font-bold text-blue-600">Blue Desert Pool</a>
```

To change the company name:
1. Locate this line in the header section
2. Replace "Blue Desert Pool" with your desired text
3. Keep the surrounding code intact

### Hero Section
The main headline and subtitle are in the hero section:

```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 mb-6">
    Pool Services in Albuquerque, New Mexico
</h1>
<p class="text-xl md:text-2xl text-gray-600 mb-12">
    Crystal-clear pools. Zero hassle.
</p>
```

To modify:
1. Find these elements within the `<section class="pt-32 pb-24...">` block
2. Update the text between the opening and closing tags
3. Maintain the existing classes for consistent styling

### Understanding Tailwind Classes
Common classes used in this page:

- Text sizes: `text-xl`, `text-2xl`, `text-4xl`
- Colors: `text-blue-600`, `text-gray-900`
- Spacing: `mb-6`, `py-24`, `px-6`
- Responsive prefixes: `md:`, `lg:`

Example of modifying text size:
```html
<!-- Original -->
<h3 class="text-xl font-semibold mb-4">Pool Maintenance</h3>

<!-- Modified to be larger -->
<h3 class="text-2xl font-semibold mb-4">Pool Maintenance</h3>
```

## Managing Links

### Navigation Menu Links
Current navigation links:
```html
<div class="hidden md:flex space-x-8">
    <a href="#services" class="text-gray-600 hover:text-blue-600 transition-colors duration-300">Services</a>
    <a href="#benefits" class="text-gray-600 hover:text-blue-600 transition-colors duration-300">Benefits</a>
    <a href="#faq" class="text-gray-600 hover:text-blue-600 transition-colors duration-300">FAQ</a>
    <a href="#contact" class="text-gray-600 hover:text-blue-600 transition-colors duration-300">Contact</a>
</div>
```

To update a link:
1. Locate the `<a>` tag you want to modify
2. Change the `href` attribute value
3. Update the text between the tags if needed

Example:
```html
<!-- Original -->
<a href="#services" class="text-gray-600 hover:text-blue-600 transition-colors duration-300">Services</a>

<!-- Modified -->
<a href="/services.html" class="text-gray-600 hover:text-blue-600 transition-colors duration-300">Our Services</a>
```

### External Links
The page contains these external links that need attention:
- Main CTA: `https://bluedesertpool.com`
- Email: `mailto:contact@astrve.com`

To update:
1. Find the relevant section
2. Replace the `href` value with your desired URL
3. Ensure the new URL includes the proper protocol (http://, https://, mailto:)

## Adding Privacy and Terms Pages

### Footer Links Setup
Current privacy and terms links in footer:
```html
<div>
    <h4 class="text-lg font-semibold mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

To link to new pages:
1. Create `privacy.html` and `terms.html` in your root directory
2. Update the href attributes:

```html
<li><a href="/privacy.html" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="/terms.html" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

## Troubleshooting

Common issues and solutions:

1. **Broken Internal Links**
   - Ensure all internal page links start with `/`
   - Check that section IDs match their corresponding links
   - Verify file names and paths are correct

2. **Styling Issues**
   - Don't remove `class` attributes
   - Keep responsive prefixes (`md:`, `lg:`)
   - Maintain spacing classes for layout

3. **Text Overflow**
   - When updating text, keep similar length to original
   - Use appropriate text size classes
   - Test on mobile and desktop views

For additional help:
- Reference the [Tailwind CSS documentation](https://tailwindcss.com/docs)
- Test all changes in multiple browsers
- Validate your HTML using [W3C Validator](https://validator.w3.org/)

Remember to always backup your files before making changes and test thoroughly after modifications.