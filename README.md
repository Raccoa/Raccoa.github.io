<html lang="en">
<center> 
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>  <center> 
    <div class="calculator-container">
        <h1>Claculatrice BMI </h1>
        <p>Taille en Metres:</p> 
        <input class="height-input-field" type="text">
        <p>Poids en Kg:</p>
        <input class="weight-input-field" type="text"><br>
        <button class="calculate"> Calcule</button>
    </div>
    <h3 class="result"></h3>
    <p class="result-statement"></p>
</center> 
    <script >
        var heightInput = document.querySelector(".height-input-field");
var weightInput = document.querySelector(".weight-input-field");
var calculateButton = document.querySelector(".calculate");
var result = document.querySelector(".result");
var statement = document.querySelector(".result-statement");
var BMI, height, weight; 

calculateButton.addEventListener("click", ()=>{
    
    height = heightInput.value;
    weight = weightInput.value;
    BMI = weight/(height**2); 
    result.innerText = BMI;

    if(BMI < 18.5){
        statement.innerText = "Votre BMI se situe dans la fourchette d’insuffisance pondérale";    
    }else if((BMI > 18.5) && (BMI <= 24.9)){
        statement.innerText = "Votre BMI se situe dans la fourchette de poids normal ou santé";
    }else if((BMI >= 25) && (BMI <= 29.9 )){
        statement.innerText = "Votre BMI se situe dans la fourchette de surpoids";
    }else{
        statement.innerText = "Votre BMI se situe dans la fourchette obèse";
    }
});

    </script>
    <img src = "" height = "500" width = 500 alt =>
</body>
</html>

<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01//EN">
<html>
<head>
  <title>My first styled page</title>
  <style type="text/css">
  body {
    color: White;
    background-color: #2904f8 }
  </style>
</head>
