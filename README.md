# Dhauladhar Candles Website

A modern, beautiful e-commerce website for Dhauladhar Candles, built with Astro and Tailwind CSS. Inspired by premium candle studio websites like Brooklyn Candle Studio.

## Features

- 🎨 **Modern Design**: Clean, elegant design with beautiful typography and spacing
- 📱 **Fully Responsive**: Works perfectly on all devices (mobile, tablet, desktop)
- 🛒 **Shopping Cart**: Full cart functionality with localStorage persistence
- 🏠 **Homepage**: Hero section with featured products and call-to-action sections
- 🛍️ **Product Pages**: Individual product detail pages with related products
- 📄 **Additional Pages**: About, Contact, and Shop pages
- ⚡ **Fast Performance**: Built with Astro for optimal performance
- 🎯 **SEO Friendly**: Proper meta tags and semantic HTML

## Tech Stack

- [Astro](https://astro.build/) - The web framework
- [Tailwind CSS](https://tailwindcss.com/) - For styling
- TypeScript - For type safety

## Getting Started

### Prerequisites

- Node.js 18.20.8 or higher (or Node.js 20.3.0+)
- npm 9.6.5 or higher

### Installation

1. Install dependencies:
```bash
npm install
```

2. Start the development server:
```bash
npm run dev
```

3. Open your browser and visit `http://localhost:4321`

### Build for Production

```bash
npm run build
```

This will create a `dist/` folder with your production-ready site.

### Preview Production Build

```bash
npm run preview
```

## Project Structure

```
/
├── public/
│   └── favicon.svg
├── src/
│   ├── components/
│   │   ├── Header.astro      # Navigation header with cart
│   │   ├── Footer.astro      # Site footer
│   │   └── ProductCard.astro # Product card component
│   ├── data/
│   │   └── products.ts        # Product data
│   ├── layouts/
│   │   └── Layout.astro      # Base layout
│   └── pages/
│       ├── index.astro        # Homepage
│       ├── shop.astro         # Shop page
│       ├── cart.astro         # Shopping cart
│       ├── about.astro        # About page
│       ├── contact.astro      # Contact page
│       └── products/
│           └── [id].astro     # Product detail page
├── astro.config.mjs
├── tailwind.config.mjs
└── package.json
```

## Features in Detail

### Shopping Cart

The shopping cart uses browser localStorage to persist cart items. Features include:
- Add to cart from product pages
- View cart with all items
- Update quantities
- Remove items
- Calculate subtotals
- Cart count badge in header

### Product Management

Products are defined in `src/data/products.ts`. To add new products, simply add them to the products array.

### Styling

The site uses Tailwind CSS with custom configuration. Colors, fonts, and other design tokens can be customized in `tailwind.config.mjs`.

## Customization

### Adding Products

Edit `src/data/products.ts` to add or modify products:

```typescript
{
  id: 'unique-id',
  name: 'Product Name',
  description: 'Product description',
  price: 24.99,
  image: 'image-url',
  category: 'Category Name',
  featured: true, // Show on homepage
}
```

### Changing Colors

Edit `tailwind.config.mjs` to customize the color scheme.

### Modifying Layout

Edit `src/layouts/Layout.astro` to change the base layout structure.

## Deployment

This site can be deployed to any static hosting service:

- **Vercel**: Connect your GitHub repo and deploy automatically
- **Netlify**: Drag and drop the `dist/` folder or connect via Git
- **Cloudflare Pages**: Connect your repository
- **GitHub Pages**: Use GitHub Actions to build and deploy

## Future Enhancements

- Payment integration (Stripe, PayPal)
- User authentication
- Product reviews and ratings
- Wishlist functionality
- Newsletter subscription
- Blog section
- Admin dashboard for product management

## License

This project is open source and available for use.
