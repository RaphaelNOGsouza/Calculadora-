# Calculadora-
Fiz  uma calculadora 


CODIGO HTML:

<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    <link rel="stylesheet" href="script.js">
    <link rel="stylesheet" href="style.css">
    <title>Calculadora</title>
</head>
<body>
    <div>
        <form action="" name="Calculator">
            <input type="text" class="text maincolor" name="text1" disabled />
            <input type="text" class="text1 maincolor" name="text12" value="C" 
                        onclick="location.reload()" /><br>


            <input type="button" class="num maincolor" name="btn9" value="9" 
                        onclick="displaynum(btn9.value)" />
            <input type="button" class="num maincolor" name="btn8" value="8" 
                        onclick="displaynum(btn8.value)" />
            <input type="button" class="num maincolor" name="btn7" value="7" 
                        onclick="displaynum(btn7.value)" />
            <input type="button" class="num blue" name="addbtn" value="+" 
                        onclick="displaynum(addbtn.value)" /><br>


            <input type="button" class="num maincolor" name="btn6" value="6" 
                        onclick="displaynum(btn6.value)" />
            <input type="button" class="num maincolor" name="btn5" value="5" 
                        onclick="displaynum(btn5.value)" />
            <input type="button" class="num maincolor" name="btn4" value="4" 
                        onclick="displaynum(btn4.value)" />
            <input type="button" class="num pin" name="subbtn" value="-" 
                        onclick="displaynum(subbtn.value)" /><br>
            

            <input type="button" class="num maincolor" name="btn3" value="3" 
                        onclick="displaynum(btn3.value)" />
            <input type="button" class="num maincolor" name="btn2" value="2" 
                        onclick="displaynum(btn2.value)" />
            <input type="button" class="num maincolor" name="btn1" value="1" 
                        onclick="displaynum(btn1.value)" />
            <input type="button" class="num gre" name="mulbtn" value="*" 
                        onclick="displaynum" /><br>


            <input type="button" class="num maincolor" name="dot" value="." 
                        onclick="displaynum(dot.value)" />
            <input type="button" class="num maincolor" name="btn0" value="0" 
                        onclick="displaynum(btn0.value)" />
            <input type="button" class="num pur" name="eqlbtn" value="=" 
                        onclick="text1.value=eval(text1.value)" />
            <input type="button" class="num ora" name="divbtn" value="/" 
                        onclick="displaynum(div.value)" /><br>

        </form>
    </div>  
</body>
<script src="script.js"></script>
</html>


CODIGO JAVASCRIPT:

function displaynum(n1) {
    Calculator.text1.value = Calculator.text1.value + n1;
}


CODIGO CSS:

@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Lato:wght@100&display=swap');

body {
    width: 100%;
    right: 10vh;
    display: flex;
    align-items: center;
    justify-content: center;
    background: blue;
}

input {
    color: #fff;
    padding: 17px;
    outline: none;
    font-size: 30px;
    font-family: 'Bebas Neue', cursive;
    border-radius: 25%;
}

.num {
    width: 64px;
    height: 67px;
}

.tex {
    width: 160px;
    height: 26px;
    border-radius: 22px;
    letter-spacing: 5px;
    text-align: center;
    margin-bottom: 12px;
}

.text1 {
    width: 24px;
    height: 26px;
    border-radius: 50%;
    letter-spacing: 5px;
    text-align: center;
    margin-bottom: 12px;
    cursor: pointer;
}

.main {
    display: inline-block;
}

.maincolor {
    background-color: #000;
}

.blue {
    background-color: #0cd0cd;
}

.pin {
    background-color: #cf1596;
}

.gre {
    background-color: #aad800;
}

.pur {
    background-color: #8c52ff;
}

.ora {
    background-color: #fcb707;
}
