## How to run server

```python
python miniredis.py
```


## Redis command examples

### PING command
```
echo -e "*1\r\n\$4\r\nPING\r\n" | nc 127.0.0.1 6379
```

Output
```
+PONG
```

### SET command
```
$ echo -e "*3\r\n\$3\r\nset\r\n\$5\r\nmykey\r\n\$1\r\n1\r\n" | nc 127.0.0.1 6379
```

Output
```
+OK
```

### GET command
```
echo -e "*2\r\n\$4\r\nINCR\r\n\$5\r\nmykey\r\n" | nc 127.0.0.1 6379
```

Output
```
$1
1
```
