# get-this-index
获取当前循环次数的索引值
```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
      <meta charset="UTF-8">
      <title>Document</title>
       <style type="text/css">
         #main li{
             display: inline-block;
             width: 100px;
             height: 100px;
             background: #aaa;
         }
       </style>
    </head>
    <body>
      <ul id="main">
        <li>0</li>
        <li>1</li>
        <li>2</li>
        <li>3</li>
        <li>4</li>
      </ul>
      
      <script type="text/javascript">
        var main=document.getElementById("main");
        var mains=main.getElementsByTagName("li");   
        for(var i=0;i<mains.length;i++){
          mains[i].index=i;  //重点就是在这里！
          mains[i].onclick=function(){
            this.style.background="red";
            console.log(this.index);
          }
        }
    
      </script>
    </body>
    </html>
```
