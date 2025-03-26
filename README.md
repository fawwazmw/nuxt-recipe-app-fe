# Nuxtcipes

Nuxtcipes is a recipe application built with Nuxt 3 that uses the dummyJSON API to display various recipes. Users can browse popular recipes, view recipe details, and follow cooking instructions.

![Nuxtcipes](./public/nuxt-course-hero.png)

## Features

- Browse popular recipes with preview cards
- View detailed recipe information including:
    - Ingredients with interactive checklist
    - Step-by-step cooking instructions
    - Cooking time, calorie information, and ratings
- Responsive design for all device sizes
- SEO optimization with meta tags
- Custom error handling

## Tech Stack

- **Nuxt 3**: Vue-based framework for building modern web applications
- **Vue 3**: Progressive JavaScript framework
- **TypeScript**: For type safety
- **Tailwind CSS**: For styling
- **Nuxt Image**: For optimized image handling
- **Nuxt Icon**: For icon integration

## Project Structure

```
nuxtcipes/
├── app/
│   ├── components/
│   │   ├── BaseBtn.vue           # Reusable button component
│   │   ├── BaseNavigation.vue    # Site navigation header
│   │   └── RecipeCard.vue        # Recipe preview card
│   ├── layouts/
│   │   └── default.vue           # Default layout with navigation
│   ├── pages/
│   │   ├── recipes/
│   │   │   └── [id].vue          # Dynamic recipe detail page
│   │   ├── about.vue             # About page
│   │   └── index.vue             # Home page
│   ├── app.vue                   # Application entry point
│   └── error.vue                 # Custom error page
├── public/                       # Static assets
│   ├── icon-green.png
│   ├── nuxt-course-hero.png
│   └── robots.txt
├── server/                       # Server-side code
├── types/                        # TypeScript interfaces
│   └── types.ts                  # Recipe data type definitions
├── nuxt.config.ts                # Nuxt configuration
├── package.json                  # Project dependencies
├── tailwind.config.js            # Tailwind CSS configuration
└── tsconfig.json                 # TypeScript configuration
```

## Getting Started

### Prerequisites

- Node.js (v18 or later recommended)
- npm or yarn

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/fawwazmw/nuxt-recipe-app-fe.git
   cd nuxt-recipe-app-fe
   ```

2. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```

3. Run development server:
   ```bash
   npm run dev
   # or
   yarn dev
   ```

4. Open your browser and navigate to `http://localhost:3000`

## Building for Production

```bash
# Generate static site
npm run generate
# or
yarn generate

# Build for production
npm run build
# or
yarn build

# Preview production build
npm run preview
# or
yarn preview
```

## Project Configuration

### Tailwind CSS

Custom colors defined in `tailwind.config.js`:
- `dodgeroll-gold`: #F79F1A
- `apple-green`: #046E1B
- `dire-wolf`: #292727

### Google Fonts

The project uses the Montserrat font family which is loaded via the Google Fonts module.

### Image Optimization

Images are optimized using the Nuxt Image module with support for various formats including WebP.

## API Integration

This project uses the [dummyJSON Recipes API](https://dummyjson.com/recipes) to fetch recipe data.

## Features in Detail

### Recipe Cards

Recipe cards display:
- Recipe image
- Recipe name
- Cooking time
- Calories per serving
- Rating and review count

### Recipe Details Page

The recipe details page includes:
- Recipe name and image
- Cooking metrics (time, calories, rating)
- Interactive ingredients checklist
- Numbered step-by-step instructions

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the [MIT License](https://opensource.org/license/MIT) - see the LICENSE file for details.

## Acknowledgments

- [DummyJSON](https://dummyjson.com/) for providing the recipe API
- [Nuxt](https://nuxt.com/) for the framework
- [Tailwind CSS](https://tailwindcss.com/) for the styling utilities