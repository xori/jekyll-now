---
layout: post
title: "Last login: Mon Aug 22 16:14:39 2016 from 10.2.1.12"
---

<code>
Last login: Mon Aug 22 16:14:39 2016
evan@verworn.ca ~ $ uptime
<span uptime></span>
evan@verworn.ca ~ $ <span class="blinking-cursor">|</span>
</code>


<style>
code {
  white-space: pre-wrap;
}

.blinking-cursor {
  font-weight: 100;
  color: #2E3D48;
  -webkit-animation: 1s blink step-end infinite;
  -moz-animation: 1s blink step-end infinite;
  -ms-animation: 1s blink step-end infinite;
  -o-animation: 1s blink step-end infinite;
  animation: 1s blink step-end infinite;
}

@keyframes "blink" {
  from, to {
    color: transparent;
  }
  50% {
    color: black;
  }
}

@-moz-keyframes blink {
  from, to {
    color: transparent;
  }
  50% {
    color: black;
  }
}

@-webkit-keyframes "blink" {
  from, to {
    color: transparent;
  }
  50% {
    color: black;
  }
}

@-ms-keyframes "blink" {
  from, to {
    color: transparent;
  }
  50% {
    color: black;
  }
}

@-o-keyframes "blink" {
  from, to {
    color: transparent;
  }
  50% {
    color: black;
  }
}
</style>

<script src="https://cdnjs.cloudflare.com/ajax/libs/moment.js/2.14.1/moment.min.js"></script>
<script>
  var cmd = document.querySelector('[uptime]');
  var now = moment()
  var then = moment(1471896879000)
  var result = " ";
  
  result += now.format('HH:MM:SS') +
  	" up " + now.diff(then, 'days') + " days, " +
    (now.diff(then, "hours") % 24) + ":" +
    (now.diff(then, "minutes") % 60) + 
    ", u users, load average: 0.04 0.12 0.09"
  
  cmd.innerHTML = result;
</script>
