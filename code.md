<!DOCTYPE html>
<html>
   <head>
    <meta name="viewport" content="width=device-width, initial-scale=1">
   </head>
    <body bgcolor="blue">
        <h3> Arm control panel</h3>
        <form name="formArm" method="post" action="index.php">     
<div>
    <span id="v1"></span>
    <input type="range" id="mot1" name="Foward" min="0" max="200">
    <label for="volume1">  Forward  </label>
    
</div>
<br><br>
<div>

    <span id="v2"></span>
    <input type="range" id="mot2" name="Back" min="0" max="200">
    <label for="volume2">  Back  </label>
    
</div>
<br><br>
<div>
    <span id="v3"></span>
    <input type="range" id="mot3" name="Right" min="0" max="200">
    <label for="volume3">  Right  </label>
    
</div>
<br><br>
<div>
    <span id="v4"></span>
    <input type="range" id="mot4" name="Left" min="0" max="200">
    <label for="volume4">   Left   </label>
    
</div>
<br><br>


<input type="submit" name="save" id="submit" value="save">
</form>

<form name="formArm" method="post" action="phpTest.php">
<input type="submit" name="run" id="Run" value="run">
</form>

<script>
    var slider1 = document.getElementById("mot1");
var output1 = document.getElementById("v1");
output1.innerHTML = slider1.value;

slider1.oninput = function() {
  output1.innerHTML = this.value;
}
var slider2 = document.getElementById("mot2");
var output2 = document.getElementById("v2");
output2.innerHTML = slider2.value;

slider2.oninput = function() {
  output2.innerHTML = this.value;
}

var slider3 = document.getElementById("mot3");
var output3 = document.getElementById("v3");
output3.innerHTML = slider3.value;

slider3.oninput = function() {
  output3.innerHTML = this.value;
}


var slider4 = document.getElementById("mot4");
var output4 = document.getElementById("v4");
output4.innerHTML = slider4.value;

slider4.oninput = function() {
  output4.innerHTML = this.value;
}
var slider5 = document.getElementById("mot5");
var output5 = document.getElementById("v5");
output5.innerHTML = slider5.value;

slider5.oninput = function() {
  output5.innerHTML = this.value;
}
var slider6 = document.getElementById("mot6");
var output6 = document.getElementById("v6");
output6.innerHTML = slider6.value;

slider6.oninput = function() {
  output6.innerHTML = this.value;
}

</script>
<script>
  window.watsonAssistantChatOptions = {
      integrationID: "f73c1616-bcc7-470e-87b0-be86d99aef06", 
            region: "eu-gb", 
      serviceInstanceID: "1ab137d0-7068-4b3c-8860-e6577e6e8a73"
      onLoad: function(instance) { instance.render(); }
    };
  setTimeout(function(){
    const t=document.createElement('script');
    t.src="https://web-chat.global.assistant.watson.appdomain.cloud/loadWatsonAssistantChat.js";
    document.head.appendChild(t);
  });
</script>

    </body>
</html>
