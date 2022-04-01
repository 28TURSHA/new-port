<template>
  <h1>Resume</h1>
  <div class="container">
  <div class="row">
    <div class="col-md-12 col-lg-8 offset-lg-2">
      <article class="education-item">
        <i class="education-icon fa fa-graduation-cap"></i>
        <h3 class="education-date">2022</h3>
        <div class="card">
          <div class="card-body">
            <h5 class="card-title">Education: </h5>

            <h6 class="card-subtitle"> Life Choices Academy </h6>
            <p class="card-text text-muted">2021 - 2022</p>
            <p class="card-text">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam quis risus id nulla eleifend eleifend. In ligula eros, hendrerit eu tristique sit amet, gravida ut mi. Integer eu nisl id augue aliquet condimentum sit amet nec turpis. Sed eget hendrerit lacus.
              Donec erat lectus, varius sed risus id, bibendum cursus velit </p>
            
          </div>
        </div>
      </article>
      <article class="education-item">
        <i class="education-icon fa fa-graduation-cap"></i>
        <h3 class="education-date">2020</h3>
        <div class="card">
          <div class="card-body">
            <h5 class="card-title">Education: </h5>

            <h6 class="card-subtitle">Wynberg Secondary</h6>
            <p class="card-text text-muted">2016 - 2020</p>
            <p class="card-text">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam quis risus id nulla eleifend eleifend. In ligula eros, hendrerit eu tristique sit amet, gravida ut mi. Integer eu nisl id augue aliquet condimentum sit amet nec turpis. Sed eget hendrerit lacus.
              Donec erat lectus, varius sed risus id, bibendum cursus velit </p>
            
          </div>
        </div>
      </article>
      <article class="education-item">
        <i class="education-icon fa fa-graduation-cap"></i>
        <h3 class="education-date">2020</h3>
        <div class="card">
          <div class="card-body">
            <h5 class="card-title">Volunteer Work:</h5>

            <h6 class="card-subtitle"> Saartjie Baartman Centre for Abused Women & Children</h6>
            <p class="card-text text-muted">2011 - 2015</p>
            <p class="card-text">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam quis risus id nulla eleifend eleifend. In ligula eros, hendrerit eu tristique sit amet, gravida ut mi. Integer eu nisl id augue aliquet condimentum sit amet nec turpis. Sed eget hendrerit lacus.
              Donec erat lectus, varius sed risus id, bibendum cursus velit </p>
        
          </div>
        </div>
      </article>
      <article class="education-item">
        <i class="education-icon fa fa-graduation-cap"></i>
        <h3 class="education-date">2011</h3>
        <div class="card">
          <div class="card-body">
            <h5 class="card-title"> <a href="">
                  Secondary School</a> </h5>

            <h6 class="card-subtitle"> <a href="">link to website</a> </h6>
            <p class="card-text text-muted">2005 - 2011</p>
            <p class="card-text">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam quis risus id nulla eleifend eleifend. In ligula eros, hendrerit eu tristique sit amet, gravida ut mi. Integer eu nisl id augue aliquet condimentum sit amet nec turpis. Sed eget hendrerit lacus.
              Donec erat lectus, varius sed risus id, bibendum cursus velit </p>
            
          </div>
        </div>
      </article>
    </div>
  </div>
</div>

</template>

<script>
export default {};
</script>
<style scoped>
h1 {
  padding-top: 160px;
}

.education-item {
  border-left: 1px solid #000;
  position: relative;
  padding: 32px 24px 8px 40px;
  margin-left: 35px;
}
@media (min-width: 768px) {
  .education-item {
    margin-left: 110px;
  }
}
.education-item .education-icon {
  position: absolute;
  left: -1.3rem;
  width: 42px;
  text-align: center;
  font-size: 22px;
  background-color: #fff;
}
@media (min-width: 768px) {
  .education-item .education-date {
    position: absolute;
    left: -10rem;
    width: 7.5rem;
    text-align: right;
  }
}
</style>
