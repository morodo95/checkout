<template>
  <div class="container">
    <div class="notificacion">
      <b-carousel>
        <b-carousel-item v-for="(carousel, i) in carousels" :key="i">
            <section :class="`hero is-medium is-${carousel.color}`">
                <div class="hero-body has-text-centered">
                    <h1 class="title">{{carousel.text}}</h1>
                </div>
            </section>
        </b-carousel-item>           
    </b-carousel>
    <b-field label="Select a date">
        <b-datepicker
            placeholder="Click to select..."
            v-model="dates"
            inline
            :min-date="minDate"
            :max-date="maxDate"
            range>
        </b-datepicker>
    </b-field>

    
    </div>
  </div>
</template>
<script>
export default {
    data(){
        const today = new Date()
        return {
           dates: [],
           minDate: new Date(today.getFullYear(), today.getMonth(), today.getDate()),
           maxDate: new Date(today.getFullYear(), today.getMonth(), today.getDate() + 356),
            carousels: [
                { text: 'Slide 1', color: 'primary' },
                { text: 'Slide 2', color: 'info' },
                { text: 'Slide 3', color: 'success' },
                { text: 'Slide 4', color: 'warning' },
                { text: 'Slide 5', color: 'danger' }
            ]
        }
    },
    mounted() {
            console.log(process.env);
    },
   
}
</script>
<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
