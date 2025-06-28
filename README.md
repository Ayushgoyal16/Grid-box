#Html code for Gridbox
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grid box</title>
    <link rel="stylesheet" href="C:\Users\goyal\Desktop\HTML\style01.css"/>
</head>
<h1>Grid Playground</h1>
<div class="container">
    <div id="ayush1">Item-1</div>
    <div id="ayush2">Item-2</div>
    <div id="ayush3">Item-3</div>
</div>
<span>Ayush Goyal</span>
<hr/>
<h1 id="rabba">Animations</h1>
<div id="lenovo">
    <div class="caps"> Ayush Goyal</div><br/>
    <div class="caps">Software Engineer</div><br/>
    <div class="caps">Software Deweloper</div><br/>
    <div class="caps">Blockchain Technology</div><br/>
    
    <br/><br/><hr/><br/><br/>
    
    <div class="box">
    <h1 id="qwerty">Z-Index</h1><br/><br/>
    <div id="Ayush4">1</div>
    <div  id="Ayush5">2</div>
    <div  id="Ayush6">3</div>               
</div>
<body>
    
</body>
</html>



#Css code to Apply on Grid box properties of Html code
h1{
   height: 100px;
   width:350px;
   margin:auto;
}

.container{
    height:500px;
    width:650px;
    margin:auto;
    border:2px solid blueviolet;
    border-radius: 10px;
    display:inline-grid;
    grid-template-rows: 100px 100px 100px;
    /*grid-template-columns: 200px 200px 200px;*/
    grid-template-rows: repeat(3,1fr);
   /* grid-template-columns:1fr 1fr 1fr;*/
   row-gap:20px;
   /*column-gap: 20px;*/
   /*justify-items: start;
   justify-items:center;
   align-items: end;*/
   /*place-items: end;*/
}
#ayush1{
    text-align: center;
    height:50px;
    width:200px;
     border:2px solid purple;
    border-radius: 10px;
    background-color: purple;
   /* grid-row-start: 1;
   grid-row-end:3;
   grid-row:1/3; */
   grid-row:1/2;
   /*grid-column-start:1;
   grid-column-end: 4;*/
   /*grid-column:1/3;
   justify-self:end;*/
}

#ayush2{
    text-align: center;
     height:50px;
     width:200px;
      border:2px solid green;
    border-radius: 10px;
    background-color: green;
    /*justify-self:stretch;
    align-self: center;*/
}

#ayush3{
    text-align: center;
     height:50px;
     width:200px;
      border:2px solid red;
    border-radius: 10px;
    background-color: red;
    /*place-self:center;*/
}

#lenovo{
    height:200px;
    width:500px;
    background-color: pink;
    margin:auto;
   /* animation-name:fontanimation;
    animation-duration: 5s;
    animation-timing-function: ease-in;
    animation-delay: 0s;
    animation-iteration-count: 5;
    animation-direction: normal;*/
    animation:fontanimation 5s ease-out 0s 3 reverse;   /*Animation Shorthand!!!*/ 
    animation:widespread 3s ease-in 0s 3 alternate;                                 
   
}

@keyframes fontanimation
{
    from
    {
     color:black;
     font-size: 20px;
    }
    to
    {
      color:blue;
      font-size: 25px;
    }
}

@keyframes widespread
{
    0%{
        color:black;
        text-decoration:none;
    }

    50%{
        color:blueviolet;
        text-decoration:underline;
    }
}

@media(width:560px){
    #rabba{
        color:blue;
        background-color: red;
    }
}
@media(min-width:900px) {
    h1{
        color:white;
        background-color: yellow;

    }
}
@media(max-width:300px){
    h1{
        color:red;
        background-color: blueviolet;
    }
}
@media(min-width:500px) and (max-width:600px){
    h1{
        background-color: crimson;
       
    }
}


@media(orientation:landscape)
{
    .caps{
        background-color:green;
    }
}
/*Z-index*/
.box{
    height:300px ;
    width:300px;
}
h1{
    color:red;
    background-color: aqua;
}
#Ayush4{
    height:200px;
    width:200px;
    background-color: blueviolet;
    border:2px solid purple ;
    margin:auto;
    
}
#Ayush5{
    height:300px;
    width:400px;
    color:white;
    background-color:aquamarine;
    border:2px solid lightblue;
    margin:auto;
   /* position:relative;
    z-index: 1;*/
    

}

#Ayush6{
    height:200px;
    width:200px;
    background-color: orangered;
    border:2px solid orangered;
    margin:auto;

}
