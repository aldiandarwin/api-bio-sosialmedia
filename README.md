
# Backend Setup

The backend of SocialLink Hub is powered by Strapi, a flexible and open-source headless CMS. This section will guide you through the setup and configuration of the Strapi backend.

## Strapi Installation and Configuration

Install Strapi

In the root directory of your backend project, run the following command to install Strapi:

```bash
Copy code
npm install strapi@beta
```

## clone a Strapi Project

Run the following command to create a new Strapi project:

```bash
Copy code
git clone https://github.com/aldiandarwin/api-bio-sosialmedia.git
```

## Configure Strapi

Navigate to the my-project directory:

cd my-project

Start Strapi and install dependencies

``` bash
Copy code
npm install
```

# Database

Here's an example of how you can create
an .env.example

file with placeholders for the environment variables you need provided:

``` bash
HOST=0.0.0.0
PORT=1337
APP_KEYS="toBeModified1,toBeModified2"
API_TOKEN_SALT=tobemodified
ADMIN_JWT_SECRET=tobemodified
TRANSFER_TOKEN_SALT=tobemodified
JWT_SECRET=tobemodified
```

During the setup process, you will be prompted to choose your database settings.

Choose the appropriate database type (e.g., SQLite, PostgreSQL, MongoDB) based on your project requirements.

## Run Strapi

After the setup is complete, you can run Strapi with the following command:

```bash
Copy code
npm start
```

Your Strapi backend will be accessible at <http://localhost:1337/admin>.

Log in with the credentials you provided during the setup.

Strapi Configuration in SocialLink Hub Frontend
Configure Strapi API Endpoint

dont forget In your frontend project (SocialLink Hub)

update the .env.local file or your configuration file with the Strapi API endpoint:

```Copy code
NEXT_PUBLIC_API_URL=http://localhost:1337
```

Replace the URL with the correct address where your Strapi backend is running.

## Start the Frontend

Run the following command in your frontend project directory to start the Next.js frontend:

```bash
Copy code
npm run dev
```

Your SocialLink Hub with the integrated Strapi backend should now be accessible at <http://localhost:3000>.
