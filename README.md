# Angular-TypeScript

Simple AngularJS Application with TypeScript

# Usage

- Install global dependencies **if necessary**

  ```
    npm install -g gulp-cli typings
  ```

- Install node packages:

  ```
   npm install
  ```

- Launch the server

  ```
   npm start
  ```

## Throubleshooting

If you are in ** Linux ** and you get a bug related to the watch when running gulp like the following,

```
[13:53:08] 'watch' errored after 8.99 ms
[13:53:08] Error: watch ENOSPC
    at errnoException (fs.js:1024:11)
    at FSWatcher.start (fs.js:1056:11)
    at Object.fs.watch (fs.js:1081:11)
```

it is solved by running the following command:

```sh
$ echo fs.inotify.max_user_watches=524288 | sudo tee -a /etc/sysctl.conf && sudo sysctl -p
```
