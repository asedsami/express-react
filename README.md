```
$ npm run dashboard
```
And voila!
this will run three commands concurrently(using concurrently-dashboard package), the first will watch and compile your backend ES6 code into ES5 whenever it changes. another one will start the compiled express server. and the third starts the webpack server for react development which is created using react-create-app.

If you're using tmux, concurrently-dashboard won't work and you need to use concurrently alone. you need two commands instead of one now:
```
$ npm run dev
```



