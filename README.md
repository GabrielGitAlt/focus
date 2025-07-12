# FOCUS - Future Opportunities and Career Understanding for Students

A Jekyll-based website for FOCUS, a non-profit organization providing career exploration and guidance for students.

## Features

- Modern, responsive design with Bootstrap 5
- Green color palette optimized for accessibility
- Career exploration sections covering various fields
- Contact form for inquiries
- Testimonials section
- Social media integration

## File Structure

```
focus/
├── _config.yml          # Jekyll configuration
├── _layouts/            # Jekyll layouts
│   └── default.html     # Default page layout
├── _includes/           # Reusable components
│   ├── navigation.html  # Navigation bar
│   └── footer.html      # Footer
├── assets/              # Static assets
│   └── images/         # Images
│       └── landing.webp # Hero image
├── styles/              # Stylesheets
│   ├── styles.css      # Main stylesheet
│   └── about.css       # About page styles
├── _pages/              # Jekyll pages collection
│   ├── index.html     # Home page
│   └── about.html     # About page
├── Gemfile            # Ruby dependencies
└── README.md          # This file
```

## Getting Started

### Prerequisites

- Ruby (version 2.6.0 or higher)
- RubyGems
- GCC and Make

### Installation

1. Clone the repository:

   ```bash
   git clone <repository-url>
   cd focus
   ```

2. Install Jekyll and other dependencies:

   ```bash
   bundle install
   ```

3. Start the Jekyll development server:

   ```bash
   bundle exec jekyll serve
   ```

4. Open your browser and navigate to `http://localhost:4000`

### Building for Production

To build the site for production:

```bash
bundle exec jekyll build
```

The built site will be in the `_site` directory.

## Customization

### Colors

The site uses CSS custom properties for easy color customization. The main colors are defined in `styles/styles.css`:

- `--primary-color`: Deep green accent (#226633)
- `--secondary-color`: Light beige/earthy background (#f1f5ee)
- `--tertiary-color`: Light green background (#e3f2e8)
- `--dark-color`: Dark green for text (#184422)

### Content

- Update the main content in `index.html`
- Modify navigation links in `_includes/navigation.html`
- Update footer information in `_includes/footer.html`
- Add new pages by creating HTML files with front matter

### Images

Place new images in the `assets/images/` directory and reference them using Jekyll's `relative_url` filter:

```html
<img
  src="{{ '/assets/images/your-image.jpg' | relative_url }}"
  alt="Description"
/>
```

## Deployment

This Jekyll site can be deployed to:

- GitHub Pages
- Netlify
- Vercel
- Any static hosting service

For GitHub Pages, simply push to a repository and enable GitHub Pages in the repository settings.

## Support

For questions or support, please contact: focusnonprofit24@gmail.com
