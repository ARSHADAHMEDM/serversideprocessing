## Design a Website for Server Side Processing

## AIM:
To design a website to perform mathematical calculations in server side.

## DESIGN STEPS:

### Step 1:

Create a new django project and app.

### Step 2:

Make on changes in settings and create templates folder.

### Step 3:

Create a code for frontend of calculation using HTML and CSS and save it in templates

### Step 4:

Give an url mapping and write a python code for calculation in views.

### Step 5:

Take a screenshot of the site and upload it.

### Step 6:

Publish the website in the given URL.

## PROGRAM :

```html

math.html

<!DOCTYPE html>
<html>
<head>
<meta charset='utf-8'>
<meta http-equiv='X-UA-Compatible' content='IE=edge'>
<title>Area of Rectangle</title>
<meta name='viewport' content='width=device-width, initial-scale=1'>
<style type="text/css">
body 
{
background-color:cyan;
}
.edge {
width: 1080px;
margin-left: auto;
margin-right: auto;
padding-top: 200px;
padding-left: 300px;
}
.box {
display:block;
border: Thick dashed lime;
width: 500px;
min-height: 300px;
font-size: 20px;
background-color: purple;
}
.formelt{
color: Red;
text-align: center;
margin-top: 5px;
margin-bottom: 5px;
}
h1
{
color: yellow;
text-align: center;
padding-top: 20px;
}
</style>
</head>
<body>
<div class="edge">
<div class="box">
<h1>Area of a Rectangle</h1>
<form method="POST">
{% csrf_token %}
<div class="formelt">
Length : <input type="text" name="length" value="{{l}}"></input>(in m)<br/>
</div>
<div class="formelt">
Breadth : <input type="text" name="breadth" value="{{b}}"></input>(in m)<br/>
</div>
<div class="formelt">
<input type="submit" value="Calculate"></input><br/>
</div>
<div class="formelt">
Area : <input type="text" name="area" value="{{area}}"></input>m<sup>2</sup><br/>
</div>
</form>
</div>
</div>
</body>
</html>

result.html

<!DOCTYPE html>
<html>
    <head>
        <title>SEC demo on server processing result</title>
    </head>
    <body>
        The result is {{result}}
    </body>
</html>


```

## OUTPUT:

![SERVER](serverout.png)

### Home Page:

![OUTPUT](clientout.png)

## Result:

The program for implementing server side processing is completed
