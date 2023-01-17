<template>
  <div>
    <div class="container jumbo-box ">

      <!-- titolo + bottone -->
      <div class="container perfomcance-jumbo">
        <h1>
          Performace without compromises
        </h1>
        <p>
          How we helped Blumarine to conquer new business
        </p>
        <button class="btn">
          Discover
        </button>

        <!-- blumarine -->
        <div class="jumbo-blumarine d-flex">
          <h4>
            Blumarine
          </h4>
          <small>
            Front end, Design UX/UI
          </small>
        </div>
        <!-- /blumarine -->
   
      </div>
      <!-- /titolo + bottone -->
      
      <!-- jumbotron immagine -->
      <div class="jumbo-img"></div>
      <!-- /jumbotron immagine -->

      <!-- sfera -->
      <div class="sfera"></div>  
      <!-- /sfera -->

    </div>
  </div>
</template>

<script>
export default {
  name: 'JumboComp',
}
</script>

<style lang= "scss" scoped>

@import '../assets/style/_vars.scss';
@import '../assets/style/_utilities.scss';


.jumbo-box{
  position: relative;
  .perfomcance-jumbo{
    margin-top: 176px;
    h1{
      width: 814px;
      font-size: 72px;
    }
    p{
      color: $fifth-color;
      width: 329px;
      font-size: 1.2rem;
    }
    .btn{
      width: 121px;
      transition: 0.5s;
      @include btn-1;
      &:hover{
        background-color: $fourth-color;
        color: $secondary-color;
      }
    }
    .jumbo-blumarine{
      width: 400px;
      text-align: right;
      flex-direction: column;
      margin-top: 70px;
      small{
        color: $fifth-color;
      }
    }
  }
  .jumbo-img{
    position: absolute;
    z-index: -1;
    height: 566px;
    width: 755px;
    background-image: url('../assets/img/Blauer_Detroit_D5_612.jpg');
    top:-120px;
    right: 135px;
  }
  .sfera{
    position: absolute;
    z-index: -2;
    top: -160px;
    right: -40px;
    width: 880px;
    height: 880px;
    border-radius: 50%;
    background-color: $sixth-color;
  }

}

</style>