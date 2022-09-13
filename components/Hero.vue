<template>
  <div class="hero-wrapper hero d-flex">
    <b-container class="d-flex">
      <b-row>
        <b-col cols="12" md="6">
          <h3 class="title c-white">
            Headache on complex customs matters for your business?
          </h3>
          <img src="seprator2.svg" class="py-4" />
          <p class="c-white desc pb-2">
            Customs Support is your neutral full-service customs broker for
            complex customs matters with 20+ years of expertise in Europe and
            over 400 customs specialists who are happy to take the load off your
            mind!
          </p>
          <button class="standard-btn px-4">Get your quote now</button>
        </b-col>
        <b-col cols="12" md="6">
          <ul class="c-white">
            <li>Fast and accurate customs clearance delivery</li>
            <li>EU-wide customs coverage</li>
            <li>EU-wide customs coverage</li>
          </ul>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<style lang="scss" scoped>
.hero {
  height: 600px;
  /* UI Properties */
  align-items: center;
  background: url("/hero.png");
  .title {
    font-size: 40px;
  }
  .desc {
    font-size: 16px;
  }
  ul {
    list-style: none;
    li {
      padding: 10px 0px;
      font-size: 20px;
      position: relative;
      &:before {
        background: url(/bullet.svg) no-repeat !important;
        height: 23px;
        width: 21px;
        position: absolute;
        top: 20px;
        left: -31px;
        content: "";
      }
    }
  }
}
.nuxt-logo {
  height: 180px;
}
@media only screen and (max-width: 1024px) {
  .hero {
    height: 600px;
    /* UI Properties */
    align-items: center;
    background: url("/hero.png");
    .title {
      font-size: 20px;
    }
    .desc {
      font-size: 16px;
    }
    ul {
      list-style: none;
      li {
        padding: 10px 0px;
        font-size: 18px;
        position: relative;
        &:before {
          background: url(/bullet.svg) no-repeat !important;
          height: 23px;
          width: 21px;
          position: absolute;
          top: 20px;
          left: -31px;
          content: "";
        }
      }
    }
  }
}
</style>
<script>
export default {
  name: 'HeroWrapper'
}
</script>
