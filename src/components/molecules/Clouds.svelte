<div>
  <span />
  <span />
  <span />
  <span />
  <span />
  <span />
  <span />
  <span />
  <span />
  <span />
  <span />
  <span />
</div>

<style type="text/scss">
  div {
    --cloud-base-duration: 60s;
    --cloud-1: var(--cloud-base-duration);
    --cloud-2: calc(var(--cloud-base-duration) * 0.95);
    --cloud-3: calc(var(--cloud-base-duration) * 0.9);
    --cloud-4: calc(var(--cloud-base-duration) * 0.85);
    --cloud-5: calc(var(--cloud-base-duration) * 0.8);
    --cloud-6: calc(var(--cloud-base-duration) * 0.75);
    --cloud-7: calc(var(--cloud-base-duration) * 0.7);
    --cloud-8: calc(var(--cloud-base-duration) * 0.65);
    --cloud-9: calc(var(--cloud-base-duration) * 0.6);
    --cloud-10: calc(var(--cloud-base-duration) * 0.55);
    --cloud-11: calc(var(--cloud-base-duration) * 0.5);
    --cloud-12: calc(var(--cloud-base-duration) * 0.45);

    position: absolute;
    bottom: 200px;
    width: 100%;

    & > span {
      width: 200px;
      height: 60px;
      left: 0;
      bottom: 220px;
      z-index: 999;
      background: #fff;
      border-radius: 200px;
      position: absolute;

      &::before,
      &::after {
        content: '';
        position: absolute;
        background: #fff;
        border-radius: 100px;
        transform: rotate(30deg);
      }

      &::before {
        width: 100px;
        height: 80px;
        top: -15px;
        left: 10px;
      }

      &::after {
        width: 120px;
        height: 120px;
        top: -55px;
        left: auto;
        right: 15px;
      }

      &:nth-child(1) {
        bottom: -25px;
        animation: moveclouds var(--cloud-1) linear infinite;
      }
      &:nth-child(2) {
        bottom: 100px;
        transform: scale(0.6);
        opacity: 0.6;
        animation: moveclouds var(--cloud-2) linear infinite;
      }

      &:nth-child(3) {
        bottom: 150px;
        transform: scale(0.8);
        opacity: 0.8;
        animation: moveclouds var(--cloud-3) linear infinite;
      }

      &:nth-child(4) {
        bottom: 125px;
        transform: scale(1.4);
        opacity: 0.75;
        animation: moveclouds var(--cloud-4) linear infinite;
      }

      &:nth-child(5) {
        bottom: 40px;
        transform: scale(1.2);
        opacity: 0.8;
        animation: moveclouds var(--cloud-5) linear infinite;
      }

      &:nth-child(6) {
        bottom: 75px;
        transform: scale(1.1);
        opacity: 0.8;
        animation: moveclouds var(--cloud-6) linear infinite;
      }

      &:nth-child(7) {
        bottom: 250px;
        transform: scale(1.4);
        opacity: 0.63;
        animation: moveclouds var(--cloud-7) linear infinite;
      }

      &:nth-child(8) {
        bottom: 200px;
        transform: scale(1.2);
        opacity: 0.75;
        animation: moveclouds var(--cloud-8) linear infinite;
      }

      &:nth-child(9) {
        bottom: 225px;
        transform: scale(1.1);
        opacity: 0.95;
        animation: moveclouds var(--cloud-9) linear infinite;
      }

      &:nth-child(10) {
        bottom: 175px;

        transform: scale(1.3);
        opacity: 0.4;
        animation: moveclouds var(--cloud-10) linear infinite;
      }

      &:nth-child(11) {
        bottom: 70px;
        transform: scale(1.3);
        opacity: 0.8;
        animation: moveclouds var(--cloud-11) linear infinite;
      }

      &:nth-child(12) {
        bottom: 275px;
        transform: scale(1.6);
        opacity: 0.75;
        animation: moveclouds var(--cloud-12) linear infinite;
      }
    }
  }

  @keyframes moveclouds {
    0% {
      margin-left: 100vw;
    }
    100% {
      margin-left: -200px;
    }
  }
</style>
