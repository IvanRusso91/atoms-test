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

      <section>
        <JumboComp />
      </section>
      <!-- /Navbar -->

    </div>
</template>

<script>

import JumboComp from '@/components/JumboComp';

export default {
  name: 'App',
  components: {
    JumboComp,
  }
}
</script>

<style lang="scss">

@import './assets/style/_global.scss';
@import './assets/style/_vars.scss';

.box-nav{
  margin-top: 30px;
  justify-content: space-between;
  .btn-nav{
    justify-content: end;
    li{
      margin-top: 10px;
      display: inline-block;
      text-transform: uppercase;
      text-align: center;
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

</style>
