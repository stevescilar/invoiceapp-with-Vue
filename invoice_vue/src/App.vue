<template>
  <div id="wrapper">
    <nav class="navbar is-dark">
      <div class="navbar-brand">
        <router-link to="/" class="navbar-item"><strong>MyInvoice</strong></router-link>
      </div>
    </nav>
  </div>
  <router-view/>
</template>

<style lang="scss">
@import '../node_modules/bulma';
</style>
