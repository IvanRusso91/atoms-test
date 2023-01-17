<template>
  <main>
    <div class="container ">

      <!-- Zerogrey text -->
      <div class="container zerogrey-text">
        <span>
          Zerogrey is a et iusto odio dignissimos ducimus qui blanditiis praesentium corrupti et quas  excepturi sint occaecati cupiditate non provident.
        </span>
      </div>
      <!-- /Zerogrey text -->

      <!-- oval -->
      <div class="oval0"></div>
      <div class="oval1"></div>
      <!-- /oval -->

      <div class="desktop-text d-flex">

        <!-- How can we ... -->
        <div class="group1 d-flex">
          <h4>How can we help your business?</h4>
          <button class="btn">
            Discover our services
          </button>
        </div>
        <!-- /How can we ... -->

        <!-- Merchant ... -->
        <div class="d-flex container box-group">

          <!-- group 2 -->
          <div class="group2 d-flex container">

            <div class="sub-group d-flex">
              <h5>Merchant of records</h5>
              <small>Neque porro quisquam est, qui dolorem ipsum quia   dolor sit amet, sed quia empora incidunt ut labore et dolore magnam aliquam quaerat voluptatem.
              </small>
            </div>

            <div class="sub-group d-flex">
              <h5>Operations</h5>
              <small>
                Nequempora incidunt ut labore et dolore magnam aliquam quaerat voluptatem.
              </small>
            </div>

            <div class="sub-group d-flex">
              <h5>Marketing & Sales</h5>
              <small>
                Nequempora incidunt ut labore et dolore magnam aliquam quaerat voluptatem.
              </small>
            </div>

            <div class="sub-group d-flex">
              <h5>Store Management</h5>
              <small>
                Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, sed quia non numquam eius modi tempora incidunt ut labore et dolore magnam aliquam quaerat voluptatem.
              </small>
            </div>
            
          </div>
          <!-- /group 2 -->

        </div>
        <!-- /Merchant ... -->


      </div>

      <!-- img mancante + testo -->
      <div class="block d-flex container">
        <div class="text-block">
          <h4>
            Why should  you choose us?
          </h4>
          <small>
            Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet dolorem ipsum quia dolor sit amet.
          </small>
          <div class="box-btn d-flex">
            <button class="btn-why">
              Discover
            </button>
          </div>
        </div>
      </div> 
      <!-- /img mancante + testo -->
        
    </div>
  </main>
</template>

<script>
export default {
  name: 'mainComp'
}
</script>

<style lang="scss" scoped>

@import '../assets/style/_vars.scss';
@import '../assets/style/_utilities.scss';

main{
  .zerogrey-text{
    height: 120px;
    width: 867px;
    color: $third-color;
    font-family: Butler;
    font-size: 32px;
    letter-spacing: -0.3px;
    line-height: 40px;
    text-align: center;
    margin-bottom: 220px;
  }

  .oval0{
    position: absolute;
    z-index: -2;
    top: 1055px;
    right: -150px;
    height: 1500px;
    width: 1500px;
    opacity: 0.08;
    background-color: #80C7E5;
    border-radius: 50%;
  }
  .oval1{
    position: absolute;
    z-index: -1;
    top: 1300px;
    right: 80px;
    height: 1031.25px;
    width: 1031.25px;
    opacity: 0.16;
    background-color: #80C7E5;
    border-radius: 50%;

  }
  .desktop-text{
    .group1{
      justify-content: center;
      flex-direction: column;
      h4{
        width: 308px;
        color:$primary-color;
        font-family: Butler;
        font-size: 48px;
        letter-spacing: -0.3px;
        line-height: 56px;
      }
      button{
        width: 186px;
        @include btn-1;
        font-size: 14px;
        margin-top: 20px;
        &:hover{
          cursor: pointer;
          background-color: $fourth-color;
          color: $secondary-color;
        }
      }
    }
    .group2{
      flex-direction: column;
      .sub-group{
        justify-content: space-around;
        opacity: 0.5;
        animation: 1s;
        &:hover{
          cursor: pointer;
          opacity: 1;
        }
        h5{
          width: 200px;
          color:$primary-color;
          font-family: Butler;
          font-size: 32px;
          font-weight: bold;
          letter-spacing: -0.3px;
          line-height: 40px;
          text-align: right;
          &:not(:nth-last-child(1)){
            padding-bottom: 70px ;
          }
        }
        small{
          height: 72px;
          width: 420px;
          opacity: 0.8;
          color: $primary-color;
          font-family: "Fira Sans";
          font-size: 16px;
          letter-spacing: 0;
          line-height: 24px;
        }
      }  
    }
  }
  .block{
    width: 100%;
    height: 600px;
    background-color: $primary-color;
    margin-bottom: 100px;
    justify-content: end;
    .text-block{
      margin-top: 176px;
      margin-right: 120px;
      text-align: right;
      width: 421px;
      h4{
        height: 112px;
        color: $secondary-color;
        font-family: Butler;
        font-size: 48px;
        font-weight: bold;
        letter-spacing: -0.3px;
        line-height: 56px;
        
      }
      small{
        height: 48px;
        color: $secondary-color;
        font-family: "Fira Sans";
        font-size: 16px;
        letter-spacing: 0;
        line-height: 24px;
      }
      .box-btn{
        justify-content: end;
        margin-top: 28px;
        .btn-why{
          width: 144px;
          height: 40px;
          border: 2px solid $fourth-color;
          border-radius: 30px;
          color:$secondary-color;
          font-family: "Fira Sans";
          font-weight: bold;
          border-color: $secondary-color;
          background-color: transparent;
          transition: 0.5s;
          &:hover{
            background-color: $secondary-color;
            color: black;
          }         
        }
      }
    }
  }
}

/* MQ */

@media screen and (min-width:1200px) and (max-width: 1500px){

  main{
    .zerogrey-text{
      margin-bottom:220px;
    }
    .oval0{
      top: 1055px;
      right: -150px;
    }
    .oval1{
      position: absolute;
      z-index: -1;
      top: 1300px;
      right: 80px;
      height: 1031.25px;
      width: 1031.25px;
      opacity: 0.16;
      background-color: #80C7E5;
      border-radius: 50%;

    }
  }
}

@media screen and (min-width:800px) and (max-width: 1200px){

  main{
    .zerogrey-text{
      margin-bottom:220px;
    }
    .oval0{
      top: 1055px;
      right: -150px;
    }
    .oval1{
      position: absolute;
      z-index: -1;
      top: 1300px;
      right: 80px;
      height: 1031.25px;
      width: 1031.25px;
      opacity: 0.16;
      background-color: #80C7E5;
      border-radius: 50%;

    }
  }
}
</style>