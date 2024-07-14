# DevOverflow - Full Stack Next.js 14 Application

### Welcome to DevOverflow

DevOverflow is a full-stack application built with Next.js 14 and Server Actions, offering a range of powerful features to enhance your experience in the developer community. It is designed to be a comprehensive platform where developers can ask questions, share knowledge, and engage in a vibrant community.
<br>
![devoverflow-light](https://github.com/user-attachments/assets/8964c5e2-4719-4591-ad02-6e76ffba7acc)




## 🚀 Features

- **Next.js Server Actions**: Enhanced backend functionality with Next.js server actions.
- **Authentication Webhooks**: Streamlined authentication services using webhooks.
- **Question and Answer Platform**: Engage in discussions by posting questions and answers.
- **Bookmarking**: Save and organize favorite posts for easy access later.
- **Post Recommendation System**: Advanced system to recommend relevant content.
- **Global Data Fetching**: Efficient data fetching from all database models for the search feature.
- **AI-Generated Answers**: Utilize AI to generate insightful answers to questions.
- **Community Badges & Reputation System**: Earn badges and build reputation within the community.
- **Views and Voting**: Track views and enable voting on content.
- **Filter and Pagination**: Enjoy features like filtering and pagination for easy navigation.
- **Responsive UI**: A responsive user interface that adapts to different screen sizes.
- **User Authentication**: Create a personalized account for full engagement.
- **Theme Switching**: Switch between light and dark themes for comfort.
- **Multiple Layouts & Grouped Routes**: Organized interface with various layout options.
- **Form Handling**: Efficient form handling for smooth user interactions.
- **Tag Browsing**: Browse content categorically using an intuitive tag system.

## 🛠️ Tech Stack

- **Next.js 14**: React framework for building server-rendered applications.
- **Tailwind CSS**: Utility-first CSS framework for responsive design.
- **TypeScript**: Typed superset of JavaScript.
- **ESLint**: Linting utility for JavaScript and TypeScript.
- **MongoDB**: Database management system.
- **Mongoose**: MongoDB object modeling for Node.js.
- **Clerk**: Authentication workflow simplification.
- **React Hook Form**: Form management for React.
- **Zod**: TypeScript-first schema declaration.

## 🚀 Developer

- LinkedIn: Tipu Sultan - [Tipu Sultan](https://www.linkedin.com/in/tipu-sultan2315/)
- GitHub: [@TipuSultan](https://github.com/Tipu30)

## 🛠️ Running the Project

1. Clone the repository.
2. Install dependencies using:

    ```bash
    npm install
    # or
    yarn install
    ```

3. Run the development server:

    ```bash
    npm run dev
    # or
    yarn dev
    # or
    pnpm dev
    # or
    bun dev
    ```

4. Open [http://localhost:3000](http://localhost:3000) in your browser to see the result.
5. Create a `.env.local` file in the project's root directory and add the following environment variables:

    ```bash
    # Clerk secrets for API key and webhook
    NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
    CLERK_SECRET_KEY=
    NEXT_CLERK_WEBHOOK_SECRET=

    # Clerk routes
    NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
    NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
    NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
    NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

    # TinyMCE editor
    NEXT_PUBLIC_TINY_EDITOR_API_KEY=

    # Database
    MONGO_DB_URI=

    # OpenAI API
    OPENAI_API_KEY=
    ```

**Notes**

- **Clerk Authentication**: Create a Clerk account [here](https://clerk.com/) and set the `NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY` and `CLERK_SECRET_KEY` environment variables in the `.env.local` file. Configure different URLs for Clerk sign-in, sign-up, after sign-in, and after sign-up pages.
- **MongoDB Database**: Create a MongoDB database and connect it to the application. Change the `MONGO_DB_URI` environment variable in the `.env.local` file.
- **TinyMCE**: Create a TinyMCE account [here](https://www.tiny.cloud/) and set the `NEXT_PUBLIC_TINY_EDITOR_API_KEY` environment variable in the `.env.local` file.
- **OpenAI API**: Create an OpenAI account [here](https://www.openai.com/) and set the `OPENAI_API_KEY` environment variable in the `.env.local` file.
- After deployment, create a new webhook on Clerk, add the endpoint of `http://<Your-deployed-link>/api/webhook`, set `user` events, and set the `NEXT_CLERK_WEBHOOK_SECRET` environment variable in the `.env.local` file.


