<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

## Description

A responsive anime website built with Next.js and Tailwind CSS, featuring dynamic discussions and comprehensive anime ratings. This project utilizes a Nest.js backend to manage API endpoints and data processing, providing a seamless user experience for anime enthusiasts.

## Getting Started

### Reuqirements

- [Node.js](https://nodejs.org/) (v14.x or higher)
- [yarn](https://yarnpkg.com/)
- [PostgreSQL](https://www.postgresql.org/) (v12 or higher)
- [Git](https://git-scm.com/)

### Step 1 -- Instalation Dependecies

```bash
yarn install
```

### Step 2 -- Configuration

```bash
# Copy the .env.example file to .env
cp .env.example .env
```

### Step 3 -- How to Use

```bash
# Run the App
npm run start:dev

# Access via postman or others for testing
http://localhost:4321
```

## Api Endpoints

Here are some of the main temporary endpoints available in this application:

- Anime:

  - POST /anime/post: Adding new anime.
  - GET /anime/get/:id: Get a list of anime details by ID.
  - GET /anime/get: Get all anime.
  - GET /anime/get/by-genre/:id: Get a list of anime by genre ID.
  - PUT /anime/update/:id: Update anime data.
  - DELETE /anime/delete/:id: Soft delete anime by ID.
  - GET /anime/popular: Display recommended anime data.

- Genre:

  - POST /genre/post: Adding new genre.
  - PUT /genre/update/:id: Update genre data.
  - DELETE /genre/delete/:id: Delete genre data.
  - GET /genre/get-all: Get all existing genre data.

- Review:

  - GET /review/get-all: Get all existing review data.
  - GET /review/get/:id: Get a list of review details by ID
  - POST /review/post: Adding new review.
  - PUT /review/update/:id: Update review data.
  - PUT /review/restore/:id: Restore review data
  - DELETE /review/delete/:id: Delete review data.

- Photo_anime:

  - GET /photo-anime/get-all: Get all photo anime.
  - PUT /photo-anime/update/:id: Update data photo anime.
  - DELETE /photo-anime/delete/:id: Delete data photo anime.

- Topic:

  - POST /topic/post: Adding new data topic.
  - GET /topic/get/:id: Get a list of topic details by ID.
  - PUT /topic/update/:id: Update topic data.
  - DELETE /topic/delete/:id: Delete data topic.

- Photo_topic:

  - PUT /photo-topic/update/:id: Update topic photo data.
  - DELETE /photo-topic/delete/:id: Delete data photo topic

- Like_topic:

  - POST /like-topic/post: Add new data like topic.
  - DELETE /like-topic/delete/:id: Delete topic likes data.

- Favorite_anime:

  - POST /favorite-anime/post: Add new data favorite anime.
  - PUT /favorite-anime/restore/:id: Restore anime favorite data.
  - DELETE /favorite-anime/delete/:id: Delete anime favorite data.

- Comment:

  - POST /comment/post: Add new comment data.
  - PUT /comment/update/:id: Update comment data.
  - PUT /comment/restore/:id: Restore comment data.
  - DELETE /comment/delete/:id: Delete comment data.

- Like_comment:

  - POST /like-comment/post: Add new data like comment.
  - DELETE /like-comment/delete/:id: Delete comment likes data.

- User:
  - GET /user/get-all: Get a list of all user data with the role user.

- Auth:
  - POST /auth/login: Validates the user's credentials and generates a JWT (JSON Web Token) as an authentication token.
  - POST /auth/register: Register new users into the database system.

- Dashboard
  - GET /dashboard/total-topic: Display the number of topic data.
  - GET /dashboard/anime-top: Display top anime data all time.
  - GET /dashboard/total-premium: Display the number of premium members with user role.

## Project Developer

- Backend - [Akbar Ridho Arrafi](https://github.com/AkbarF0rce)
- Frontend - [Fadlan Hamsyari Priyanto](https://github.com/Rcikaym)
