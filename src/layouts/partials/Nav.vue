<template>
  <nav class="main-nav flex gap-15">

    <SearchForm class="hide-for-small"  />

    <g-link to="/docs">
      <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="show-for-small feather feather-file-text"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path><polyline points="14 2 14 8 20 8"></polyline><line x1="16" y1="13" x2="8" y2="13"></line><line x1="16" y1="17" x2="8" y2="17"></line><polyline points="10 9 9 9 8 9"></polyline></svg>
      <span>Docs</span>
    </g-link>

    <g-link to="/learn">
      <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="show-for-small feather feather-compass"><circle cx="12" cy="12" r="10"></circle><polygon points="16.24 7.76 14.12 14.12 7.76 16.24 9.88 9.88 16.24 7.76"></polygon></svg>
      <span>Learn</span>
    </g-link>

    <g-link to="/plugins">
      <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="show-for-small feather feather-zap"><polygon points="13 2 3 14 12 14 11 22 21 10 12 10 13 2"></polygon></svg>
      <span>Plugins</span>
    </g-link>

    <g-link to="/blog">
      <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="show-for-small feather feather-edit"><path d="M20 14.66V20a2 2 0 0 1-2 2H4a2 2 0 0 1-2-2V6a2 2 0 0 1 2-2h5.34"></path><polygon points="18 2 22 6 12 16 8 16 8 12 18 2"></polygon></svg>
      <span>Blog</span>
    </g-link>


  </nav>
</template>

<script>
import SearchForm from '~/components/SearchForm.vue'

export default {
  components: {
    SearchForm
  }
}
</script>

<style lang="scss">
  @media screen and (max-width: 750px) {
    .main-nav {
      position: fixed;
      bottom:0;
      left:0;
      right:0;
      background: var(--primary-bg);
      color: var(--secondary-bg);
      margin-right:0!important;
      justify-content: center;
      box-shadow: 0 0 10px 0 rgba(0,0,0,.2);
      min-height: 60px;
      flex-wrap: nowrap!important;
      padding: 5px var(--space);
    }
  }
  @media only screen 
  and (device-width : 375px) 
  and (device-height : 812px) 
  and (-webkit-device-pixel-ratio : 3) {
    .main-nav {
      padding-bottom: var(--space);
    }
  }
</style>
