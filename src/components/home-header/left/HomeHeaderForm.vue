<template>
  <div id="home-header-form">
    <div class="home-header-form-inputs">
      <div class="home-header-form-inputs-item">
        <v-icon
          size="28"
          color="#BDC1CE"
          class="home-header-form-inputs-item-icon"
        >
          apartment
        </v-icon>
        <input
          class="home-header-form-inputs-item-input"
          placeholder="Terrain"
          type="text"
        >
        <v-btn
          color="#BDC1CE"
          class="home-header-form-inputs-right"
          icon
        >
          <v-icon>
            expand_more
          </v-icon>
        </v-btn>
      </div>
      <div class="home-header-form-inputs-separator" />
      <div class="home-header-form-inputs-item">
        <v-icon
          size="28"
          color="#BDC1CE"
          class="home-header-form-inputs-item-icon"
        >
          near_me
        </v-icon>
        <input
          class="home-header-form-inputs-item-input"
          placeholder="Lieux"
          type="text"
        >
        <v-btn
          color="#BDC1CE"
          class="home-header-form-inputs-right"
          icon
        >
          <v-icon
            size="40"
            color="#00BFA6"
          >
            filter_alt
          </v-icon>
        </v-btn>
      </div>
    </div>
    <v-btn
      class="home-header-form-search"
      height="70"
      width="70"
    >
      <v-icon
        color="#fff"
        size="40"
      >
        search
      </v-icon>
    </v-btn>
  </div>
</template>

<script>
export default {
  name: "HomeHeaderForm"
}
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@100;200;300;500;700&family=Raleway:wght@100;200;300;400;500;700&display=swap');
  #home-header-form{
    display: inline-flex;
    height: 98px;
    background: #FFFFFF 0 0 no-repeat padding-box;
    box-shadow: 0 4px 10px #00000029;
    border-radius: 10px;
    align-items: center;
    padding: 0 40px;
    max-width: 780px;
    position: relative;
    .home-header-form-inputs{
      align-items: center;
      display: flex;
      .home-header-form-inputs-item{
        align-items: center;
        display: flex;
        &:last-child{
          .home-header-form-inputs-right{
            margin-right: 10px;
          }
        }
        .home-header-form-inputs-item-icon{
          margin-right: 29px;
        }
        .home-header-form-inputs-item-input{
          font: normal normal 300 30px/46px Poppins;
          color: #BDC1CE;
          width: 100%;
        }
      }
      .home-header-form-inputs-separator{
        width: 2px;
        height: 43px;
        background: #BDC1CE 0 0 no-repeat padding-box;
        border-radius: 20px;
        margin: 0 40px;
      }
    }
    .home-header-form-search{
      background: transparent linear-gradient(180deg, #00BFA6 0%, #288E45 100%) 0 0 no-repeat padding-box;
      position: absolute;
      right: 0;
      transform: translateX(50%);
    }
  }
</style>
