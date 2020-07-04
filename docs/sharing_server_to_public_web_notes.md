# Ways of sharing your development work to the public web.

1. localtunnel
   1. punches a hole in your firewall so your local server is available
   2. It creates a URL on a public web server that is hosting your content (or redirecting, or something)
   3. running it is as simple as:
      1. npm install localtunnel -g
      2. Start your app
      3. lt --port 3000 -h "http://serverless.social"
         1. This is an update, see [this StackOverflow Q&A](https://stackoverflow.com/a/60621979/6501141)
         2. If it works, it will report back the live url to use
2. ngrok
   1. Basics
      1. punches a hole in firewall
      2. provides access via a public web server
      3. possible to use for web hosting as well
   2. additional features (securetunnel)
   3. but additional setup required
   4. Instructions
      1. Sign up on web page
      2. Install ngrok
      3. Install authtoken
      4. Start your app
      5. ./ngrok http 80
   5. You can password protect access
3. now
   1. low-friction way to deploy node.js apps to the cloud
   2. new URL every time you use it
   3. Instructions
      1. npm install -g now
      2. Create start script
      3. now
   4. Publishes files to a public server, so available permanently (good and bad)
4. Surge
   1. Quickly host static files to public URL
   2. Can be used for final hosting platform as well
   3. Setup
      1. setup surge account
      2. npm install -g surge
      3. surge
