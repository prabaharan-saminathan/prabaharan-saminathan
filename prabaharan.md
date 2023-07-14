<!DOCTYPE html>
<html>

<head>
   <meta charset="UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <link rel="stylesheet" href="praba2.css">
   <title>calculator</title>
   <style>
    *{
    margin:0;
    padding:0;
    box-sizing:border-box;
 }
 body{
    background-color:red;
    
 }
 .container{
    background-color:white;
    height:100vh;
    padding:15px;
    border:1px solid black;
    display:flex;
    justify-content:center;
    align-items:center;
  }
  .calculator{
     background-color:lightgrey;
     padding:10px;
     border-radius:10%;
     box-shadow: rgba(191, 60, 193, 0.25) 0px -23px 25px 0px inset, rgba(0, 0, 0, 0.15) 0px -36px 30px 0px inset, rgba(0, 0, 0, 0.1) 0px -79px 40px 0px inset, rgba(0, 0, 0, 0.06) 0px 2px 1px, rgba(0, 0, 0, 0.09) 0px 4px 2px, rgba(0, 0, 0, 0.09) 0px 8px 4px, rgba(0, 0, 0, 0.09) 0px 16px 8px, rgba(0, 0, 0, 0.09) 0px 32px 16px;
     
     
  }
  .calc{
    
    font-size:35px;
    opacity:0.7;
    text-align:center;
 }

.calculator form input{
   margin-top:25px;
   height:60px;
   width:60px;
   font-size:28px;
   border-radius:40px;
   text-align:center;
   border:none;
  box-shadow: rgba(100, 216, 170, 0.23) 0px -23px 25px 0px inset, rgba(0, 0, 0, 0.15) 0px -36px 30px 0px inset, rgba(0, 0, 0, 0.1) 0px -79px 40px 0px inset, rgba(0, 0, 0, 0.06) 0px 2px 1px, rgba(0, 0, 0, 0.09) 0px 4px 2px, rgba(0, 0, 0, 0.09) 0px 8px 4px, rgba(0, 0, 0, 0.09) 0px 16px 8px, rgba(0, 0, 0, 0.09) 0px 32px 16px;
    padding:8px;
   margin:6px;
   
}
form .display{
    display:flex;
    justify-content:end;
    align-items:end;
    
 }
 form .display input{
    height:100px;
   margin-top:30px;
   width:100%;
   border:none;
   box-shadow: rgba(190, 200, 40, 0.25) 0px 30px 60px -12px inset, rgba(0, 0, 0, 0.3) 0px 18px 36px -18px inset;
     padding:12px;
     text-align:end;
 }
 .calculator form input:hover{
    background-color: darkturquoise;
    color:white;
 }
 
 
 .equal{
  
    background-color:lightblue;
 }
 .br{
    display:flex;
     justify-content:center;
 }
   </style>
</head>

<body>
   <div class="container">
      <div class="calculator"><div class="calc"> PRABA.CALC
      <button>©</button></div>
        <form>
            <div class="display">
               <input type="text" name="display"
               id="input"placeholder="00000"></input>
            </div>
            <div>
               <input type="button" value="ac" onclick="display.value = ''">
         <input type="button" value="del" onclick="display.value = display.value.slice(0,-1)">
               <input type="button" value="%" onclick=display.value+="%">
               <input type="button" value="/" onclick=display.value+="/">
            </div>
            <div>
               <input type="button" value="7" onclick=display.value+="7">
               <input type="button" value="8" onclick=display.value+="8">
               <input type="button" value="9" onclick=display.value+="9">
               <input type="button" value="*" onclick=display.value+="*">
            </div>
            <div>
               <input type="button" value="4" onclick=display.value+="4">
               <input type="button" value="5" onclick=display.value+="5">
               <input type="button" value="6" onclick=display.value+="6">
               <input type="button" value="-" onclick=display.value+="-">
            </div>
            <div>
               <input type="button" value="1" onclick=display.value+="1">
               <input type="button" value="2" onclick=display.value+="2">
               <input type="button" value="3" onclick=display.value+="3">
               <input type="button" value="+" onclick=display.value+="+">
            </div>
            <div>
               <input type="button" value="00" onclick=display.value+="00">
               <input type="button" value="0" onclick=display.value+="0">
               <input type="button" value="." onclick=display.value+=".">

               <input type="button" value="=" class="equal" onclick="    display.value=eval(display.value)">
           
                </div>
                <div class="br">
                   <input type="button" value="(" onclick=display.value+="(">
                   <input type="button" value=")" onclick=display.value+=")">
                   
                </div>
         </form>
      </div>
   </div>
   <button onclick="display('try')"> try</button>
</body>

</html>


