# NoGames 

## Final Product 

!["Start Game"](https://github.com/Nschulz88/jungle-rails/blob/master/public/imgs/nogames_homepage_screenshot.png)

!["Play Game"]((https://github.com/Nschulz88/jungle-rails/blob/master/public/imgs/nogames_game_screenshot.png))

!["End Game"]((https://github.com/Nschulz88/jungle-rails/blob/master/public/imgs/nogames_endgame_screenshot.png))



## Getting Started

1. Clone this repository (do not fork)
2. Remove the git remote: `git remote rm origin`
3. Make sure you have a db runnning (PostgreSQL preferred as project is setup for ppsql)
4. Create your `.env` by using `.env.example` as a reference: `cp .env.example .env`
   --> Create base DB in your DB app of choice and make sure your DB name aligns with your DB_NAME in the .env file
5. For ease of setiing this up and simply running immidiately comment out as follows in the knexfile.js :
```       // host     : process.env.DB_HOST,
      // user     : process.env.DB_USER,
      // password : process.env.DB_PASS,
      database : process.env.DB_NAME,
      // port     : process.env.DB_PORT,
```
6. Update the .env file with your correct local information
7. Install dependencies: `npm i`
8. Fix to binaries for sass: `npm rebuild node-sass`
9. Run migrations: `npm run knex migrate:latest`
10. Run the seed: `npm run knex seed:run`
11. Run the server: `npm run local`
12. Visit `http://localhost:8080/`
13. Play a game and beat the bot !!




## Dependencies

- Node 5.10.x or above
- NPM 3.8.x or above
- body-parser
- dotenv
- ejs
- express
- knex
- knex-logger
- node-sass-middleware
- pg

- REMINDER: Must have running DB (PostgreSQL preferred)