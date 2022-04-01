<template>
  <div class="container">
   <div class="row justify-content-around">
    <div class="col-4">
  <img src="" alt="">
    </div>
    <div class="col-4">
     <h4>Hey, I am</h4> 
     <h1>Tursha Arendse</h1>
     <p class="line anim-typewriter">An aspiring frontend web developer</p>

    </div>
  </div>
</div>
</template>

<script>
export default {};
</script>
<style scoped>
h4{padding-top:400px

}
@import url(https://fonts.googleapis.com/css?family=Anonymous+Pro);

html {
      min-height: 100%;
      overflow: hidden;
}

body {
      height: calc(100vh - 6em);
      padding: 4em;
      color: rgba(255, 255, 255, 0.75);
      font-family: "Helvetica Neue",Helvetica,Arial,sans-serif;
      /* background-color: rgb(25, 25, 25); */
}

.line {
      position: relative;
      top: 5%;
      width: 16em;
      margin: 0 auto;
      border-right: 2px solid rgba(255, 255, 255, 0.75);
      font-size: 180%;
      text-align: center;
      white-space: nowrap;
      overflow: hidden;transform: translateY(-50%);
}

/*Animation*/

.anim-typewriter {
      animation: typewriter 4s steps(60) 1s 1 normal both,
      blinkTextCursor 500ms steps(60) infinite normal;
}

@keyframes typewriter {
      from { width: 0;}
      to { width: 16em;}
}

@keyframes blinkTextCursor {
      from {border-right-color: rgba(255, 255, 255, 0.75); }
      to {border-right-color: transparent }
}

</style>
