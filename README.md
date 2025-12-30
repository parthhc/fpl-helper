# FPL Player Comparison Tool ⚽

A data-driven tool for Fantasy Premier League managers to analyze live player and team data, leading to a proven 35% improvement in global rank.

## ✨ Features

- **Data Scraping**: Uses Puppeteer to aggregate and merge live data from three different soccer statistics sites.
- **Performance Insights**: Analyses data for over 1,000 players to help users make strategic transfers.
- **RESTful API**: A custom Node.js API serves processed data from MongoDB to the frontend.

## 🛠️ Tech Stack

- **Frontend**: React
- **Backend**: Node.js, Express
- **Database**: MongoDB, Mongoose
- **Tools**: Puppeteer, Postman

## Run Application

- Clone the repository.
- Install dependencies.
  ```
  cd server
  npm install
  cd ..
  cd client
  npm install
  ```
- Create a MongoDB database, save the connection URI.
- Create `config.env` file, add variables for `DATABASE_CONN`, `CHROME_EXECUTABLE_PATH`, `NODE_ENV`. `NODE_ENV` is either development or production. `DATABASE_CONN` is MongoDB connection string. `CHROME_EXECUTABLE_PATH` is the path to run Chrome from on your machine.
- To run the backend
```
cd server
npm index.js
```
OR
```
cd server
nodemon index.js
```
for continuous running.
- To run the frontend:
```
cd client
npm run dev
```
for development, or
```
cd client
npm run build
```
for production.
