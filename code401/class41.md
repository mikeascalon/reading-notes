# Reading Notes

## React 4

Explain the concept of dynamic routes in Next.js and how they differ from static routes.

Dynamic routes in Next.js provide a powerful way to build pages that adapt to different data, making them essential for applications that require content to be dynamic and personalized. Static routes, while simpler, are used for pages with fixed content.

Describe the process of deploying a Next.js application. What are the key steps involved, and what are some deployment platforms you can use?

**1. Prepare Your Application**

Optimization: Ensure your Next.js application is optimized for production. This includes using Next.js features like Image Optimization, Automatic Static Optimization, Incremental Static Regeneration, and more to ensure your application loads quickly and efficiently.

Environment Variables: Set up any necessary environment variables for different environments (development, staging, production). Next.js allows you to define environment variables in .env files (e.g., .env.local, .env.production).

**2. Build Your Application**
 
Run the Build Command: Execute next build to create an optimized production build of your application. This step compiles your application, performs optimizations, and generates static HTML pages (where applicable).

Static Export (Optional): If your application is fully static, you can use `next export` to generate static HTML files for your pages. This is optional and depends on the nature of your application.

**3. Choose a Deployment Platform**
Next.js applications can be deployed to various platforms, each with its own set of instructions. Some popular platforms include:

**Vercel:** As the creators of Next.js, Vercel offers a seamless deployment experience for Next.js applications, with features like automatic SSL, global CDN, and edge functions. Deploying to Vercel typically involves pushing your code to a Git repository and connecting your repository to Vercel.

**Netlify:** Netlify supports Next.js deployments with features like continuous deployment from Git across all of Netlify’s CDN, serverless functions for backend logic, and more. Deploying to Netlify usually involves connecting your Git repository to Netlify and configuring build settings.

**AWS (Amazon Web Services): **Deploying on AWS can be done in several ways, including using services like AWS Amplify for simpler deployments or more complex setups involving S3 for static files and CloudFront as a CDN.

**Heroku:** Heroku can host Next.js applications with support for both static sites and applications with server-side components. Deployment typically involves pushing your code to a Heroku Git repository.

**Other Cloud Providers:** Other providers like Google Cloud Platform (GCP) and Microsoft Azure also support hosting Next.js applications, with various services for hosting, storage, and functions.

How does Next.js handle static file serving? Discuss the default folder structure for storing static assets and explain how to reference them in a Next.js application.

Next.js provides a straightforward and efficient way to handle static file serving through its public directory. This functionality is designed to serve static assets like images, stylesheets, and other files that don't need to be processed by Webpack. 

**Public Directory**

*Location and Naming:* The `public` directory should be located at the root of your Next.js project. The name of this directory is fixed to `public` and cannot be changed. This is where you place your static files that you want to serve directly, without any processing by Next.js or Webpack.

*Accessing Static Files:* Files placed inside the `public` directory can be accessed using a URL that starts from the base path (`/`). For example, if you place an image called `me.png` inside `public/avatars/`, it can be accessed via the URL `/avatars/me.png.`

### Resources

[Dynamic Routes](https://nextjs.org/learn-pages-router/basics/dynamic-routes/dynamic-routes-details)

[Deploying Your Next.js App](https://nextjs.org/learn-pages-router/basics/deploying-nextjs-app/deploy)

