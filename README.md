# Web Page for Mathematical Calculations

## AIM:

To design a static website with validation to perform mathematical calculations in client side.

## DESIGN STEPS:

### Step 1:

Requirement collection.

### Step 2:

Creating the layout using HTML and CSS.

### Step 3:

Write javascript to perform the calculations.

### Step 4:

Include regularexpression based input validation.

### Step 5:

Validate the layout in various browsers.

### Step 6:

Validate the HTML code.

### Step 6:

Publish the website in the given URL.

## PROGRAM :
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Javascript</title>
    <style>
        * {
            box-sizing: border-box;
            font-family: Arial, Helvetica, sans-serif;
        }
        body {
            color: snow;
            background-image: url("https://th.bing.com/th/id/OIP.YdvxTTDIR-a-0C8fGsF63gHaEo?w=278&h=180&c=7&r=0&o=5&pid=1.7");
            background-repeat: no-repeat;
            background-size: cover;
        }    
        .container{
            background-size: 700px 500px ;
            width: 700px;
            height: 400px;
            text-align: center;
            border-style: solid;
            border-color: white;
            margin-left: 300px;
            display: inline-block;
         }
        .container1{
            
            width:700px;
            height:400px;
            text-align:center;
            border-style: solid;
            border-color: white;
            margin-left: 300px;
            margin-top: 10px;
        }
        .content {
            display: block;
            width: 100%;
            min-height: 500px;
            margin: 0px 0px 0px 0px;
            margin-top: 65px;
            }
        .content2 {
            display: block;
            width: 100%;
            min-height: 500px;
            margin: 0px 0px 0px 0px;
            margin-top: 65px;
            }
        h1{
            text-align: center;
        }
        h2{
            text-align: center;
            padding-top: 20px;
            font-style: italic;
        }
        .formelement{
            text-align: center;

        }
    </style>
</head>
<body>
    <h1><u>【CALCULATOR】</u></h1>
    <div class="container">
        <div class="content">
            <h2>𒆜<u>Volume</u> <u>of</u> <u>a</u> <u>Pyramid</u>𒆜</h2>
            <form>
                <div class="formelement"></br>
                    <label for="aedit">Enter Base area:</label>
                    <input type="text" id="aedit" value=" "/><label> cm</label>
                </div>
                <div class="formelement">
                </br>
                    <label for="bedit">Enter Height:</label>
                    <input type="text" id="bedit" value=" "/><label> cm</label>
                </div>
                <div class="formelement">
                </br>
                    <input type="button" value="Calculate" id="addbutton"/>
                </div>
                <div class="formelement">
                </br>
                    <label for="cedit">Volume:</label>
                    <input type="text" id="cedit" readonly value=" "/><label> cm³</label>
                </div>
            </form>
    </div>
    </div>
    <div class="container1">
    <div class="content2">
        <h1>𒆜<u>Volume</u> <u>of</u> <u>a</u> <u>Cone</u>𒆜</h1>
        <form>
            <div class="formelement"></br>
                <label for="dedit">Enter Radius:</label>
                <input type="text" id="dedit" value=" "/><label> cm</label>
            </div>
            <div class="formelement">
            </br>
                <label for="eedit">Enter Height:</label>
                <input type="text" id="eedit" value=" "/><label> cm</label>
            </div>
            <div class="formelement">
            </br>
                <input type="button" value="Calculate" id="button"/>
            </div>
            <div class="formelement">
            </br>
                <label for="fedit">Volume:</label>
                <input type="text" id="fedit" readonly value=" "/><label> cm³</label>
            </div>
        </form>
</div>
    </div>
<script type="text/javascript">
    var button;
    button=document.querySelector("#addbutton");
    button.addEventListener("click",function(){
        var atext,btext,ctext;
        var aval,bval,cval;
        atext=document.querySelector("#aedit");
        btext=document.querySelector("#bedit");
        ctext=document.querySelector("#cedit");

        aval = parseInt(atext.value);
        bval = parseInt(btext.value);
        cval = 1/3*(aval*aval)*bval;
        ctext.value=""+cval;
    });
    button=document.querySelector("#button");
    button.addEventListener("click",function(){

        var dtext,etext,ftext;
        var dval,eval,fval;

        dtext=document.querySelector("#dedit");
        etext=document.querySelector("#eedit");
        ftext=document.querySelector("#fedit");

        dval = parseInt(dtext.value);
        eval = parseInt(etext.value);
        fval = 3.14*(dval*dval)*(eval/3);
        ftext.value=""+fval;

    });
</script>
</body>
</html>
~~~
## OUTPUT:
![OUTPUT](./calculations/img/cal1.png)
![OUTPUT](./calculations/img/cal2.png)

## Result:

Thus a website is designed to perform mathematical calculations in the client side.
