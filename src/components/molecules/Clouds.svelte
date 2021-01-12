<style>
  div {
    --cloud-base-duration: 60s;
    --cloud-1: var(--cloud-base-duration);
    --cloud-2: calc(var(--cloud-base-duration) * .95);
    --cloud-3: calc(var(--cloud-base-duration) * .9);
    --cloud-4: calc(var(--cloud-base-duration) * .85);
    --cloud-5: calc(var(--cloud-base-duration) * .8);
    --cloud-6: calc(var(--cloud-base-duration) * .75);
    --cloud-7: calc(var(--cloud-base-duration) * .7);
    --cloud-8: calc(var(--cloud-base-duration) * .65);
    --cloud-9: calc(var(--cloud-base-duration) * .6);
    --cloud-10: calc(var(--cloud-base-duration) * .55);
    --cloud-11: calc(var(--cloud-base-duration) * .5);
    --cloud-12: calc(var(--cloud-base-duration) * .45);
    --cloud-13: calc(var(--cloud-base-duration) * .4);


    position: relative;
    bottom: 220px;
    z-index: 1200;
  }
  /*Time to finalise the cloud shape*/
  .cloud {
    width: 200px;
    height: 60px;
    background: var(--cloud);
    border-radius: 200px;
    -moz-border-radius: 200px;
    -webkit-border-radius: 200px;
    position: absolute;
  }

  .cloud:before,
  .cloud:after {
    content: '';
    position: absolute;
    background: var(--cloud);
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
    /* left: 0; */
    left: 0;
    bottom: -25px;

    -webkit-animation: moveclouds var(--cloud-1) linear infinite;
    /* -moz-animation: moveclouds 15s linear infinite; */
    /* -o-animation: moveclouds 15s linear infinite; */
  }

  /*variable speed, opacity, and position of clouds for realistic effect*/
  .x2 {
    left: 0;
    bottom: 100px;

    -webkit-transform: scale(0.6);
    -moz-transform: scale(0.6);
    transform: scale(0.6);
    opacity: 0.6; /*opacity proportional to the size*/

    /*Speed will also be proportional to the size and opacity*/
    /*More the speed. Less the time in 's' = seconds*/
    -webkit-animation: moveclouds var(--cloud-2) linear infinite;
    /* -moz-animation: moveclouds 25s linear infinite; */
    /* -o-animation: moveclouds 25s linear infinite; */
  }

  .x3 {
    left: 0;
    bottom: 150px;

    -webkit-transform: scale(0.8);
    -moz-transform: scale(0.8);
    transform: scale(0.8);
    opacity: 0.8; /*opacity proportional to the size*/

    -webkit-animation: moveclouds var(--cloud-3) linear infinite;
    /* -moz-animation: moveclouds 18s linear infinite; */
    /* -o-animation: moveclouds 18s linear infinite; */
  }

  .x4 {
    left: 0;
    bottom: 125px;

    -webkit-transform: scale(1.4);
    -moz-transform: scale(1.4);
    transform: scale(1.4);
    opacity: 0.75; /*opacity proportional to the size*/

    -webkit-animation: moveclouds var(--cloud-4) linear infinite;
    /* -moz-animation: moveclouds 23s linear infinite; */
    /* -o-animation: moveclouds 23s linear infinite; */
  }

  .x5 {
    left: 0;
    bottom: 40px;

    -webkit-transform: scale(1.2);
    -moz-transform: scale(1.2);
    transform: scale(1.2);
    opacity: 0.8; /*opacity proportional to the size*/

    -webkit-animation: moveclouds var(--cloud-5) linear infinite;
    /* -moz-animation: moveclouds 20s linear infinite; */
    /* -o-animation: moveclouds 20s linear infinite; */
  }

  .x6 {
    left: 0;
    bottom: 75px;

    -webkit-transform: scale(1.1);
    -moz-transform: scale(1.1);
    transform: scale(1.1);
    opacity: 0.8; /*opacity proportional to the size*/

    -webkit-animation: moveclouds var(--cloud-6) linear infinite;
    /* -moz-animation: moveclouds 28s linear infinite; */
    /* -o-animation: moveclouds 28s linear infinite; */
  }

  .x7 {
    left: 0;
    bottom: 250px;

    -webkit-transform: scale(1.4);
    -moz-transform: scale(1.4);
    transform: scale(1.4);
    opacity: 0.63; /*opacity proportional to the size*/

    -webkit-animation: moveclouds var(--cloud-7) linear infinite;
    /* -moz-animation: moveclouds 21s linear infinite; */
    /* -o-animation: moveclouds 21s linear infinite; */
  }

  .x8 {
    left: 0;
    bottom: 200px;

    -webkit-transform: scale(1.2);
    -moz-transform: scale(1.2);
    transform: scale(1.2);
    opacity: 0.75; /*opacity proportional to the size*/

    -webkit-animation: moveclouds var(--cloud-8) linear infinite;
    /* -moz-animation: moveclouds 28s linear infinite; */
    /* -o-animation: moveclouds 28s linear infinite; */
  }

  .x9 {
    left: 0;
    bottom: 225px;

    -webkit-transform: scale(1.1);
    -moz-transform: scale(1.1);
    transform: scale(1.1);
    opacity: 0.95; /*opacity proportional to the size*/

    -webkit-animation: moveclouds var(--cloud-9) linear infinite;
    /* -moz-animation: moveclouds 42s linear infinite; */
    /* -o-animation: moveclouds 42s linear infinite; */
  }

  .x10 {
    left: 0;
    bottom: 175px;

    -webkit-transform: scale(1.3);
    -moz-transform: scale(1.3);
    transform: scale(1.3);
    opacity: 0.4; /*opacity proportional to the size*/

    -webkit-animation: moveclouds var(--cloud-10) linear infinite;
    /* -moz-animation: moveclouds 36s linear infinite; */
    /* -o-animation: moveclouds 36s linear infinite; */
  }

  .x11 {
    left: 0;
    bottom: 70px;

    -webkit-transform: scale(1.3);
    -moz-transform: scale(1.3);
    transform: scale(1.3);
    opacity: 0.8; /*opacity proportional to the size*/

    -webkit-animation: moveclouds var(--cloud-11) linear infinite;
    /* -moz-animation: moveclouds 22s linear infinite; */
    /* -o-animation: moveclouds 22s linear infinite; */
  }

  .x12 {
    left: 0;
    bottom: 275px;

    -webkit-transform: scale(1.6);
    -moz-transform: scale(1.6);
    transform: scale(1.6);
    opacity: 0.75; /*opacity proportional to the size*/

    -webkit-animation: moveclouds var(--cloud-12) linear infinite;
    /* -moz-animation: moveclouds 40s linear infinite; */
    /* -o-animation: moveclouds 40s linear infinite; */
  }

  .x13 {
    left: 0;
    bottom: 20px;

    -webkit-transform: scale(1.2);
    -moz-transform: scale(1.2);
    transform: scale(1.2);
    opacity: 0.6; /*opacity proportional to the size*/

    /*Speed will also be proportional to the size and opacity*/
    /*More the speed. Less the time in 's' = seconds*/
    -webkit-animation: moveclouds var(--cloud-13) linear infinite;
    /* -moz-animation: moveclouds 42s linear infinite; */
    /* -o-animation: moveclouds 42s linear infinite; */
  }

  @-webkit-keyframes moveclouds {
    0% {
      margin-left: 100vw;
      /* margin-left: 1000px; */
    }
    100% {
      margin-left: -200px;
      /* margin-left: -1000px; */
    }
  }
  /* @-moz-keyframes moveclouds {
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
  } */
</style>

<div>
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
