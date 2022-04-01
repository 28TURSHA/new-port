<template>
  <h1>About Me</h1>
  <div class="container">
    <div class="row justify-content-around">
      <div class="col-6">
        <img src="https://i.postimg.cc/LXBxCDTH/flower.jpg" alt="" />
      </div>
      <div class="col-6">
        <h3>A bit about me!</h3>
        <p>
          I am a an aspiring frontend web developer, who loves trying new things
          and exploring all the things the world has to offer. I decided on
          coding because web development is so facinating and an ever changing
          industry. The design aspect of an application really sparks my
          interests and is definitely something I would like to dabble in.
        </p>

        <div class="item">
          <span>Name:</span>
          
          <h5>Tursha Arendse</h5>
        </div>

        <div class="item">
          <span>D.O.B:</span>
          
          <h5>28/10/2002</h5>
        </div>

        <div class="item">
          <span>Email Address:</span>
          
          <h5>turshaarendse@gmail.com</h5>
        </div>

        <div class="item">
          <span>Contact Number:</span>
          
          <h5>+(27) 67 668 5517</h5>
        </div>

        <div class="item">
          <span>Location:</span>
          
          <h5>Cape Town, South Africa</h5>
        </div>
        <!-- <p><span>D.O.B :</span> 28/10/2002</p>
        <p><span>Email Address :</span> turshaarendse@gmail.com</p>
        <p><span>Contact Number :</span> +(27) 67 668 5517</p>
        <p><span>Current Location :</span> Cape Town, South Africa</p> -->
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>
<style scoped>
h1 {
  padding-top: 150px;
}
span {
  color: #05a8df;
}
.item {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-direction: row;
  width: 30%;
}
.col-6 {
  display: flex;
  justify-content: flex-start;
  align-items: center;
  flex-direction: column;
}
</style>
