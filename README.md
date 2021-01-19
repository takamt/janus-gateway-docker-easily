## Descriptions

- Provide WebRTC with Janus using janus-gateway.
- Easy access to janus-gateway sample pages ready-to-run WebRTC.
- For more information about janus-gateway, see https://github.com/meetecho/janus-gateway.

## Usage

```
$ docker-compose up -d

// → access to http://localhost:8080/ or https://localhost:1443/
```

## Note

### Janus HTML

- Below the janus directory is basically copies of the files generated when janus is installed.
  - Same as /usr/local/src/janus-gateway/html/

### Janus Server

- Janus server name depends on the location of nginx proxy pass requests from port 8088(HTTP), 8089(HTTPS).

```janus/janus.js
- var server = gatewayCallbacks.server;
+ // var server = gatewayCallbacks.server;
+ var server = '/janusbase/janus';
```


### SSL certificate keys

- You can change the SSL certificate keys.

## Copyright

- See ./LICENSE

