### Install Client Library for Node
```
npm install redis
```

### Install and Start Redis via brew
```
brew services start redis
```

### Install and Start Redis on Windows
```
https://github.com/MicrosoftArchive/redis/releases
redis-server.exe
```

### Ping Server
```
redis-cli ping
```

### Connection String
```js
const redisUrl = 'redis//127.0.0.1:6379';
```
