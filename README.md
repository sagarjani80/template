# templa<!DOCTYPE html>
<html lang="en-US">
    <head>
        <title>template</title>
   <meta name="viewport" content="width=device-width,initial-scale=1.0">
   <style>
       * {
  box-sizing: border-box;
}
       header
       {
           background-color: black;
          color: white;
           font-size: 35px;
           padding: 35px;
           text-align: center;     
       }
       .left{
           background-color: lightgray;
           float: left; 
           width: 20%;
           height: 300px;
           padding: 20px;     
       }
       .left ul{
           font-size: 200%;
           list-style-type: none;
           padding: 0; 
       }
       .left li{
           background-color: green;
           margin: 20px;
           border: 4px solid black;
           border-radius: 20px;
           text-align: center;  
         }
       nav li:hover
      {
          font-size: 40px;
          background-color: brown;
   text-decoration: underline;  
      }
       .main
       {
           padding: 5px;
           float: left;
           width: 80%;
       height: 300px;
       text-align: center;
       background-color:gainsboro;
       overflow-y: scroll;
       }
       .main h1{
           font-size: 50px;
           text-decoration: underline;
           text-shadow: 8px 8px 4px red;  
       }
       .main p{
           font-size: 25px;
           text-align: justify;
         word-spacing: 4px;
       }
       section::after {
  content: "";
  display: table;
  clear: both;
       }
       footer
       {
           background-color: limegreen;
           text-align: center;
           font-size: 20px;
           color: black;
           padding: 10px;
       }
       @media screen and (max-width:650px){
           .left,.main,.right
           {
               width: 100%;
           }
       }
   </style>
    </head>
    <body>
        <h2>CSS Layout Float</h2>
<p>In this example, we have created a header, two columns/boxes and a footer. On smaller screens, the columns will stack on top of each other.</p>
<p>Resize the browser window to see the responsive effect (you will learn more about this in our next chapter - HTML Responsive.)</p>
<header><h1>Cities</h1></header>
<section>
    <nav class="left">
        <ul>
            <li><a href="#london"target="sagar"onclick="london()"style="color:white;text-decoration:none;">London</a></li>
            <li><a href="#paris"target="sagar"onclick="paris()"style="color:white;text-decoration:none;">Paris</a></li>
            <li><a href="#tokyo"target="sagar"onclick="tokyo()"style="color:white;text-decoration:none;">Tokyo</a></li>
        </ul>
    </nav>
    <div class="main"name="sagar">
    <div id="london">
        <h1>London</h1>
        <p>London is the capital city of England. It is the most populous city in the  United Kingdom, with a metropolitan area of over 13 million inhabitants.</p>
        <p>Standing on the River Thames, London has been a major settlement for two millennia, its history going back to its founding by the Romans, who named it Londinium.</p>
        <p>London is one of the world's most important global cities.It exerts considerable influence upon the arts, commerce, education, entertainment, fashion, finance, healthcare, media, professional services, research and development, tourism and transportation.It is one of the largest financial centres in the world and in 2019, London had the second highest number of ultra high-net-worth individuals in Europe, after Paris.And in 2020, London had the second-highest number of billionaires of any city in Europe, after Moscow.London's universities form the largest concentration of higher education institutes in Europe,and London is home to highly ranked institutions such as Imperial College London in natural and applied sciences, the London School of Economics in social sciences, as well as the comprehensive University College London.In 2012,London became the first city to have hosted three modern Summer Olympic Games.</p>
    </div> 
     <div id="paris"style="display:none;">
        <h1>Paris</h1>
        <p>paris is the capital city of England. It is the most populous city in the  United Kingdom, with a metropolitan area of over 13 million inhabitants.</p>
        <p>Standing on the River Thames, London has been a major settlement for two millennia, its history going back to its founding by the Romans, who named it Londinium.</p>    
    </div>
    <div id="tokyo"style="display:none">
        <h1>Tokyo</h1>
        <p>tokyo is the capital city of England. It is the most populous city in the  United Kingdom, with a metropolitan area of over 13 million inhabitants.</p>
        <p>Standing on the River Thames, London has been a major settlement for two millennia, its history going back to its founding by the Romans, who named it Londinium.</p>
    </div>
    </div>
   <script>
function london()
{
    document.getElementById("london").style.display="inline";
    document.getElementById("paris").style.display="none";
    document.getElementById("tokyo").style.display="none";
}
function paris()
{
    document.getElementById("london").style.display="none";
    document.getElementById("paris").style.display="inline";
    document.getElementById("tokyo").style.display="none";
}
function tokyo()
{
    document.getElementById("london").style.display="none";
    document.getElementById("paris").style.display="none";
    document.getElementById("tokyo").style.display="inline";
}
   </script> 
</section>
<footer>
    <h1>Footer</h1>
</footer>
    </body>
</html>te
