
# mouse simulator

```js
javascript:(()=>{if(window.__topTouchpadLR2)return;window.__topTouchpadLR2=1;const d=document,b=d.body,p=d.createElement("div"),l=d.createElement("div"),r=d.createElement("div"),c=d.createElement("div");let cx=innerWidth/2,cy=innerHeight/2,drag=0;Object.assign(c.style,{position:"fixed",width:"20px",height:"20px",border:"2px solid #4fd1c5",borderRadius:"50%",background:"rgba(79,209,197,.15)",pointerEvents:"none",zIndex:99999,transform:"translate(-50%,-50%)"});Object.assign(p.style,{position:"fixed",top:"16px",right:"20px",transform:"translateX(-50%)",width:"260px",height:"160px",background:"rgba(0,0,0,.45)",borderRadius:"12px",touchAction:"none",zIndex:99998,color:"#fff",fontFamily:"monospace"});Object.assign(l.style,{position:"absolute",bottom:0,left:0,width:"50%",height:"44px",background:"rgba(255,255,255,.12)",borderRadius:"0 0 0 12px",display:"flex",alignItems:"center",justifyContent:"center",fontSize:"16px",fontWeight:"bold"});Object.assign(r.style,{position:"absolute",bottom:0,right:0,width:"50%",height:"44px",background:"rgba(255,255,255,.18)",borderRadius:"0 0 12px 0",display:"flex",alignItems:"center",justifyContent:"center",fontSize:"16px",fontWeight:"bold"});l.textContent="L";r.textContent="R";p.append(l,r);b.append(p,c);const fire=(t)=>d.elementFromPoint(cx,cy)?.dispatchEvent(new MouseEvent(t,{bubbles:1,cancelable:1,view:window,clientX:cx,clientY:cy,screenX:cx,screenY:cy,button:0,buttons:drag?1:0}));c.style.left=cx+"px";c.style.top=cy+"px";let lx,ly;p.addEventListener("touchstart",e=>{const t=e.touches[0];lx=t.clientX;ly=t.clientY});p.addEventListener("touchmove",e=>{const t=e.touches[0],dx=t.clientX-lx,dy=t.clientY-ly;lx=t.clientX;ly=t.clientY;cx=Math.max(0,Math.min(innerWidth,cx+dx*1.2));cy=Math.max(0,Math.min(innerHeight,cy+dy*1.2));c.style.left=cx+"px";c.style.top=cy+"px";drag&&fire("mousemove")},{passive:!1});l.addEventListener("touchstart",e=>{drag=1});l.addEventListener("touchend",e=>{fire("click");drag=0});r.addEventListener("touchstart",e=>{drag=1;fire("mousedown")});r.addEventListener("touchend",e=>{fire("mouseup");drag=0});})();
 ```





# web projects

| name | Link | demo|
| ------ | ------ | ------ |
| owl-locator | [owl-locator](https://github.com/Jisan901/Owl-locator-v1-client) | [demo](https://owl-locator.firebaseapp.com/) |
| Node editor three js | [node editor](https://github.com/Jisan901/tsl-editor/)| [demo](https://jisan901.github.io/Tsl-editor/) |
|course site| [dev-server-v1](https://github.com/Jisan901/development-server-v1)| [demo](https://risosi.onrender.com/)|
|govt official| [govt server](https://github.com/Jisan901/Client-gov)|[demo](https://govt-service.web.app/)|


