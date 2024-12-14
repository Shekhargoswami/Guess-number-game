<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <title> Number Guess</title>
    <style>
      body,html{
        margin: 0;
        padding: 0;
        height: 100%;
        background-color: rgb(60, 78, 83);
    }
    .container{
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
       
    .box{
        background-color: rgb(185, 188, 189);
        color: black;
        text-align: center;
        padding: 10px 20px;
        border-radius: 10%;
        border: 10px solid black;
        
        
        
    }
   
    button{
        padding: 5px 20px;
        border-radius: 10px;
        color: black;
        background-color: rgb(211, 211, 211);
        border: 3px solid rgb(60, 34, 34);
    }
   
    }
    button:hover{
        background-color: antiquewhite;
        color: black;
    }
    </style>
  
  </head>
  
  <body>
   <div class="container">
    <div class="box">
     <h1>Number guess</h1><br><br>
  <input id="num1" type="number">
  <button onclick="guess()">submit</button>
    </div>
   </div>
    
    <script >
      let rand =Math.floor(Math.random()*10);
function guess(){
  let input =parseInt(document.getElementById("num1").value);
  if (input==rand){
    document.getElementById("you won the game").innerHTML="yupppp...";
  }
  else if(input< rand){
    alert ("Guess a higher number");
  }
  else{
    alert("guees a lower number");
  }
}
    </script>
  </body>
</html># Guess-number-game
