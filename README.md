# Realtime Chat Application  

[The site](https://spacechatapp.netlify.app/)  

This is the repository made via a tutorial whose link is - [Build and Deploy a Realtime Chat Application - Socket.io, Node.js, and React.js - JavaScript Mastery](https://www.youtube.com/watch?v=ZwFA3YMfkoc)  


### Start  
1. ` npx create-react-app client `
2. ` cd client && npm install --save react-router socket.io-client react-scroll-to-bottom react-emoji query-string `
3. Create another directory named 'server'    
4. ` cd server && npm init -y `  
5. ` npm install --save cors nodemon express socket.io `  
### Client Side  
6. Remove all unnecessary files in client/src folder and create index.js and App.js. Copy the code
7. In client/src/components, copy all the components found  
8. Components include  
    - Join
    - Chat
    - Input
    - Infobar
    - Messages and Message
    - TextContainer
### Server Side 
8. In server create index.js, router.js and users.js  
9. Copy the code
### Deploy
10. Login to Heroku and Netlify. Download Heroku cli and Netlify cli
11. Create a new Heroku app
12. In server folder do the following -  
`git init  heroku git:remote -a heroku-app-name git add .  git commit -m "commit message"  git push heroku master  `
13. Copy the heroku app server website link and paste it in client/src/components/Chat/Chat.js as
` const ENDPOINT = 'https://link'; `  
14. `cd ../client && npm run build  netlify deploy`
15. Make Publish Directory as ./build
16. `netlify deploy --prod` and your react chat application is deployed successfully!!  
  
### Alternatively Setup: 
`npm i && npm start` for both client and server sude to start the development server 