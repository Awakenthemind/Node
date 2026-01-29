# Node Landing Page

A modern, minimalist landing page built with Tailwind CSS, GSAP animations, and Cal.com integration.

## Features

- 🎨 **Stripe-like Minimalism** - Clean, professional design with subtle shadows and generous whitespace
- ✨ **GSAP Animations** - Staggered page load timeline and scroll-triggered animations
- 🌌 **Anti-Gravity Particle System** - 60 interactive particles with network connections
- 📱 **Fully Responsive** - Mobile-first design with proper breakpoints
- 📅 **Cal.com Integration** - Direct booking integration
- 🔒 **Glassmorphism UI** - Modern frosted glass effects
- ⚡ **Performance Optimized** - GSAP ticker for efficient animations

## Tech Stack

- **Tailwind CSS** - Utility-first CSS framework
- **GSAP** - Professional-grade animation library
- **Lucide Icons** - Beautiful, consistent iconography
- **Cal.com** - Embedded booking system
- **Vercel** - Deployment platform

## Local Development

1. Clone the repository:
```bash
git clone https://github.com/Awakenthemind/Node.git
cd Node
```

2. Open `index.html` in your browser or use a local server:
```bash
npx serve
```

## Deployment

### Deploy to Vercel (Recommended)

1. **Via GitHub Integration:**
   - Go to [vercel.com](https://vercel.com)
   - Click "Import Project"
   - Select this GitHub repository
   - Click "Deploy"

2. **Via Vercel CLI:**
```bash
npm install -g vercel
vercel --prod
```

## Project Structure

```
node-landing/
├── index.html              # Main landing page
├── package.json            # Project metadata
├── vercel.json             # Vercel configuration
├── .gitignore              # Git ignore rules
├── *.svg                   # Icon assets
└── Hero Images/            # Hero graphics
```

## Features Breakdown

### Journey-Based Features
1. **Built for Speed** - Optimized for instant loading
2. **Easy to Maintain** - Clean, scalable code
3. **Safe & Secure** - Industry-standard security

### Animations
- Staggered page load (nav → badge → headline → CTA)
- Scroll-triggered feature cards
- Contact form reveal
- Footer fade-in
- Particle system with mouse interaction

### Responsive Design
- Mobile: `px-4`, `text-4xl`, `grid-cols-1`
- Tablet: `md:px-6`, `md:text-6xl`, `md:grid-cols-3`
- Desktop: `lg:text-7xl`, generous spacing

## Cal.com Setup

The booking integration is configured for: `alex-c5ns68/30min`

To update:
1. Find `data-cal-link` attributes in `index.html`
2. Replace with your Cal.com username/event

## Future Enhancements

### Contact Form Backend
To make the form functional, add an API endpoint:

```javascript
// api/send.js
import { Resend } from 'resend';

export default async function handler(req, res) {
  // Email sending logic
}
```

Set environment variables in Vercel:
- `RESEND_API_KEY`
- `RECIPIENT_EMAIL`

## License

MIT

## Contact

For inquiries, use the contact form on the landing page.
