# ExploreX - Smart Tour Planning Website

A modern, fully responsive tour planning website built with HTML5, Tailwind CSS, and Vanilla JavaScript. Features smooth animations, mobile-first design, and professional UI/UX.

![ExploreX Banner](https://images.unsplash.com/photo-1488646953014-85cb44e25828?w=1200&q=80)

## 🌟 Features

- **Fully Responsive Design** - Mobile, tablet, and desktop optimized
- **Modern UI/UX** - Clean, professional travel startup aesthetic
- **Smooth Animations** - Fade-in effects on scroll using Intersection Observer
- **Interactive Navigation** - Sticky navbar with mobile hamburger menu
- **Form Validation** - Real-time client-side validation with user feedback
- **SEO Optimized** - Semantic HTML, meta tags, and proper heading structure
- **Performance Optimized** - CDN images, minimal dependencies
- **Accessibility** - ARIA labels, keyboard navigation, focus states

## 📁 Project Structure

```
tourpage/
├── index.html              # Main HTML file
├── assets/
│   ├── css/
│   │   └── style.css      # Custom CSS styles
│   └── js/
│       └── main.js        # JavaScript functionality
└── README.md              # Documentation
```

## 🎨 Sections

1. **Navbar** - Sticky navigation with mobile menu toggle
2. **Hero Section** - Full-screen banner with CTA buttons
3. **Popular Destinations** - 6 destination cards in responsive grid
4. **Tour Packages** - 3 pricing tiers with recommended highlight
5. **Why Choose Us** - 4 feature cards with icons
6. **Testimonials** - 3 client reviews with ratings
7. **Contact Form** - Validated contact form
8. **Footer** - Quick links, social icons, contact info

## 🚀 How to Run Locally

### Option 1: Direct File Opening
1. Navigate to the project folder
2. Double-click `index.html` to open in your default browser

### Option 2: Using Live Server (Recommended)
1. Install [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) extension in VS Code
2. Right-click on `index.html`
3. Select "Open with Live Server"

### Option 3: Using Python HTTP Server
```bash
# Python 3
cd tourpage
python -m http.server 8000

# Open browser to http://localhost:8000
```

### Option 4: Using Node.js HTTP Server
```bash
# Install http-server globally
npm install -g http-server

# Run server
cd tourpage
http-server -p 8000

# Open browser to http://localhost:8000
```

## 🌐 Deployment on Netlify

### Method 1: Drag & Drop (Easiest)
1. Go to [Netlify](https://www.netlify.com/)
2. Sign up or log in
3. Drag the `tourpage` folder to the Netlify dashboard
4. Your site will be live instantly!

### Method 2: Git Integration
1. Create a GitHub repository
2. Push your code:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin <your-repo-url>
   git push -u origin main
   ```
3. Go to Netlify and click "New site from Git"
4. Connect your GitHub repository
5. Configure build settings:
   - **Build command:** Leave empty
   - **Publish directory:** `.` (current directory)
6. Click "Deploy site"

### Method 3: Netlify CLI
```bash
# Install Netlify CLI
npm install -g netlify-cli

# Navigate to project
cd tourpage

# Deploy
netlify deploy

# For production deployment
netlify deploy --prod
```

## 🎨 Customization Guide

### Change Colors
Edit the Tailwind config in `index.html`:
```javascript
tailwind.config = {
    theme: {
        extend: {
            colors: {
                primary: '#0891b2',    // Change this
                secondary: '#0e7490',  // Change this
                accent: '#06b6d4',     // Change this
            }
        }
    }
}
```

### Update Images
Replace Unsplash URLs in `index.html` with your own images:
```html
<!-- Example -->
<img src="https://images.unsplash.com/photo-..." alt="...">
<!-- Replace with -->
<img src="assets/images/your-image.jpg" alt="...">
```

### Modify Content
- **Company Name:** Search and replace "ExploreX" in `index.html`
- **Destinations:** Edit destination cards in the Destinations section
- **Packages:** Update pricing and features in the Packages section
- **Contact Info:** Update email, phone, and address in the Footer

### Add Google Analytics
Add before closing `</head>` tag in `index.html`:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

## 🔧 Technologies Used

- **HTML5** - Semantic markup
- **Tailwind CSS** - Utility-first CSS framework (via CDN)
- **Vanilla JavaScript** - No frameworks, pure JS
- **Google Fonts** - Poppins font family
- **Font Awesome** - Icon library
- **Unsplash** - High-quality images

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 🚀 Future Enhancements

### Backend Integration Ideas
1. **Contact Form Backend**
   - Integrate with [Formspree](https://formspree.io/) or [EmailJS](https://www.emailjs.com/)
   - Add Node.js/Express backend with email service
   - Use serverless functions (Netlify Functions, AWS Lambda)

2. **Booking System**
   - Add booking functionality with payment gateway (Stripe, PayPal)
   - Implement date picker for travel dates
   - Create booking confirmation emails

3. **User Authentication**
   - Add user registration and login
   - Create user dashboard for managing bookings
   - Implement social login (Google, Facebook)

4. **Content Management**
   - Integrate with headless CMS (Strapi, Contentful, Sanity)
   - Allow admin to manage destinations and packages
   - Add blog section for travel tips

5. **Advanced Features**
   - Real-time chat support
   - Multi-language support (i18n)
   - Currency converter
   - Weather API integration
   - Interactive maps (Google Maps, Mapbox)
   - Review and rating system
   - Newsletter subscription

6. **Database Integration**
   - MongoDB for storing bookings and user data
   - PostgreSQL for relational data
   - Firebase for real-time features

7. **Performance Optimization**
   - Implement lazy loading for images
   - Add service worker for offline support
   - Convert to Progressive Web App (PWA)
   - Optimize images with WebP format

## 📄 License

This project is open source and available for personal and commercial use.

## 👨‍💻 Developer

Built with ❤️ by a Senior Frontend Developer

---

**Need Help?** Open an issue or contact support at info@explorex.com

**Live Demo:** [Coming Soon]

**Version:** 1.0.0
