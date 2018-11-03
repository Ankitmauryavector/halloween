<!DOCTYPE html>
<html>
    <head>
        <title>Page Title</title>
        <meta name="viewport" content="width=device-width,initial-scale=1">
       
    </head>
    <body>
     <div id="enter">
          <p>Beware!!! this girl is Creepy.<br><br> Her name is Sally, nicknamed Evil Sally as she used to create trouble for people around her. She died 10 years ago in a car accident. It is said that on every Halloween night she wakes up from her grave searching for a prey to play with her. <br><br> Oh! Someone's knocking your door. Be careful it could be Evil Sally.</p>
          <button id="okBtn">Ok</button>
        </div>
          <div class="rain anime"></div>
         <div class="lightning anime">
           <img class="skull" src="https://raw.githubusercontent.com/prathu9/prathu9.github.io/master/js/halloween/skull.png"> 
          <img class="nany" src="https://i.pinimg.com/originals/a6/55/fc/a655fc3ea06df8e7715dfc99c1794253.jpg">
       </div> 
       <div class="face anime">
         <div class="eye lefteye anime"><div class="inside_eye anime"></div></div>
         <div class="eye righteye anime"><div class="inside_eye anime"></div></div>
         
         <div class="mouth anime"></div>
       </div>
       <div id="nany">
            
       </div>
       
       <div class="text anime">Happy <span class="halloween anime">Halloween</span></div>
          
               
       <script>
         let audio = new Audio('https://raw.githubusercontent.com/prathu9/prathu9.github.io/master/js/halloween/twls.mp3');
         let enter=document.getElementById("enter");
         let okBtn=document.getElementById("okBtn");
         let anime=document.getElementsByClassName("anime");

        const playSound=()=>{  
          enter.style.display="none"; 
          for(let i=0;i<anime.length;i++){
            anime[i].style.animationPlayState="running";
          } 
          setTimeout(()=>{anime[0].style.display="block";},9000);  
          audio.play();
          audio.volume=0.8;
        }

        okBtn.addEventListener("click",playSound);
        
       </script>
      
    </body>
</html>
