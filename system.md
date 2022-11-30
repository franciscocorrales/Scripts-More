# System

### Get process list

```js
ps
```

### Process in port

```js
netstat -an | grep <PORT>
netstat -an | grep 27017

lsof -i tcp:<PORT>
lsof -i tcp:27017
```

### Kill process

```js
kill -9 <PORT>
kill -9 27017
```

### Get website address, DNS information

```js
dig google.com
```
