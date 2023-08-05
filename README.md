# flexboxTrialinHtml
<!--WHAT IS FLEXBOX??   vertically centering a block of content inside its parent.
Making all the children of a container take up an equal amount of the availble width,height,  regardless of how much width/height is available.-->
<!--Terminologies using...
ALSO SEE SS AT VRINDA'S IMP STUFF(WEB)
ALSO CLICK ON INSPECT THAN ON REPONSIVE BUTTON TO CLEARLY INSPECT THIS PAGE.-->

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flexbox</title>
    <style>
        body{
            font-family: Arial, Helvetica, sans-serif;
            font-size: 20px;
            padding: 0 20px 30px 0;
            line-height: 1.4;

        }
        .flex-container{
            display:flex; /*  or you can use block */
            flex-direction: row;/*boxes row m rakhni h ya column m, ye decide krta...*/
            flex-wrap: wrap;  /*(box sift hoke align hone lagenge ,when you compress window)you can use nowrap so that when you small the window they dont get compress with it */
          align-content: center; /*you can also use align-items here, and center ki jagah you can write flex-end or flex-start, or stretch too or apace-around or space-between*/
          
        }

        .flex-item{
            width: 75px;
            height: 75px;
            background-color: aquamarine;
            border: 2px solid darkblue;
            text-align:center;
            font-size: 2em;
            color:white;
            font-weight: bold;
            line-height: 1.4;
            flex-flow: column wrap;/*you can hover over it know what sequence and u are writing*/

        }

        #flex-item-1{
            background-color: lightpink;
            flex-basis:200px;/*this property helps to stretch the box size, u can see*/
            flex-grow:2;/*ye kya krega ki ab jese hi reponsiveness badhaenge, means window size, toh iski stretching speed 2times jyada tezi se badhegi*/

        }

        #flex-item-2{
            background-color: lightskyblue;
            order:3;
            flex-shrink:3;/*iske liye flex wrap hatadena..(  jaldi shrink hota)*/
            
            /*
            you can also change the order of dabba by using order property*/
        }

        
        #flex-item-3{
            background-color: lightgreen ;
            align-self:flex-end;/*you can do flex start or flex end or stretch*/
        } 


        #flex-item-4{
            flex: 3 2 250px;/*you can hover over it to know what order is this*/
            background-color: rgb(229, 23, 95);
        }
    </style>
</head>
<body>
    <div class="flex-container">
        <div class="flex-item" id="flex-item-1">1</div>
        <div class="flex-item" id="flex-item-2">2</div>
        <div class="flex-item" id="flex-item-3">3</div>
        <div class="flex-item" id="flex-item-4">4</div>
        <div class="flex-item" id="flex-item-5">5</div>
    </div>
</body>
</html>
