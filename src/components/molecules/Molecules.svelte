<style>
  img {
    position: absolute;
    filter: drop-shadow(20px 8px 20px grey);
  }

  .m1 {
    width: 180px;
    margin-left: 150px;
  }

  .m2 {
    width: 250px;
    right: 18%;
  }

  .m3 {
    width: 150px;
    left: 40%;
    margin-top: 22%;
    opacity: .3;
    z-index: -1000;
  }

  .moving {
    animation: rotation 3s ease-in-out infinite;
    animation-delay: 1s;
  }

  .moving45 {
    animation: rotation45 3s ease-in-out infinite;
  }

  .moving120 {
    animation: rotation120 3s ease-in-out infinite;
    animation-delay: 2s;
  }

  .circleMotion {
    animation: movement 3s linear infinite;
  }

  .circleMotion1 {
    animation: movement 3s linear infinite;
    animation-delay: 1s;
  }

  .circleMotion2 {
    animation: movement 3s linear infinite;
    animation-delay: 1.5s;
  }

  @keyframes movement {
    from {
      transform: rotate(0deg) translateX(10px) rotate(0deg);
    }
    to {
      transform: rotate(360deg) translateX(10px) rotate(-360deg);
    }
  }

  @keyframes rotation {
    0% {
      transform: rotate(13deg);
    }
    50% {
      transform: rotate(17deg);
    }
    75% {
      transform: rotate(8deg);
    }
    100% {
      transform: rotate(13deg);
    }
  }

  @keyframes rotation45 {
    0% {
      transform: rotate(46deg);
    }
    50% {
      transform: rotate(50deg);
    }
    75% {
      transform: rotate(41deg);
    }
    100% {
      transform: rotate(46deg);
    }
  }

  @keyframes rotation120 {
    0% {
      transform: rotate(121deg);
    }
    50% {
      transform: rotate(125deg);
    }
    75% {
      transform: rotate(116deg);
    }
    100% {
      transform: rotate(121deg);
    }
  }
</style>

<div class="circleMotion">
  <img class="moving45 m1" src="../images/molecule.svg" alt="" />
</div>

<div class="circleMotion1">
  <img class="moving m2" src="../images/molecule.svg" alt="" />
</div>

<div class="circleMotion2">
  <img class="moving120 m3" src="../images/molecule.svg" alt="" />
</div>
