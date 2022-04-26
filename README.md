Client Site: [https://github.com/sebokdas1/genius-car-service-map](https://github.com/sebokdas1/genius-car-service-map)
install all node and mongo and other: 
- npm init -y
- npm i express cors mongodb dotenv
for run: 
- npm run start-dev
---
installed jwt:
- npm i jsonwebtoken
---
Genarate access token on terminal:
- node
- require('crypto').randomBytes(64).toString('hex')






## Heroku deploy
  -------------------
 - ONE TIME for your computer
 - -----------------
 -  create heroku account
 -  verify email
 -  install heroku cli
 -  heroku login
 - --------------------
 - For each project one time
 - --------------------------
 -  heroku create
 -  make sure you: git add . git commit. git push
 -  git push heroku main
 -  Go to Heroku Dashboard > Current Project> Settings > Reveal Config vars
 -  copy paste config vars from your .env file
 -  Make sure you have whitelisted all ip address to access mongodb
 - --------------------
 - UPDATE SERVER with new changes
 - ------------------------
 -  Make changes
 -  make sure you: git add . git commit. git push
 -  git push heroku main
 - ---------------------
 - Connect Server with Client and deploy client
 - -------------------------
 -  replace localhost by heroku link
 -  npm run build
 -  firebase deploy
