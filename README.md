# Disaster Management App - GDSC '24
 

## Stack

- Next.js 13: Build powerful and scalable server-side rendered React applications.
- Firebase: Leverage the Firebase platform for authentication, real-time database, and cloud functions.
- Tailwind CSS: Rapidly build custom user interfaces using the utility-first CSS framework.
- Automatic Code Splitting: Optimize performance by splitting your JavaScript code into smaller, cacheable chunks.
- Dynamic Routing: Create dynamic routes for handling different pages and content.
- Hot Module Replacement: Enjoy a fast development experience with hot module replacement for instant code changes.
- Environment Variables: Safely manage environment-specific configuration values using environment variables.
- ESLint and Prettier: Maintain code quality and consistency with the help of ESLint and Prettier.

## Setup

Before getting started, ensure you have the following prerequisites:

- Node.js 14 or higher
- npm or yarn package manager

## Getting Started

- To start a new project using this template click `Use this template` button.
- Navigate into the project directory: `cd nextjs-13-firebase-starter`
- Install the dependencies:

```bash
  npm install
  # or
  yarn install
```

- Run the development server:

```bash
  npm run dev
  # or
  yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Set Up Firebase

<https://console.firebase.google.com/>

- Log in with your Google account.
- Click on `Go to console` button.
- Click `Add Project` card.
- Give your project a name.
- Click on `Continue` button.
- Disable `Google Analytics for this project` (unless you wish to use it).
- Click `Create project` button.
- Click on the web icon button to create your web app. It will show a text popup `Web`.
- Register app by giving it a nickname and click `Register app` button.
- Where package.json is located, in your cli, type `npm i firebase`.
- Copy configuration file. Make a new file in `src` called `firebase` called `firebase.js`.
- In project root, create a file and name it `.env`.
- Make sure you add `.env.local` to your `.gitignore` so you don't expose your variables in git repo.
- Follow the instructions here at <https://nextjs.org/docs/pages/building-your-application/configuring/environment-variables#loading-environment-variables> to add your variables from firebase.js into this file.

Example...

```md
NEXT_PUBLIC_FIREBASE_API_KEY=your_api_key
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=your_auth_domain
NEXT_PUBLIC_FIREBASE_PROJECT_ID=your_project_id
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=your_storage_bucket
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=your_messaging_sender_id
NEXT_PUBLIC_FIREBASE_APP_ID=your_app_id
```

- Create `env` file and paste these variables with your own information.
- Click on `Continue on console` button
- On your project homepage, choose a product to add to your app. First, click on `Authentication`.
- Under `Get started with Firebase Auth by adding your first sign-in method` select `Email/Password`.

You should now be setup to use Firebase.

## Authentication

- In `src/firebase` directory, exists the directory `auth` containing the logic for `signin` and `signup`.

## Folder Structure

The folder structure of this project is organized as follows:

- `pages`: Contains the Next.js pages for server-side rendering.
- `components`: Holds the reusable React components.
- `lib`: Includes utility functions and modules.
- `public`: Stores static assets such as images, fonts, and stylesheets.
- `styles`: Contains global styles and Tailwind CSS configuration.
- `firebase`: Houses the Firebase configuration and Firebase-related functions.

Feel free to modify and expand the folder structure according to your project requirements.

## Deployment

To deploy your Next.js application with Firebase, follow the Firebase deployment instructions specific to your hosting option (Firebase Hosting, Cloud Functions, etc.). Make sure to set up the appropriate environment variables for your production environment.

## Members