# Streamer

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A modern Netflix-inspired streaming platform built with Next.js, React and Prisma. Streamer allows users to authenticate, manage personal watch lists and enjoy smooth video playback on any device.

## Table of Contents

- [Features](#features)
- [Demo](#demo)
- [Setup](#setup)
  - [Simple Mode Setup](#simple-mode-setup)
  - [Advanced Mode Setup](#advanced-mode-setup)
- [Usage](#usage)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [FAQ](#faq)
- [License](#license)
- [Acknowledgements](#acknowledgements)
- [Contact](#contact)

## Features

- Secure authentication with Google, GitHub and email/password
- Responsive UI with Tailwind CSS
- MongoDB database powered by Prisma ORM
- Personalized favorite lists and profile selection
- Video playback in a dedicated watch page
- Data fetching via SWR hooks
- State management through Zustand
- REST API routes for movies and favorites

## Demo

[YouTube Tutorial](https://www.youtube.com/watch?v=mqUN4N2q4qY)

## Setup

The project uses environment variables for database and OAuth configuration.

### Simple Mode Setup

1. **Clone the Repository**
   ```bash
   git clone [repo-url]
   cd [project-name]
   ```

2. **Install Dependencies**
   ```bash
   npm install
   ```

3. **Configure Environment**
   ```bash
   cp .env.example .env.local
   ```
   Required variables:
   * `DATABASE_URL=`
   * `GOOGLE_CLIENT_ID=`
   * `GOOGLE_CLIENT_SECRET=`
   * `GITHUB_ID=`
   * `GITHUB_SECRET=`
   * `NEXTAUTH_JWT_SECRET=`
   * `NEXTAUTH_SECRET=`

4. **Run the App**
   ```bash
   npm run dev
   ```

### Advanced Mode Setup

Configure additional services such as a production MongoDB instance or custom domain with SSL. You can also adjust NextAuth providers or add plugins like analytics in this mode.

## Usage

1. Register or sign in using Google, GitHub or email.
2. Create/select a profile to start browsing.
3. Click a movie thumbnail to open the info modal or play instantly.
4. Add movies to your favorites for quick access.
5. Use the watch page for fullscreen playback and controls.

## Deployment

The app works seamlessly on [Vercel](https://vercel.com/). After setting the environment variables in your Vercel dashboard, simply push your repository and click the button below:

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/import)

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests to improve the project.

## FAQ

1. **Do I need a MongoDB database?**  
   Yes. Set `DATABASE_URL` to your MongoDB connection string.
2. **Can I use other OAuth providers?**  
   You can extend the NextAuth configuration to include any provider supported by NextAuth.
3. **Is this project production ready?**  
   The code is a solid starting point but you should audit security and performance before deploying to production.

## License

This project is licensed under the MIT license.

## Acknowledgements

- [Next.js](https://nextjs.org/)
- [React](https://reactjs.org/)
- [Tailwind CSS](https://tailwindcss.com/)
- [Prisma](https://www.prisma.io/)
- [NextAuth.js](https://next-auth.js.org/)
- [Zustand](https://github.com/pmndrs/zustand)
- [SWR](https://swr.vercel.app/)

## Contact

For support or questions, please open an issue on the [GitHub repository](https://github.com/your-org/your-repo).

