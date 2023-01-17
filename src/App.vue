<template>
    <div>
      <header>
        <!-- Navbar -->
        <div class="container box-nav d-flex">
          <!-- logo -->
          <div class="container">
            <img src="./assets/img/logo-3.svg" alt="logo-3">
          </div>
          <!-- /logo -->

          <!-- btn navbar -->
          <div class="container d-flex btn-nav">
            <nav>
              <ul>
                <li>
                  <a href="#">Works</a>
                </li>
                <li>
                  <a href="#">Services</a>
                </li>
                <li>
                  <a href="#">Why us</a>
                </li>
                <li>
                  <a class="last" href="#">Let's talk</a>
                </li>
                <li>
                  <div class="box-icon">
                    <div class="rec-copy"></div>
                    <div class="rec-copy"></div>
                    <small>menu</small>               
                  </div>
                </li>
              </ul>
            </nav>

          </div>
          <!-- /btn navbar -->

        </div>
      </header>
      <!-- /Navbar -->

      <!-- jumbotron -->
      <section>
        <JumboComp />
      </section>
      <!-- /jumbotron -->
      

      <MainComp />
      

    </div>
</template>

<script>

import JumboComp from '@/components/JumboComp';
import MainComp from '@/components/MainComp';

export default {
  name: 'App',
  components: {
    JumboComp,
    MainComp,
  }
}
</script>

<style lang="scss">

@import './assets/style/_global.scss';
@import './assets/style/_vars.scss';

  header{
    position: fixed ;
    top: 0;
    left: 0;
    right: 0;
    z-index: 999;
    background-color: $secondary-color;
    .box-nav{
      margin-top: 30px;
      justify-content: space-between;
      padding-bottom: 20px;
      .btn-nav{
        justify-content: end;
        li{
          margin-top: 10px;
          display: inline-block;
          text-transform: uppercase;
          text-align: center;
          font-family: "Fira Sans";
          a{  
            font-weight: bold;
            margin-right: 22px;
            padding: 15px 16px 15px 16px;
            &:hover{
              background-color: $fourth-color;
              color: $secondary-color;
              border-radius: 30px;
            }
          }
          .last{
            background-color: $fourth-color;
            color: $secondary-color;
            border-radius: 30px;
          }
          .box-icon{
            &:hover{
              cursor: pointer;
    
            }
            .rec-copy{
              height: 2px;
              width: 24px;
              border-radius: 1px;
              background-color: #484A54;
              &:nth-child(2){
                margin-top: 2px;
                margin-bottom: -10px;
              }
            }
            small{
              font-size: 0.5em;
              font-weight: bold;
            }
          }
        }
      }
    }
  }

/* MQ */ 



@media screen and (min-width:1200px) and (max-width: 1500px) {

  header{
    .box-nav{
      .btn-nav{
        li{
          a{  
            font-weight: bold;
            margin-right: px;
            padding: 15px 16px 15px 16px;
            &:hover{
              background-color: $fourth-color;
              color: $secondary-color;
              border-radius: 30px;
            }
          }
          .last{
            background-color: $fourth-color;
            color: $secondary-color;
            border-radius: 30px;
          }
          .box-icon{
            margin-left: 10px;
            &:hover{
              cursor: pointer;
            }
            .rec-copy{
              height: 2px;
              width: 24px;
              border-radius: 1px;
              background-color: #484A54;
              &:nth-child(2){
                margin-top: 2px;
                margin-bottom: -10px;
              }
            }
            small{
              font-size: 0.5em;
              font-weight: bold;
            }
          }
        }
      }
    }
  }
        
}


@media screen and (min-width:800px) and (max-width: 1200px) {

  header{
    .box-nav{
      .btn-nav{
        li{
          a{  
            display: none;
          }
          .last{
            display: block;
          }
          .box-icon{
            .rec-copy{
              width: 48px;
              &:nth-child(2){
                margin-bottom: -5px;
              }
            }
            small{
              font-size: 1em;
            }
          }
        }
      }
    }
  }
        
}

</style>
