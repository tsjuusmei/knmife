<style type="text/scss">

  .wrapper {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    width: 100%;
    height: 100%;
    margin: 0 auto;
    z-index: 99;

    & > div {
      position: absolute;

      &:nth-child(1) {
        left: 0;
        top: 12rem;
      }

      &:nth-child(2) {
        right: 0;
        bottom: 12rem;
      }
    }
  }

  .m1 {
    width: 140px;
  }

  .m2 {
    width: 120px;
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

<div class="container wrapper">
  <div class="circleMotion1">
    <img class="moving m1" src="../images/shape-molecule.svg" alt="" />
  </div>

  <div class="circleMotion2">
    <img class="moving120 m2" src="../images/shape-molecule.svg" alt="" />
  </div>
</div>
