---
date: 2018-12-20T22:05:09-05:00
draft: false
type: "page"
layout: "single"
---

The United States Government is currently funded through midnight on

<div class="tc b">Sept 30, 2019</div>

<div id="unless">Unless lawmakers pass a continuing resolution, the federal government will shutdown in:</div>

<div id="timer"></div>


<script>
// Set the date we're counting down to
var countDownDate = new Date("Sept 30, 2019 23:59:59").getTime(); 
var d = new Date();
var tzOffset = 300 - d.getTimezoneOffset();

//document.write(tzOffset);
// Update the count down every 1 second
var x = setInterval(function() {

  // Get todays date and time
  var now = new Date().getTime();
    
  // Find the distance between now and the count down date
  var distance = countDownDate - now + (1000 * 60 * tzOffset);
    
  // Time calculations for days, hours, minutes and seconds
  var days = Math.floor(distance / (1000 * 60 * 60 * 24));
  var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
  var seconds = Math.floor((distance % (1000 * 60)) / 1000);
  // Output the result in an element with id="demo"
  document.getElementById("timer").innerHTML = days + "d " + hours + "h "
  + minutes + "m " + seconds + "s ";    
  // If the count down is over, write some text 
  if (distance < 0) {
    clearInterval(x);
    document.getElementById("timer").innerHTML = "NOW";
  }
}, 1000);
</script>

