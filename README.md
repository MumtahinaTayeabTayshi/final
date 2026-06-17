# BookNest MERN Reading Tracker

BookNest is a full MERN stack application for students and readers who want to manage a personal digital library. Users can add books, track reading status, filter by category, give ratings, and write short notes.

## Project Topic

**BookNest: A MERN Reading Tracker and Library Management Website**

This project was selected as a different topic from the previous project. It is suitable for a React.js final project because it demonstrates component structure, hooks, routing, API integration, backend logic, MongoDB modeling, and responsive frontend design.

## Required Features Covered

- Responsive frontend built with React
- Backend API built with Node.js and Express
- MongoDB database integration using Mongoose
- CRUD operations for books
- React Router pages
- Custom React hook for book data management
- API service layer using Axios
- Public GitHub-ready repository structure
- Netlify-ready frontend configuration
- README documentation
- Files matching the sample repository structure:
  - `guidelines/`
  - `src/`
  - `.gitignore`
  - `ATTRIBUTIONS.md`
  - `LICENSE`
  - `README.md`
  - `index.html`
  - `package-lock.json`
  - `package.json`
  - `postcss.config.mjs`
  - `vite.config.ts`

## Main Pages

- Home page with hero section and project overview
- Library page with searchable and filterable book cards
- Add Book page with form validation
- About page with MERN project explanation

## Backend API Endpoints

Base URL for local development:

```txt
http://localhost:5000/api/books
```

| Method | Endpoint | Description |
|---|---|---|
| GET | `/api/books` | Get all books |
| GET | `/api/books/:id` | Get one book |
| POST | `/api/books` | Create a new book |
| PUT | `/api/books/:id` | Update a book |
| DELETE | `/api/books/:id` | Delete a book |

## Installation

Install dependencies from the root folder:

```bash
npm install
```

Create a backend environment file:

```bash
cp backend/.env.example backend/.env
```

Add your MongoDB connection string in `backend/.env`:

```env
MONGO_URI=mongodb://127.0.0.1:27017/booknest
PORT=5000
CLIENT_URL=http://localhost:5173
```

## Run the Full MERN App

Start frontend and backend together:

```bash
npm run dev
```

Or run separately:

```bash
npm run client
npm run dev:server
```

Frontend will run on:

```txt
http://localhost:5173
```

Backend will run on:

```txt
http://localhost:5000
```

## Seed Sample Data

After setting up MongoDB, run:

```bash
npm run seed
```

## Netlify Deployment Note

This project includes `netlify.toml` for frontend deployment. For a real hosted MERN app, deploy the backend separately on Render, Railway, Cyclic, or another Node hosting platform and set the frontend environment variable:

```env
VITE_API_BASE_URL=https://your-backend-url.com/api
```

## Folder Structure

```txt
booknest-mern/
├── guidelines/
├── src/
│   ├── components/
│   ├── hooks/
│   ├── pages/
│   ├── services/
│   ├── types/
│   ├── App.tsx
│   ├── main.tsx
│   └── styles.css
├── backend/
│   ├── config/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── seeds/
│   └── server.js
├── .gitignore
├── ATTRIBUTIONS.md
├── LICENSE
├── README.md
├── index.html
├── package-lock.json
├── package.json
├── postcss.config.mjs
└── vite.config.ts
```

## Final Submission Checklist

- Source code folder is complete
- React components are organized
- Hooks are used for data management
- Backend API is included
- MongoDB model is included
- README is included
- Netlify build configuration is included
- GitHub repository can be created from this folder
- Live deployment can be created after adding hosting accounts
