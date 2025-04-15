# Welcome to your Lovable project

## Project info

**URL**: https://lovable.dev/projects/d3e0a8e2-360d-4caa-b308-eac23b2fe86f

## How can I edit this code?

There are several ways of editing your application.

**Use Lovable**

Simply visit the [Lovable Project](https://lovable.dev/projects/d3e0a8e2-360d-4caa-b308-eac23b2fe86f) and start prompting.

Changes made via Lovable will be committed automatically to this repo.

**Use your preferred IDE**

If you want to work locally using your own IDE, you can clone this repo and push changes. Pushed changes will also be reflected in Lovable.

The only requirement is having Node.js & npm installed - [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating)

Follow these steps:

```sh
# Step 1: Clone the repository using the project's Git URL.
git clone <YOUR_GIT_URL>

# Step 2: Navigate to the project directory.
cd <YOUR_PROJECT_NAME>

# Step 3: Install the necessary dependencies.
npm i

# Step 4: Start the development server with auto-reloading and an instant preview.
npm run dev
```

**Edit a file directly in GitHub**

- Navigate to the desired file(s).
- Click the "Edit" button (pencil icon) at the top right of the file view.
- Make your changes and commit the changes.

**Use GitHub Codespaces**

- Navigate to the main page of your repository.
- Click on the "Code" button (green button) near the top right.
- Select the "Codespaces" tab.
- Click on "New codespace" to launch a new Codespace environment.
- Edit files directly within the Codespace and commit and push your changes once you're done.

## What technologies are used for this project?

This project is built with:

- Vite
- TypeScript
- React
- shadcn-ui
- Tailwind CSS

## How can I deploy this project?

Simply open [Lovable](https://lovable.dev/projects/d3e0a8e2-360d-4caa-b308-eac23b2fe86f) and click on Share -> Publish.

## Can I connect a custom domain to my Lovable project?

Yes it is!

To connect a domain, navigate to Project > Settings > Domains and click Connect Domain.

Read more here: [Setting up a custom domain](https://docs.lovable.dev/tips-tricks/custom-domain#step-by-step-guide)

## Running the App with Database Backend

To run the app with the SQLite database backend, follow these steps:

1. Install backend dependencies (one-time setup):
   ```bash
   npm run server:install
   ```

2. Install frontend dependencies (if not already installed):
   ```bash
   npm install
   ```

3. Start the backend server:
   ```bash
   npm run server
   ```
   or for development with auto-restart:
   ```bash
   npm run server:dev
   ```

4. In a separate terminal, start the frontend development server:
   ```bash
   npm run dev
   ```

5. Access the app:
   - Frontend: http://localhost:5173
   - Backend API: http://localhost:5000/api

The database will be initialized automatically when the server starts for the first time, creating all necessary tables and default data.

### Database Structure

The SQLite database includes the following tables:
- `students`: Stores registered student information
- `courses`: Stores available courses
- `enrollments`: Tracks student enrollments in courses
- `administrators`: Stores admin user accounts

### API Endpoints

#### Student Endpoints
- `GET /api/students`: Get all students
- `POST /api/students/register`: Register a new student
- `GET /api/students/:id`: Get student by ID
- `PATCH /api/students/:id/status`: Update student status
- `GET /api/students/stats/overview`: Get student statistics

#### Course Endpoints
- `GET /api/courses`: Get all courses
- `GET /api/courses/:id`: Get course by ID
- `GET /api/courses/:id/enrollments`: Get enrollments for a course
- `GET /api/courses/:id/stats`: Get course statistics

#### Admin Endpoints
- `POST /api/admin/login`: Admin login
- `GET /api/admin/profile`: Get admin profile
- `POST /api/admin/change-password`: Change admin password
- `POST /api/admin/create`: Create a new admin
- `GET /api/admin/dashboard`: Get dashboard statistics
