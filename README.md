# Chun Lin - Portfolio Website

A modern, responsive portfolio website for Chun Lin, showcasing his work as a software engineer and photographer. Built with React, Framer Motion, and modern web technologies.

## 🚀 Features

- **Modern Design**: Clean, professional design with dark theme and gradient accents
- **Responsive Layout**: Fully responsive design that works on all devices
- **Smooth Animations**: Beautiful animations powered by Framer Motion
- **Interactive Elements**: Hover effects, smooth scrolling, and interactive components
- **Photography Gallery**: Filterable photo gallery with lightbox modal
- **Contact Form**: Functional contact form with validation
- **SEO Optimized**: Proper meta tags and semantic HTML structure

## 🛠️ Technologies Used

- **React 18** - Modern React with hooks and functional components
- **Framer Motion** - Smooth animations and transitions
- **Lucide React** - Beautiful icon library
- **CSS3** - Modern CSS with Grid, Flexbox, and custom properties
- **React Router** - Client-side routing
- **Responsive Design** - Mobile-first approach

## 📁 Project Structure

```
src/
├── components/
│   ├── Navbar.js          # Navigation component
│   ├── Hero.js            # Hero section
│   ├── About.js           # About section
│   ├── Skills.js          # Skills section
│   ├── Projects.js        # Projects showcase
│   ├── Photography.js     # Photography gallery
│   ├── Contact.js         # Contact form
│   ├── Footer.js          # Footer component
│   └── *.css              # Component styles
├── App.js                 # Main app component
├── index.js              # App entry point
└── index.css             # Global styles
```

## 🎨 Sections

1. **Hero Section** - Introduction with call-to-action buttons
2. **About** - Personal information and interests
3. **Skills** - Technical skills with animated progress bars
4. **Projects** - Software engineering projects showcase
5. **Photography** - Photo gallery with filtering and lightbox
6. **Contact** - Contact form and information
7. **Footer** - Social links and quick navigation

## 🚀 Getting Started

### Prerequisites

- Node.js (version 14 or higher)
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/ChunPortfolio.git
cd ChunPortfolio
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm start
```

4. Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

### Building for Production

```bash
npm run build
```

This creates a `build` folder with optimized production files.

## 🌐 GitHub Pages Deployment

This project is configured for GitHub Pages deployment. Follow these steps to deploy:

### 1. Update Homepage URL

In `package.json`, update the homepage field with your GitHub username:

```json
{
  "homepage": "https://yourusername.github.io/ChunPortfolio"
}
```

### 2. Install gh-pages

The gh-pages package is already included in devDependencies.

### 3. Deploy

```bash
npm run deploy
```

This will:
- Build the project
- Deploy it to the `gh-pages` branch
- Make it available at `https://yourusername.github.io/ChunPortfolio`

### 4. Configure GitHub Pages

1. Go to your repository on GitHub
2. Navigate to Settings > Pages
3. Set Source to "Deploy from a branch"
4. Select the `gh-pages` branch
5. Save the settings

Your portfolio will be live at `https://yourusername.github.io/ChunPortfolio`

## 🎯 Customization

### Personal Information
Update the following files to customize personal information:
- `src/components/Hero.js` - Hero section content
- `src/components/About.js` - About section content
- `src/components/Contact.js` - Contact information
- `src/components/Projects.js` - Project details
- `src/components/Photography.js` - Photo gallery

### Styling
- Global styles: `src/index.css`
- Component-specific styles: `src/components/*.css`
- Color scheme: Update CSS custom properties in component files

### Images
Replace placeholder images with actual photos:
- Project images in `src/components/Projects.js`
- Photography images in `src/components/Photography.js`

## 📱 Responsive Design

The website is fully responsive and optimized for:
- Desktop (1200px+)
- Tablet (768px - 1199px)
- Mobile (320px - 767px)

## 🌟 Key Features

### Animations
- Scroll-triggered animations using Framer Motion
- Smooth page transitions
- Interactive hover effects
- Loading animations

### Performance
- Optimized images and assets
- Lazy loading for better performance
- Efficient CSS with modern techniques

### Accessibility
- Semantic HTML structure
- Proper ARIA labels
- Keyboard navigation support
- Screen reader friendly

## 📧 Contact

For questions or support, please contact:
- Email: chun.lin@email.com
- LinkedIn: [LinkedIn Profile]
- GitHub: [GitHub Profile]

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- [Unsplash](https://unsplash.com) for placeholder images
- [Lucide](https://lucide.dev) for beautiful icons
- [Framer Motion](https://www.framer.com/motion/) for animations
- [Google Fonts](https://fonts.google.com) for typography

---

Made with ❤️ and lots of ☕ by Chun Lin
