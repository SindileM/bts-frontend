<template>
  <section>
    <button
      type="button"
      class="button btn-primary"
      data-bs-toggle="modal"
      data-bs-target="#addDriverModal"
    >
     Create blog
    </button>
    <div class="carousel-inner">
      <div class="carousel-item active">
        <div class="row mb-2 bg-light" v-for="driver in drivers" :key="driver">
          <button
            type="button"
            class="button btn-primary"
             data-bs-toggle="modal"
             data-bs-target="#editDriverModal"
          >
            Update blog
          </button>
   <button
            type="button"
            class="button btn-primary"
          >
            Delete blog
          </button>
          <div class="col-lg-6">
            <img :src="driver.avatar" class="d-block w-100" alt="..." />
          </div>
          <div class="col-lg-6">
            <div class="d-flex flex-column justify-content-center my-5 px-3">
              <p class="review text-center">{{ driver.name }}</p>
              <div
                class="name d-flex align-items-center justify-content-center"
              >
                <span class="fas fa-minus pe-1"></span>
                <p class="m-0">{{ driver.content }}</p>
                <p>{{ driver.number }}</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

 

</template>

<script>
export default {
// name: "Drivers",
// data() {
//   return { 
//     drivers: [],
//   };
computed: {
  drivers(){
    return this.$store.state.drivers;
  }
},
mounted() {  
  // DISPATCH runs an ACTION
  this.$store.dispatch('getDrivers')
},
};
// };
</script>

<style>

</style>