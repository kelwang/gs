# gs
gopherjs related tools

go server

```
gstool "github.com/kelwang/gs/tool"

... ...

if c.DevMode() {
    gsOpts := &gbuild.Options{CreateMapFile: false}
    mux.Handle("/gs-src/", gstool.Handler("github.com/xxx/mygopherjs/", gsOpts, len("gs-src/")))
}else{
    // serve compiled javascript
    mux.Handle("/js/script/script.js", aStaticHandler)
}
 ```
 
 html
 ```
    <script src="/gs-src/script/script.js"></script> 
 ```
 
 gopherjs folder
 ```
 /mygopherjs
 --/script/main.go
 ```
 
 
