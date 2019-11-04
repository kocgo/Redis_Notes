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

### Create Client
```js
const client = redis.createClient(redisUrl);
```

### Storing/Setting A Key-Value Pair
```js
client.set('greeting', 'hello') // Returns true or false {'greeting': 'hello'}
```

### Getting A Key-Value Pair
```js
// Returns true or false
client.get('greeting', (err,value) => {
  console.log(value); // Will log 'hello'
}
```

### Easy way to log
```js
client.get('greeting', console.log);
```
