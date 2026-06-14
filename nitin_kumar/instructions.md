# ArcadeHub Nexus - Full-Stack Online Gaming Website

## 1. Context

Build a full-stack web application for ArcadeHub Nexus, a fictional online casual gaming website created for NovaPlay Labs.

The site lets users create an account, log in, browse casual games, save favorite games, submit demo scores, and view leaderboard rankings.

This task is not a frontend-only landing page. It must include a working frontend, backend API, local database, authentication, seeded sample data, and README setup instructions.

This project must not include betting, gambling, casino mechanics, payment gateways, crypto wallets, real-money rewards, or copyrighted game assets.

## 2. Reference Materials

Use these files from the task folder:

- `reference_image.png`: visual direction for the homepage layout, dark arcade style, header spacing, card layout, leaderboard preview, and dashboard panels.
- `assets.pdf`: brand colors, typography guidance, content rules, UI components, backend scope, and asset boundaries.

The reference image is layout guidance only. Do not copy it pixel-for-pixel.

## 3. Required Stack

Use this stack unless a documented equivalent is provided:

### Frontend
- React 18 or newer
- Vite
- TypeScript
- CSS modules, Tailwind, or plain CSS

### Backend
- Node.js
- Express.js
- JWT authentication
- bcrypt password hashing

### Database
- SQLite preferred
- MongoDB allowed only with local setup documentation

Cloud-only databases are not allowed.

## 4. Required Folder Structure

Submit a project with this structure or a clearly documented equivalent:

```text
arcadehub-nexus/
├── frontend/
├── backend/
├── README.md
└── screenshots/
```

## 5. Required Frontend Screens

### Homepage
Include:
- ArcadeHub Nexus branding
- Product headline
- Browse Games button
- Sign In button
- Featured Games section
- Leaderboard preview
- Daily Challenge preview

### Sign Up
Include:
- Username field
- Email field
- Password field
- Submit button
- Error message area

### Login
Include:
- Email field
- Password field
- Submit button
- Error message area

### Games Catalog
Include:
- Game cards loaded from backend API
- At least 12 seeded games
- Search input
- Category filter
- Rating sort
- Empty state for zero matches

### Game Detail
Include:
- Game title
- Description
- Category
- Rating
- Difficulty
- Estimated play time
- Tags
- Instructions
- Play Now button
- Demo preview area
- Favorite button
- Score submission form

### Leaderboard
Include:
- Ranked player list loaded from backend API
- At least 10 leaderboard records
- Rank
- Username
- Game title
- Score
- Badge

### Profile
Include:
- Authenticated username
- Saved favorite games
- Submitted scores
- Logout button

## 6. Required Backend API

Create these API routes:

- `POST /api/auth/signup`
- `POST /api/auth/login`
- `GET /api/auth/me`
- `GET /api/games`
- `GET /api/games/:id`
- `GET /api/favorites`
- `POST /api/favorites`
- `DELETE /api/favorites/:gameId`
- `POST /api/scores`
- `GET /api/leaderboard`
- `GET /api/health`

## 7. Database Requirements

Create these database tables:

- users
- games
- favorites
- scores

Seed the database with:
- At least 12 games
- At least 10 leaderboard scores
- At least 1 demo user

Game records must include:
- id
- title
- category
- description
- rating
- difficulty
- estimated_play_time
- tags
- instructions
- thumbnail_token

## 8. Authentication Requirements

Implement:
- Signup
- Login
- Password hashing
- JWT creation
- Protected profile endpoint
- Frontend logout

Do not store plain-text passwords.

## 9. Full-Stack Behavior

The frontend must fetch catalog data from the backend.

The frontend must fetch leaderboard data from the backend.

The frontend must save favorites using the backend.

The frontend must submit scores using the backend.

The profile page must require a valid token.

## 10. Visual Requirements

Use the visual direction from `reference_image.png`.

Required visual style:
- Dark navy background
- Neon cyan primary accent
- Electric violet secondary accent
- Gold leaderboard highlight
- Card-based layout
- Rounded panels
- Single sans-serif font family
- Consistent header colors
- Visible button hover states
- Visible focus states

## 11. Responsiveness Requirements

The website must work at:
- 1440px width
- 1024px width
- 768px width
- 375px width

At 375px width:
- No horizontal page overflow
- Navigation remains usable
- Cards stack vertically
- Buttons remain visible

## 12. README Requirements

README.md must include:
- Project title
- Tech stack
- Folder structure
- Frontend setup command
- Backend setup command
- Database setup command
- Seed command
- Frontend run command
- Backend run command
- Demo login credentials
- API route list
- Out-of-scope note

## 13. Screenshots

Submit:
- One desktop screenshot
- One mobile screenshot

Screenshots should be placed in the `screenshots/` folder.

## 14. Out of Scope

Do not include:
- Betting
- Gambling
- Casino mechanics
- Payment gateways
- Crypto wallets
- Live multiplayer
- Cloud-only database
- Admin dashboard
- App store deployment
- Copyrighted game art
- Real gaming company logos
- Celebrity images

## 15. Acceptance Target

A passing project must run locally as a full-stack app. The frontend, backend, database, authentication, favorites, score submission, and leaderboard must work together through API calls.
