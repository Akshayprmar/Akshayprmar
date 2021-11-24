## Interview Question :-

Q:1:

```
let race = function() {
  setTimeout(() => console.log("timeout"), 0);
  setImmediate(() => console.log("immediate"));
  process.nextTick(() => console.log("nextTick"));
  console.log("current event loop");
}
race()
```
O/P:
```
current event loop
nextTick
timeout
immediate
```



