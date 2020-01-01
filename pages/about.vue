<template>
  <section class="section">
    <div class="hero-body">
      <div class="container">
        <h1 class="title">このサイトについて</h1>
        <p>これはLighthouse CIの動作確認のために作ったサイトであって、特に何の意味もないサイトです。</p>
      </div>
    </div>

    <b-collapse class="card" aria-id="contentIdForA11y3">
      <div
        slot="trigger"
        slot-scope="props"
        class="card-header"
        role="button"
        aria-controls="contentIdForA11y3"
      >
        <p class="card-header-title">意味のないcomponent</p>
        <a class="card-header-icon">
          <b-icon :icon="props.open ? 'menu-down' : 'menu-up'"></b-icon>
        </a>
      </div>
      <div class="card-content">
        <div class="content">特に何の意味もないけど置いてみたcomponent</div>
      </div>
      <footer class="card-footer">
        <a class="card-footer-item">Button1</a>
        <a class="card-footer-item">Button2</a>
        <a class="card-footer-item">Button3</a>
      </footer>
    </b-collapse>
  </section>
</template>

<script>
export default {
  name: "About",

  components: {}
};
</script>
