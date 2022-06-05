<template>
  <div class="w-100">
    <header>
      <b-navbar toggleable="lg" type="dark" variant="dark">
        <b-navbar-brand href="#">
          <img src="../static/nasa-logo.png" style="width: 50px; height: 50px">
        </b-navbar-brand>
        <b-navbar-nav class="ml-auto">
          <b-nav-item>See the Galaxies</b-nav-item>
        </b-navbar-nav>
        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav>
            <b-nav-item href="#missoes">Missões</b-nav-item>
            <b-nav-item href="#naves">Naves</b-nav-item>
            <b-nav-item href="#trabalhos">Trabalhos</b-nav-item>
          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
    </header>

    <section class="container py-3">
      <SliderNasa />
      <main class="my-3">
        <p class="text-title text-center">Sobre a NASA</h1>
        <p class="lead">A Nasa é uma agência independente do governo dos Estados Unidos, responsável pela pesquisa e pelo desenvolvimento de tecnologias relacionadas à exploração espacial e ao estudo do universo</p>
      </main>
    </section>

    <MissoesNasa />
    <NavesNasa />
    <TrabalhosNasa />

    <footer class="text-center lead">
      Made with love by Well
    </footer>

  </div>
</template>

<script>
import SliderNasa from '~/components/SliderNasa.vue'
export default {
  name: 'IndexPage',
  components: { SliderNasa },
}
</script>
