<template>
  <div class="container">
    <div>
      <Logo />
      <Nav />
      <Header title="Netlify Plugin: Algolia Index" />
      <section>
        <main>
          <p>
            <strong
              >Automatically generate an Algolia friendly index file!</strong
            >
            Using this plugin, you can build a search index file containing of
            all your content pages automatically, excluding any pages you don't
            want to index.
          </p>
        </main>
        <footer>
          <nuxt-link to="/" class="button button--green">
            Home
          </nuxt-link>
          <a
            href="https://github.com/nuxt/nuxt.js"
            target="_blank"
            class="button button--grey"
          >
            GitHub
          </a>
        </footer>
      </section>
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import Nav from '~/components/Nav.vue'
import Header from '~/components/Header.vue'

export default {
  components: {
    Logo,
    Nav,
    Header
  },

  head() {
    return {
      title: 'Netlify Plugin: Algolia Export',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Export your search index straight to Algolia'
        }
      ]
    }
  }
}
</script>
