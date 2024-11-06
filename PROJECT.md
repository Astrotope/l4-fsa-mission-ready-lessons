# Project Log

## Week 01

### Day 01

- React orientation
  - Setup & ran create react [Create React](https://github.com/Astrotope/create-react)
  - Setup & ran create react with Typescript [Create React Typescript](https://github.com/Astrotope/create-react-typescript)

### Day 02

- PERN stack orientation (PERN App using Sequalize ORM with PostgreSQL, to store/edit/delete user info [email, city, phone] in db.
  - Dockerised a Full-stack PERN App [Fullstack: React Typescript + NodeJS Express + PostgreSQL](https://github.com/Astrotope/sern-ddd-app-typescript)
    - Based on [Tutorial Fullstack: React Typescript + NodeJS Express + PostgreSQL](https://www.tutofox.com/react/tutorial-fullstack-react-typescript-nodejs-express-postgresql/)
    - Built use node 22 LTS
    - Issues resolved
      - Removed personSlice exports from src/interfaces/Person.ts as this is the wrong module for this.
    - Current issues
      - There is some issue with the npm install during docker startup. The modules installed in the frontend/backend containers differ from those in the dev folder.
    - Start-up process before dockerising... (This setup worked as expected)
      - git clone https://github.com/Astrotope/sern-ddd-app-typescript.git
      - nvm use 22
      - cd sern-ddd-app-typescript
      - npm install
      - npm start (in a new terminal, in this folder) [Starts React Frontend]
      - cd node-backend
      - npm install
      - docker compose up & [Starts PostgreSQL] (Using original docker-compose.yml with just postgresql and outside of container db-url)
      - npm run dev [Starts Express Backend]

### Day 03

- PERN Typescript AI Chat App - AI backed chat app, with PostgreSQL backend using Prisma ORM, and Typesript
  - TODO: Setup repo for this and push it to githb. [Complete] [PERN - PostgreSQL, Express, React, Node - AI App](https://github.com/Astrotope/pern-ai-chat/tree/main)
  - Based on [PERN Stack Project: Build a Chat App From Scratch | Postgres, TypeScript, Prisma, React](https://youtu.be/vL24eiwAG_g?feature=shared)
    - Instaled the frontend and backend dependencies.
    - Used Vite for the frontend
    - Build out the server, routers, and controllers for login, along with the Prisma ORM and Schema
    - Setup PostgerSQL in docker container
    - Ran the PRISMA schema against the database, to generate the tables
    - Started building out the login, login ... controllers using the Prismas ORM backend and bcrypt for password hashing.
- Flex flow orientation.
  - Bulit the Facebook Pay page using the flex flow approach, and assets from the screen-capture
  - Code is here ... [Facebook Pay - Flex Flow](https://github.com/Astrotope/l4-fsa-mission-ready-lessons/tree/main/week-01/day-03/fb-pay)
  - Needs some work it is a little rought at the moment.
 

