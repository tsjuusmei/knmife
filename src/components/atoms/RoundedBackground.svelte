<style type="text/scss">

  @mixin roundedBackground() {

    section {
      &::before,
      &::after {
        content: url('../images/shape-rounded.svg');
        margin: -3px 0;
        display: block;
      }

      &::after {
        transform: rotate(180deg);
      }
    }
  }
</style>
