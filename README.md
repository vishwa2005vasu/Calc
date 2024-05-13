# Ex.08 Design of a Standard Calculator
## Date:10/5/24

## AIM:
To design a web application for a standard calculator with minimum five operations.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for creating attractive colors.

### Step 4:
Write JavaScript program for implementing five different operations.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
calc.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculator</title>
    <link rel="stylesheet" type="text/css" href="calculator.css">
</head>
<body>
<center>
<h3> VISHWA VASU (212222040183) </h3>
</center>
<div class="calculator">
    <input type="text" id="display" readonly>
    <input type="button" value="(" onclick="addToDisplay('(')">
    <input type="button" value=")" onclick="addToDisplay(')')">
    <input type="button" value="C" onclick="clearDisplay()">
    <input type="button" value="%" onclick="addToDisplay('%')">
    <input type="button" value="7" onclick="addToDisplay('7')">
    <input type="button" value="8" onclick="addToDisplay('8')">
    <input type="button" value="9" onclick="addToDisplay('9')">
    <input type="button" value="*" onclick="addToDisplay('*')">
    <input type="button" value="4" onclick="addToDisplay('4')">
    <input type="button" value="5" onclick="addToDisplay('5')">
    <input type="button" value="6" onclick="addToDisplay('6')">
    <input type="button" value="-" onclick="addToDisplay('-')">
    <input type="button" value="1" onclick="addToDisplay('1')">
    <input type="button" value="2" onclick="addToDisplay('2')">
    <input type="button" value="3" onclick="addToDisplay('3')">
    <input type="button" value="+" onclick="addToDisplay('+')">
    <input type="button" value="0" onclick="addToDisplay('0')">
    <input type="button" value="." onclick="addToDisplay('.')">
    <input type="button" value="/" onclick="addToDisplay('/')">
    <input type="button" value="=" onclick="calculate()">
</div>

<script src="index.js"></script>

</body>
</html>

calculator.css

.calculator 
{
    width: 220px;
    margin: 0 auto;
    border: none;
    border-radius: 15px;
    padding: 10px;
    background-color: #15ba9e;
    display: grid;
    grid-template-columns: repeat(4, 50px);
    grid-gap: 5px;
}

input[type="button"] 
{
    width: 50px;
    padding: 10px;
    font-size: 18px;
    border: none;
    border-radius: 15px;
    cursor: pointer;
    background-color: #d1ebe4;
    color: rgb(123, 17, 17);
}

input[type="text"] 
{
    grid-column: span 4;
    padding: 10px;
    font-size: 18px;
    border: 1px solid #0b0b0b;
    border-radius: 15px;
}

index.js

function addToDisplay(value) 
{
    document.getElementById('display').value += value;
}

function calculate() 
{
    var expression = document.getElementById('display').value;
    var result = eval(expression);
    document.getElementById('display').value = result;
}

function clearDisplay() 
{
    document.getElementById('display').value = '';
}
```

## OUTPUT:

![Screenshot (11)](https://github.com/vishwa2005vasu/Calc/assets/135954202/9ff5613e-2686-47f4-8a34-0768ddefef1b)
![Screenshot (12)](https://github.com/vishwa2005vasu/Calc/assets/135954202/049478a8-e50e-4161-8603-dfe329a974a3)


## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
