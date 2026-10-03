# ✦ Orbit — Personalized Content Dashboard

Orbit is a responsive, personalized content dashboard that brings news, entertainment, finance, culture, and community content together in one place. Users can discover stories, search topics, save favorites, customize interests, and switch between light and dark modes.

## ✨ Features

* **Personalized Feed** — Explore content across multiple categories.
* **Search** — Find stories by title, description, topic, or source with debounced search.
* **Category Filters** — Filter content by Technology, Culture, Finance, Entertainment, and Social.
* **Favorites** — Save interesting stories for later.
* **Custom Preferences** — Choose which topics appear in your feed.
* **Dark Mode** — Switch between light and dark appearances.
* **Trending Content** — Explore popular topics and stories.
* **Responsive Design** — Works across desktop, tablet, and mobile screens.
* **Drag-and-Drop Ordering** — Reorder content cards where supported.
* **API Integration** — Designed to support news and movie recommendation APIs.
* **Persistent Local Preferences** — Retain saved items and preferences using browser storage.

## 🛠️ Tech Stack

* Next.js
* React
* TypeScript
* Redux Toolkit
* RTK Query
* CSS / Tailwind CSS integration
* Vitest
* React Testing Library
* Playwright

> Note: Verify the dependencies and implementation in the current source before claiming every technology or feature is fully implemented.

## 🚀 Getting Started

### Prerequisites

* Node.js (LTS recommended)
* npm

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/YOUR_USERNAME/personalized-content-dashboard.git
   ```

2. Navigate into the project:

   ```bash
   cd personalized-content-dashboard
   ```

3. Install dependencies:

   ```bash
   npm install
   ```

4. Create a local environment file:

   ```bash
   cp .env.example .env.local
   ```

5. Start the development server:

   ```bash
   npm run dev
   ```

6. Open http://localhost:3000 in your browser.

## 🔑 Environment Variables

Add the API keys supported by your project to `.env.local`, for example:

```env
NEWS_API_KEY=your_news_api_key
TMDB_API_KEY=your_tmdb_api_key
```

Keep secret keys on the server. Never expose private API keys in client-side code or commit `.env.local` to GitHub.

The dashboard should use sample content when live API credentials are unavailable, where that fallback is implemented.

## 🧪 Testing

Run the available checks:

```bash
npm run typecheck
npm test
npm run build
```

For end-to-end tests, install the Playwright browser if the project includes the configured test suite:

```bash
npx playwright install chromium
npm run test:e2e
```

Confirm that these scripts exist in `package.json` and pass before submitting the project.

## 📁 Project Structure

```text
personalized-content-dashboard/
├── app/                  # Next.js pages and API routes
├── components/           # Reusable UI components
├── features/              # Redux Toolkit features and state
├── lib/                   # Utilities and API helpers
├── public/                # Static assets
├── tests/                 # Automated tests
├── .env.example           # Environment variable template
├── README.md              # Project documentation
└── package.json           # Dependencies and scripts
```

The exact structure may differ depending on the current project files.

## 🔒 Security

* Keep API keys in server-side environment variables.
* Validate API inputs and handle failed requests gracefully.
* Avoid committing secrets, credentials, or private configuration.
* Use environment variables for deployment configuration.

## 🌐 Deployment

The application can be deployed to a platform that supports Next.js, such as Vercel.

1. Push the project to GitHub.
2. Import the repository into your deployment platform.
3. Configure the required environment variables.
4. Deploy the application.
5. Verify the deployed site and API routes.

## 🔮 Future Improvements

* User authentication and account-based preferences
* Real-time content updates
* Infinite scrolling
* More recommendation sources
* Accessibility improvements
* Internationalization
* Expanded unit and end-to-end test coverage
