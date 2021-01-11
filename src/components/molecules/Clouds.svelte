<style>
  #clouds {
    padding: 100px 0;
  }

  /*Time to finalise the cloud shape*/
  .cloud {
    width: 200px;
    height: 60px;
    background: lightgray;
    border-radius: 200px;
    -moz-border-radius: 200px;
    -webkit-border-radius: 200px;
    position: absolute;
  }

  .cloud:before,
  .cloud:after {
    content: "";
    position: absolute;
    background: lightgray;
    width: 100px;
    height: 80px;
    position: absolute;
    top: -15px;
    left: 10px;

    border-radius: 100px;
    -moz-border-radius: 100px;
    -webkit-border-radius: 100px;

    -webkit-transform: rotate(30deg);
    transform: rotate(30deg);
    -moz-transform: rotate(30deg);
  }

  .cloud:after {
    width: 120px;
    height: 120px;
    top: -55px;
    left: auto;
    right: 15px;
  }

  /*Time to animate*/
  .x1 {
    left: 725px;
    bottom: -25px;

    -webkit-animation: moveclouds 15s linear infinite;
    -moz-animation: moveclouds 15s linear infinite;
    -o-animation: moveclouds 15s linear infinite;
  }

  /*variable speed, opacity, and position of clouds for realistic effect*/
  .x2 {
    left: 725px;
    bottom: 100px;

    -webkit-transform: scale(0.6);
    -moz-transform: scale(0.6);
    transform: scale(0.6);
    opacity: 0.6; /*opacity proportional to the size*/

    /*Speed will also be proportional to the size and opacity*/
    /*More the speed. Less the time in 's' = seconds*/
    -webkit-animation: moveclouds 25s linear infinite;
    -moz-animation: moveclouds 25s linear infinite;
    -o-animation: moveclouds 25s linear infinite;
  }

  .x3 {
    left: 725px;
    bottom: 150px;

    -webkit-transform: scale(0.8);
    -moz-transform: scale(0.8);
    transform: scale(0.8);
    opacity: 0.8; /*opacity proportional to the size*/

    -webkit-animation: moveclouds 18s linear infinite;
    -moz-animation: moveclouds 18s linear infinite;
    -o-animation: moveclouds 18s linear infinite;
  }

  .x4 {
    left: 725px;
    bottom: 125px;

    -webkit-transform: scale(1.4);
    -moz-transform: scale(1.4);
    transform: scale(1.4);
    opacity: 0.75; /*opacity proportional to the size*/

    -webkit-animation: moveclouds 23s linear infinite;
    -moz-animation: moveclouds 23s linear infinite;
    -o-animation: moveclouds 23s linear infinite;
  }

  .x5 {
    left: 725px;
    bottom: 40px;

    -webkit-transform: scale(1.2);
    -moz-transform: scale(1.2);
    transform: scale(1.2);
    opacity: 0.8; /*opacity proportional to the size*/

    -webkit-animation: moveclouds 20s linear infinite;
    -moz-animation: moveclouds 20s linear infinite;
    -o-animation: moveclouds 20s linear infinite;
  }

  .x6 {
    left: 725px;
    bottom: 75px;

    -webkit-transform: scale(1.1);
    -moz-transform: scale(1.1);
    transform: scale(1.1);
    opacity: 0.8; /*opacity proportional to the size*/

    -webkit-animation: moveclouds 28s linear infinite;
    -moz-animation: moveclouds 28s linear infinite;
    -o-animation: moveclouds 28s linear infinite;
  }

  .x7 {
    left: 725px;
    bottom: 250px;

    -webkit-transform: scale(1.4);
    -moz-transform: scale(1.4);
    transform: scale(1.4);
    opacity: 0.63; /*opacity proportional to the size*/

    -webkit-animation: moveclouds 21s linear infinite;
    -moz-animation: moveclouds 21s linear infinite;
    -o-animation: moveclouds 21s linear infinite;
  }

  .x8 {
    left: 725px;
    bottom: 200px;

    -webkit-transform: scale(1.2);
    -moz-transform: scale(1.2);
    transform: scale(1.2);
    opacity: 0.75; /*opacity proportional to the size*/

    -webkit-animation: moveclouds 28s linear infinite;
    -moz-animation: moveclouds 28s linear infinite;
    -o-animation: moveclouds 28s linear infinite;
  }

  .x9 {
    left: 725px;
    bottom: 225px;

    -webkit-transform: scale(1.1);
    -moz-transform: scale(1.1);
    transform: scale(1.1);
    opacity: 0.95; /*opacity proportional to the size*/

    -webkit-animation: moveclouds 42s linear infinite;
    -moz-animation: moveclouds 42s linear infinite;
    -o-animation: moveclouds 42s linear infinite;
  }

  .x10 {
    left: 725px;
    bottom: 175px;

    -webkit-transform: scale(1.3);
    -moz-transform: scale(1.3);
    transform: scale(1.3);
    opacity: 0.4; /*opacity proportional to the size*/

    -webkit-animation: moveclouds 36s linear infinite;
    -moz-animation: moveclouds 36s linear infinite;
    -o-animation: moveclouds 36s linear infinite;
  }

  .x11 {
    left: 725px;
    bottom: 70px;

    -webkit-transform: scale(1.3);
    -moz-transform: scale(1.3);
    transform: scale(1.3);
    opacity: 0.8; /*opacity proportional to the size*/

    -webkit-animation: moveclouds 22s linear infinite;
    -moz-animation: moveclouds 22s linear infinite;
    -o-animation: moveclouds 22s linear infinite;
  }

  .x12 {
    left: 725px;
    bottom: 275px;

    -webkit-transform: scale(1.6);
    -moz-transform: scale(1.6);
    transform: scale(1.6);
    opacity: 0.75; /*opacity proportional to the size*/

    -webkit-animation: moveclouds 40s linear infinite;
    -moz-animation: moveclouds 40s linear infinite;
    -o-animation: moveclouds 40s linear infinite;
  }

  .x13 {
    left: 725px;
    bottom: 20px;

    -webkit-transform: scale(1.2);
    -moz-transform: scale(1.2);
    transform: scale(1.2);
    opacity: 0.6; /*opacity proportional to the size*/

    /*Speed will also be proportional to the size and opacity*/
    /*More the speed. Less the time in 's' = seconds*/
    -webkit-animation: moveclouds 42s linear infinite;
    -moz-animation: moveclouds 42s linear infinite;
    -o-animation: moveclouds 42s linear infinite;
  }

  @-webkit-keyframes moveclouds {
    0% {
      margin-left: 1000px;
    }
    100% {
      margin-left: -1000px;
    }
  }
  @-moz-keyframes moveclouds {
    0% {
      margin-left: 1000px;
    }
    100% {
      margin-left: -1000px;
    }
  }
  @-o-keyframes moveclouds {
    0% {
      margin-left: 1000px;
    }
    100% {
      margin-left: -1000px;
    }
  }
</style>

<div id="clouds">
  <div class="cloud x1" />
  <div class="cloud x2" />
  <div class="cloud x3" />
  <div class="cloud x4" />
  <div class="cloud x5" />
  <div class="cloud x6" />
  <div class="cloud x7" />
  <div class="cloud x8" />
  <div class="cloud x9" />
  <div class="cloud x10" />
  <div class="cloud x11" />
  <div class="cloud x12" />
  <div class="cloud x13" />
</div>
