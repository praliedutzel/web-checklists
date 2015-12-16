# WordPress Pre-Launch Checklist
The following is a checklist of items to check prior to launching a new WordPress site. It does not include things like cross-browser and device testing, build processes, concatenation and minification, etc.

## General
- [ ] Remove absolute links to media files and pages (or update to correct path)
- [ ] Set copyright date using PHP's date function
- [ ] Load jQuery in the footer from a CDN
- [ ] Add favicons

## Pages
- [ ] Ensure all pages are working properly and using the correct template
- [ ] Create a 404 page
- [ ] Create category pages
- [ ] Create search pages
- [ ] Ensure any custom post types are accessible

## Digital Marketing & SEO
- [ ] Create a robots.txt file
- [ ] Add Google Tag Manager script
- [ ] Install and setup [Yoast SEO](https://wordpress.org/plugins/wordpress-seo/) plugin
- [ ] Each page has an `<h1>` tag and headlines are used properly
- [ ] Add Open Graph and Twitter Card meta tags *(can be done via Yoast SEO plugin)*

## Accessibility
- [ ] All images have an `alt=""` attribute
- [ ] Form fields have associated labels
- [ ] All links, buttons, form fields, and other clickable media have a focus state

## Theme Config
- [ ] Add theme information in style.css
- [ ] Create a screenshot (880x660 PNG)
- [ ] Styles and scripts are enqueued
- [ ] Add support for featured images (if using)
- [ ] Add support for WordPress menus
- [ ] Add WordPress' [standard CSS classes](https://codex.wordpress.org/CSS#WordPress_Generated_Classes)

## WordPress Settings
### General
- [ ] Set the site title
- [ ] Add a tagline
- [ ] Set your timezone
- [ ] Select a date and time format

### Writing
- [ ] Set a default post category

### Reading
- [ ] Set the front page to display as the homepage
- [ ] Uncheck the "Search Engine Visibility" box for production site

### Permalinks
- [ ] Set the permalink structure

## Cleanup
- [ ] Delete unused plugins
- [ ] Delete unused templates
- [ ] Delete WordPress' default posts, pages, and comments
- [ ] Delete unused or duplicated media files
- [ ] Delete test user accounts
- [ ] Turn off debugging
- [ ] Remove any console logs, alerts, or var_dumps
- [ ] Concatenate and minify CSS and JS files where possible
- [ ] Move custom post types from functions into their own plugin *(to prevent data loss on theme change)*