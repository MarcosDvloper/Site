                <!DOCTYPE html>
<html lang="es">
    
 <head>
    <meta charset="UTF-8">
    <title>Contador</title>
    <link rel="stylesheet" href="count.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Tektur&display=swap" rel="stylesheet">
 </head>

<body>
    
  <div class="container">
      
         <p id="resul">0</p>
         
    <div class="buttons">
     <button id="btn2" onclick="decrementar()">Restar</button>
     <button id="btn3" onclick="reset()">Reiniciar</button>
     <button id="btn1" onclick="incrementar()">Sumar</button>
    </div>
         <button id="btn4" onclick="compra()">Comprar</button>
  </div>
     
 <script>
        
const btnIter = document.getElementById("btn1");
const btnDecr = document.getElementById("btn2");     
const resultado = document.getElementById("resul") 
const btnReser = document.getElementById("btn3");     
      
let count = parseInt(0);      

function compra(){

let conf = window.confirm("¿Comprar potenciador?")
    if(conf == true){
        count *= 2
        resultado.textContent = count;
    }else{
        alert("Te lo perdés😌")
    }
}

function incrementar(){
       count++;
       resultado.textContent = count;
}

function decrementar(){
       count--;
       resultado.textContent = count;
}

function reset(){
       count = 0;
       resultado.textContent = count;
}

 </script>
</body>


</html>
