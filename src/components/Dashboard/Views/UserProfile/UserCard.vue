<template>
  <div class="card card-user">
    <div class="image">
      <img src="static/img/background.jpg" alt="...">
    </div>
    <div class="content">
      <div class="author">
        <img class="avatar border-blue" src="static\img\liza.jpg" alt="...">
        <h4 class="title">Nadine Adel
          <br>

        </h4>
      </div>
      <p class="description text-center">
        "I like the way you work it
        <br> SE style
        <br> I love music"
      </p>
    </div>
    <hr>

  </div>
</template>
<script>
  export default {
    data () {
      return {
        details: [
          {
            title: '12',
            subTitle: 'Files'
          },
          {
            title: '2GB',
            subTitle: 'Used'
          },
          {
            title: '24,6$',
            subTitle: 'Spent'
          }
        ]
      }
    },
    methods: {
      getClasses (index) {
        var remainder = index % 3
        if (remainder === 0) {
          return 'col-md-3 col-md-offset-1'
        } else if (remainder === 2) {
          return 'col-md-4'
        } else {
          return 'col-md-3'
        }
      }
    }
  }

</script>
<style>

</style>
