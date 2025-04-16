# Material Tailwind Dashboard React

A modern, responsive admin dashboard built with React, Material Tailwind, and Vite.

![Material Tailwind Dashboard](./public/img/logo-ct-dark.png)

## Features

- 🎨 Beautiful UI components based on Material Tailwind
- 📊 Interactive charts and statistics using ApexCharts
- 📱 Fully responsive layout
- 🔐 Authentication pages (Sign In, Sign Up)
- 📄 Multiple dashboard pages (Home, Profile, Tables, Notifications)
- ⚙️ User interface configuration options
- 🚀 Fast build times with Vite

## Live Demo

Visit [material-tailwind.com](https://material-tailwind.com) to see a live demo.

## Quick Start

Follow these steps to get started with the Material Tailwind Dashboard:

1. **Prerequisites**
   - Node.js LTS version from [Node.js Official Page](https://nodejs.org/en/download/)

2. **Installation**
   ```bash
   # Clone the repository (if not done already)
   git clone https://github.com/yourusername/paper-plane.git
   cd paper-plane

   # Install dependencies
   npm install
   # or
   yarn install
   # or
   pnpm install
   ```

3. **Development**
   ```bash
   # Start the development server
   npm run dev
   ```

4. **Building for Production**
   ```bash
   # Create a production build
   npm run build
   
   # Preview the production build locally
   npm run preview
   ```

5. **Deployment with Genezio**
   ```bash
   # Deploy to Genezio
   npx genezio deploy
   ```

## Project Structure

```
paper-plane/
├── public/               # Static assets
│   ├── css/              # CSS files
│   └── img/              # Images
├── src/
│   ├── configs/          # Configuration files
│   ├── context/          # React context for state management
│   ├── data/             # Sample data for tables, charts, etc.
│   ├── layouts/          # Layout components (Dashboard, Auth)
│   ├── pages/            # Page components
│   │   ├── auth/         # Authentication pages
│   │   └── dashboard/    # Dashboard pages
│   ├── widgets/          # Reusable UI components
│   │   ├── cards/        # Card components
│   │   ├── charts/       # Chart components
│   │   └── layout/       # Layout components (Navbar, Sidebar, etc.)
│   ├── App.jsx           # Main App component
│   ├── main.jsx          # Entry point
│   └── routes.jsx        # Route definitions
├── index.html            # HTML template
├── package.json          # Project dependencies and scripts
├── vite.config.js        # Vite configuration
├── tailwind.config.cjs   # Tailwind CSS configuration
└── genezio.yaml          # Genezio deployment configuration
```

## Browser Support

The dashboard supports the latest versions of:

- Chrome
- Firefox
- Safari
- Edge

## Technologies Used

- [React 18](https://reactjs.org/)
- [Material Tailwind 2.1.4](https://material-tailwind.com/)
- [Tailwind CSS 3.3.4](https://tailwindcss.com/)
- [Vite 4.5.0](https://vitejs.dev/)
- [React Router 6.17.0](https://reactrouter.com/)
- [ApexCharts 3.44.0](https://apexcharts.com/)
- [Heroicons 2.0.18](https://heroicons.com/)
- [Genezio](https://genez.io/) for deployment

## Contributing

If you'd like to contribute to this project, please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.

## Changelog

See the [CHANGELOG.md](./CHANGELOG.md) file for details on updates and version history.

## Documentation

For more detailed documentation, visit [material-tailwind.com](https://material-tailwind.com/?ref=readme-mtdr).