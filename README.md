
# mouse simulator

```js
function createMouseEvent(e,t){const n=t.changedTouches[0],c=new MouseEvent(e,{bubbles:!0,cancelable:!0,view:window,detail:t.detail,screenX:n.screenX,screenY:n.screenY,clientX:n.clientX,clientY:n.clientY,ctrlKey:t.ctrlKey,shiftKey:t.shiftKey,altKey:t.altKey,metaKey:t.metaKey,button:0,buttons:1});t.target.dispatchEvent(c)}document.addEventListener("touchstart",(e=>{createMouseEvent("mousedown",e)})),document.addEventListener("touchmove",(e=>{createMouseEvent("mousemove",e)})),document.addEventListener("touchend",(e=>{createMouseEvent("mouseup",e)}));
 ```





# web projects

| name | Link | demo|
| ------ | ------ | ------ |
| owl-locator | [owl-locator](https://github.com/Jisan901/Owl-locator-v1-client) | [demo](https://owl-locator.firebaseapp.com/) |
| Node editor demo | [node editor](https://github.com/Jisan901/node-editor)| [demo](https://node-editor-fxql-d48ah75gs-jisan901.vercel.app/) |
|course site| [dev-server-v1](https://github.com/Jisan901/development-server-v1)| [demo](https://risosi.onrender.com/)|
|govt official| [govt server](https://github.com/Jisan901/Client-gov)|[demo](https://govt-service.web.app/)|


