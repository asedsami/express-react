```
$ npm run dashboard
```
And voila!
this will run three commands concurrently(using concurrently-dashboard package), the first will watch and compile your backend ES6 code into ES5 whenever it changes. another one will start the compiled express server. and the third starts the webpack server for react development which is created using create-react-app. the create react app server does everything for the client side. the `/client` directory is created using the command `create-react-app client` and I didn't changed it except for adding a proxy field in `/client/package.js` in order to get rid of CORS... this you way, in your react app you don't call `localhost:8000/someApiMethod` which is the url for the express api. you call `/someApiMethod` and the cra server proxies it to the express api.

If you're using tmux, concurrently-dashboard won't work and you need to use concurrently alone. (using the below npm script)
```
$ npm run dev
```



