<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the documentation</p>
<div class="parent">
  <div class="child">Child 1</div>
  <div class="child">Child 2</div>
</div>

<style lang="scss">
  @mixin clearfix() {
    &:before,
    &:after {
      content: '';
      display: table;
    }
    &:after {
      clear: both;
    }
  }
  .parent {
    @include clearfix();

    .child {
      float: left;
      width: 50%;
      box-sizing: border-box;
      padding: 10px;
      background-color: #f0f0f0;
      border: 1px solid #ccc;
    }
  }
</style>
