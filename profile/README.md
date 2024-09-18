# MazeWith 🌀

<a href="https://mazewith.me/" style="text-align:center; display:block;">https://mazewith.me/</a>

![MazeWith](../Resources/favicon.png)

**MazeWith** is a full-stack, real-time multiplayer maze game built with React & TypeScript. Players use their mobile devices as controllers to navigate the maze. The game screen displays the maze and player movements in real-time.

## 🚀 Project Overview

**MazeWith** is a multiplayer game where players control their character through a maze using their phones as controllers. The game is separated into three key components:

1. [**Website**](https://github.com/mazewith/website): Provides an introduction to the game, its features, and a guide on how to play.
2. [**Game Screen**](https://github.com/mazewith/game): Displays the maze, real-time player movement, and game status.
3. [**Controller**](https://github.com/mazewith/controller): Allows players to control their characters using their mobile devices.

---

## 🛠️ Tech Stack

### Frontend <a href="https://reactjs.org/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" alt="react" width="24" height="24"/></a> <a href="https://www.typescriptlang.org/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/typescript/typescript-original.svg" alt="typescript" width="24" height="24"/></a> <a href="https://tailwindcss.com/" target="_blank" rel="noreferrer"><img src="https://www.vectorlogo.zone/logos/tailwindcss/tailwindcss-icon.svg" alt="tailwind" width="24" height="24"/></a>

- **React** (TypeScript): Main framework for building the website, game screen, and controller components. It manages the game logic, dynamically generates mazes, and determines valid player movements based on the maze structure. Data is updated and re-rendered in real-time.

### Backend <a href="https://firebase.google.com/" target="_blank" rel="noreferrer"><img src="https://www.vectorlogo.zone/logos/firebase/firebase-icon.svg" alt="firebase" width="24" height="24"/></a> <a href="https://redis.io/" target="_blank" rel="noreferrer"><img src="https://www.vectorlogo.zone/logos/redis/redis-icon.svg" alt="redis" width="24" height="24"/></a> <a href="https://aws.amazon.com/lambda/" target="_blank" rel="noreferrer"><img src="https://www.vectorlogo.zone/logos/amazon_aws/amazon_aws-icon.svg" alt="aws-lambda" width="24" height="24"/></a>

- **Firebase** (Realtime Database): Stores player positions, game state, and maze configurations.
- **Redis**: Used to track game room details such as `createdAt`, `roomId`, and `joins` for efficient real-time updates and displaying game stats like most recent and most played rooms.
- **AWS Lambda**: Handles serverless processing of game room data. When players create or join a room, the game sends the data to an AWS Lambda function, which processes it and stores it in Redis for fast retrieval.

### DevOps and Infrastructure

- **GitHub Actions**: Automated CI/CD pipeline to deploy the application.
- **Domain & SSL**: The game is hosted on a custom domain with SSL encryption, ensuring secure communication and a professional user experience. The SSL certificate was set up to provide HTTPS access, which is crucial for modern web applications.

![Architecture](../Resources/architecture.jpg)

---

## 📫 Contact

Feel free to reach out if you have any questions or suggestions for improvements!

- **Email**: [info@mazewith.me](mailto:info@mazewith.me)
