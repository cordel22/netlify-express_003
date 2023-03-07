
github:

https://github.com/cordel22/netlify-express_003

doesnt build on netlify:(

builds on local tho

the code is from this blocg's reference:

https://www.netlify.com/blog/2018/09/13/how-to-run-express.js-apps-with-netlify-functions/




An example of how to host an Express.js app on Netlify using serverless-http. See express/server.js for details, or check it out at https://netlify-express.netlify.com/!

index.html simply loads html from the Express.js app using <object>, and the app is hosted at /.netlify/functions/server. Examples of how to access the Express.js endpoints:

curl https://netlify-express.netlify.com/.netlify/functions/server
curl https://netlify-express.netlify.com/.netlify/functions/server/another
curl --header "Content-Type: application/json" --request POST --data '{"json":"POST"}' https://netlify-express.netlify.com/.netlify/functions/server