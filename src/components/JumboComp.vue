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


        <div class="box-bluma-from">
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

          <!-- from -->
          <div class="from">
            <section class="d-flex">
              <h5>
                From our studio
              </h5>
              <img src="../assets/img/White.svg" alt="X">
            </section>

            <small>
              Get a Weekly email with inspirational contents from <br> Zerogrey. 
            </small>
            
            <div class="write-email d-flex">
              <input  type="text" placeholder="write your e-mail">
              <img src="../assets/img/white(1).svg" alt="arrow">
            </div>

            <div class="write-row"></div>

            <div class="privacy-policy">
              <input type="checkbox">
              <label for="vehicle1"> I read and accept the Privacy policy</label>
            </div>
          </div>
          <!-- /from -->

        </div>
   
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
  margin-bottom:350px;
  .perfomcance-jumbo{
    margin-top: 176px;
    h1{
      font-family: Butler;
      width: 814px;
      font-size: 80px;
    }
    p{
      font-family: "Fira Sans";
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
    .box-bluma-from{
      .jumbo-blumarine{
        font-family: Butler;
        width: 400px;
        text-align: right;
        flex-direction: column;
        margin-top: 75px;
        small{
          font-family: "Fira Sans";
          color: $fifth-color;
        }
      }
      .from{
        position: absolute;
        right: 40px;
        top: 340px;
        margin-right: -75px;
        padding: 64px 58px 51px 48px;
        background-color: $primary-color;
        color : $secondary-color;
        section{
          justify-content: space-between;
          h5{
            font-family: Butler;
            font-size: 32px;
          } 
        }
        small{
          font-family: "Fira Sans";
        }
        .write-email{
          margin-top: 41px;
          justify-content: space-between;
          input{
            width: 290px;
            padding-bottom: 3px;
            background-color: transparent;
            border: none;
          }
        }
        .write-row{
          width: 100%;
          border: 1px solid $secondary-color;
          border-top: none;
        }
        .privacy-policy{
          margin-top: 20px;
          input{
            width: 16px;
            height: 16px;
          }
          label{
            font-family: "Fira Sans";
            margin-left: 8px;
            font-size: 12px;
          }
        }
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