asuth's experiment around prompting via an add-on:

https://github.com/mozilla-b2g/gaia-email-libs-and-more/blob/cc30f069e5595222315e685c967f13d07fe20ae6/lib/tcp_permissions.js
https://github.com/mozilla-b2g/gaia-email-libs-and-more/blob/cc30f069e5595222315e685c967f13d07fe20ae6/lib/main.js


## APIs

chrome.sockets.tcp:
https://developer.chrome.com/apps/sockets_tcp

mozTCPSocket:
https://developer.mozilla.org/en/docs/Web/API/Navigator/mozTCPSocket

```javascript
// options could have a prompt: true, if prompting the user is desirable, not
// been granted yet. For background sync would not pass prompt: true, or if it
// was passed, ignored.
navigator.socket.mail(options).then(function(socketAPI) {
  socketAPI.open();

}, function(err) {
  // not allowed
});
```

## Specs

Now defunct?
Spec draft: http://www.w3.org/2012/sysapps/tcp-udp-sockets/
On GitHub: https://github.com/sysapps/tcp-udp-sockets
