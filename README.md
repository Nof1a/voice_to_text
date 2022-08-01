# voice_to_text
IOT-week-2-tasks-
Task 1: developing an Arabic voice recognition for Chrome browser

I Stady from Youtup channle

First::  Download Visual Studio Code program

2. Developing the voice recognition:

this task contain(( three main parts)):

The index.html code:
------------------------------------------
```ruby
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8">
        <meta name="viewport" content="initial-scale=1.0, maximum-scale=1.0, user-scalable=1"›
        <title>Home</title>
         <link rel="stylesheet" type="text/css" href="css/style.css"› 
          </head> 
           <body> 
             <div class="voice_to_text"›
         <h1> Voice To Text Converter </h1> 
              <textarea id="convert_to_text"></textarea>
              <button id="click_to_convert">voice to text</button>
             </div> 
               <script type="text/javascript" src="js/script.js"></script>
               </body> 
               </html>
                ```
---------------------------------------------------------


style.css:
```ruby
*,*:after,*:before{
-webkit-box-sizing: border-box;
-moz-box-sizing: border-box;
-ms-box-sizing: border-box;
box-sizing: border-box;


}
body{

font-family: Arial, Helvetica, sans-serif;
font-size: 16px;
margin: 0;
background:linear-gradient(to right bottom,#d13cff,#031f6a);
color: #000;
display: flex;
align-items: center;
justify-content: center;
min-height: 100vh;
}
.voice_to_text{
    width: 600px;
    text-align: center;
}
```
------------------------------------------------

script.js
```ruby
click_to_convert.addEventListener('click',function(){ 
var speech = true ;
window.SpeechRecognition = window.webkitSpeechRecognition;
const recognition = new SpeechRecognition();
recognition.interimResults = true ;

recognition.addEventListener('result', e=>{
    const transcript = Array.from(e.results)
    .map(resuLt => result[0])
    .map(resuLt => result.transcript)
    convert_to_text.innerHTML= transcript
})
    if(speech == true){
        recognition.start();
    }
})


```

Then I saved it to a folder and ran it



