# Personal Portfolio Website

A modern, responsive portfolio website built with HTML, CSS, and JavaScript. This website showcases your projects, skills, and personality in a creative and professional way.

## Features

- 🎨 **Modern Design**: Clean, professional design with smooth animations
- 📱 **Responsive**: Works perfectly on all devices (desktop, tablet, mobile)
- ⚡ **Fast & Lightweight**: Optimized for performance
- 🎯 **Interactive**: Smooth scrolling, hover effects, and animations
- 📧 **Contact Form**: Functional contact form with validation
- 🌟 **Particle Effects**: Beautiful animated particles in the hero section
- 📊 **Skills Showcase**: Visual representation of your technical skills
- 🚀 **Project Gallery**: Showcase your projects with detailed descriptions

## Sections

1. **Hero Section**: Eye-catching introduction with animated title
2. **About Section**: Personal information, interests, and statistics
3. **Projects Section**: Featured projects with technologies used
4. **Skills Section**: Technical skills organized by category
5. **Contact Section**: Contact form and social media links

## Customization Guide

### 1. Personal Information

Edit `index.html` to update your personal information:

```html
<!-- Update your name throughout the file -->
<h1 class="hero-title">Hi, I'm <span class="highlight">Your Name</span></h1>

<!-- Update the profile card -->
<div class="profile-info">
    <h3>Your Name</h3>
    <p>Developer & Designer</p>
</div>

<!-- Update contact information -->
<div class="contact-method">
    <i class="fas fa-envelope"></i>
    <div>
        <h4>Email</h4>
        <p>your.email@example.com</p>
    </div>
</div>
```

### 2. Projects

Replace the sample projects in the projects section with your own:

```html
<div class="project-card">
    <div class="project-image">
        <!-- Add your project screenshot here -->
        <img src="path/to/your/project-image.jpg" alt="Project Name">
    </div>
    <div class="project-content">
        <h3>Your Project Name</h3>
        <p>Description of your project and what it does.</p>
        <div class="project-tech">
            <span class="tech-tag">React</span>
            <span class="tech-tag">Node.js</span>
            <span class="tech-tag">MongoDB</span>
        </div>
        <div class="project-links">
            <a href="your-github-link" class="project-link">
                <i class="fab fa-github"></i> Code
            </a>
            <a href="your-live-link" class="project-link">
                <i class="fas fa-external-link-alt"></i> Live
            </a>
        </div>
    </div>
</div>
```

### 3. Skills

Update the skills section to reflect your actual skills:

```html
<div class="skills-category">
    <h3>Frontend</h3>
    <div class="skills-grid">
        <div class="skill-item">
            <i class="fab fa-react"></i>
            <span>React</span>
        </div>
        <!-- Add more skills -->
    </div>
</div>
```

### 4. Colors and Styling

Customize the color scheme in `styles.css`:

```css
/* Primary colors */
:root {
    --primary-color: #667eea;
    --secondary-color: #764ba2;
    --accent-color: #fbbf24;
    --text-color: #1f2937;
    --light-text: #6b7280;
}
```

### 5. About Section

Update the about section with your personal story:

```html
<div class="about-text">
    <h3>Who I Am</h3>
    <p>Your personal story and background...</p>
    
    <h3>What I Love</h3>
    <div class="interests">
        <div class="interest-item">
            <i class="fas fa-code"></i>
            <span>Your Interest</span>
        </div>
        <!-- Add more interests -->
    </div>
</div>
```

## Adding Images

1. Create an `images` folder in your project
2. Add your project screenshots and profile picture
3. Update the image paths in the HTML

## Deployment

### GitHub Pages (Free)

1. Push your code to a GitHub repository
2. Go to repository Settings > Pages
3. Select source branch (usually `main`)
4. Your site will be available at `https://username.github.io/repository-name`

### Netlify (Free)

1. Drag and drop your project folder to [Netlify](https://netlify.com)
2. Your site will be deployed instantly
3. You can connect your GitHub repository for automatic deployments

### Vercel (Free)

1. Install Vercel CLI: `npm i -g vercel`
2. Run `vercel` in your project directory
3. Follow the prompts to deploy

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## Performance Tips

1. **Optimize Images**: Compress images before adding them
2. **Minify CSS/JS**: Use tools to minify your files for production
3. **Use CDN**: Font Awesome and Google Fonts are already loaded from CDN
4. **Lazy Loading**: Images will be lazy-loaded automatically

## Customization Ideas

- Add a blog section
- Include testimonials
- Add a resume download button
- Include a timeline of your experience
- Add a dark mode toggle
- Include a portfolio filter (by technology, type, etc.)
- Add more animations and interactions

## File Structure

```
portfolioWebsite/
├── index.html          # Main HTML file
├── styles.css          # All CSS styles
├── script.js           # JavaScript functionality
├── README.md           # This file
└── images/             # Add your images here
    ├── profile.jpg
    ├── project1.jpg
    └── project2.jpg
```

## Getting Started

1. Clone or download this repository
2. Open `index.html` in your browser to see the website
3. Customize the content as described above
4. Deploy to your preferred platform

## Support

If you need help customizing your portfolio, feel free to:
- Check the comments in the code
- Look at the browser's developer tools for debugging
- Search for specific CSS properties or JavaScript functions

## License

This project is open source and available under the [MIT License](LICENSE).

---

**Happy coding! 🚀** 