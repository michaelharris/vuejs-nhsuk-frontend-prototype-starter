<template>
  <div class="home">

    <div class="nhsuk-grid-row">

    <div class="nhsuk-grid-column-two-thirds">

      <h1>
        nhsuk-frontend library in a VueJS project for prototyping
      </h1>

      <p class="nhsuk-lede-text">
        Visit the 
          <a href="https://service-manual.nhs.uk">NHS digital service manual</a> 
        for guidance and examples.
      </p>

      <img alt="Vue logo" src="../assets/logo.png">

    </div>  

  </div>


    

  </div>
</template>


<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld,
  }
}
</script>
