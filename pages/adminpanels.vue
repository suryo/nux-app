<template>
  <section class="section">
    <div class>
      <div class="row">
        <div class="col-lg-3 col-md-6 col-sm-6 col-12">
          <div class="card card-statistic-1">
            <div class="card-icon bg-primary">
              <i class="far fa-user"></i>
            </div>
            <div class="card-wrap">
              <div class="card-header">
                <h4>Total Peserta</h4>
              </div>
              <div class="card-body">{{this.peserta.length}}</div>
            </div>
          </div>
        </div>
        <div class="col-lg-3 col-md-6 col-sm-6 col-12">
          <div class="card card-statistic-1">
            <div class="card-icon bg-danger">
              <i class="far fa-newspaper"></i>
            </div>
            <div class="card-wrap">
              <div class="card-header">
                <h4>TIU</h4>
              </div>
              <div class="card-body">{{this.tiu.length}}</div>
            </div>
          </div>
        </div>
        <div class="col-lg-3 col-md-6 col-sm-6 col-12">
          <div class="card card-statistic-1">
            <div class="card-icon bg-warning">
              <i class="far fa-file"></i>
            </div>
            <div class="card-wrap">
              <div class="card-header">
                <h4>PAPI</h4>
              </div>
              <div class="card-body">{{this.papi.length}}</div>
            </div>
          </div>
        </div>
        <div class="col-lg-3 col-md-6 col-sm-6 col-12">
          <div class="card card-statistic-1">
            <div class="card-icon bg-success">
              <i class="fas fa-circle"></i>
            </div>
            <div class="card-wrap">
              <div class="card-header">
                <h4>RIASEC</h4>
              </div>
              <div class="card-body">{{this.riasec.length}}</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  layout: "stisla/defaultadmin",
  components: {},
  data() {
    return {
      features: [
        {
          icon: "arrange-bring-to-front",
          title: "Public",
          content: `<span>No other internal dependency</span>`,
          link: "/public"
        },

        {
          icon: "github-circle",
          title: "Refview",
          content: `<span>Open source on <a href="https://github.com/buefy/buefy"> GitHub</a></span>`,
          link: "/refview"
        },
        {
          icon: "cellphone-link",
          title: "Advanced Search",
          content: `<span><b class="has-text-grey">Every</b> component is responsive</span>`,
          link: "/coach"
        }
      ],
       peserta: [],
       tiu: [],
       papi: [],
       riasec: [],
    };
  },

    mounted() {
    console.log("test");
    //fething ke Rest API
    this.$axios
      .get("/api/peserta")
      .then((response) => {
        //assign response ke state "posts"
        this.peserta = response.data.data;
        console.log(this.posts.length);
      })
      .catch((error) => {
        console.log(error.response.data);
      });

     this.$axios
      .get("/api/tiu")
      .then((response) => {
        //assign response ke state "posts"
        this.tiu = response.data.data;
        console.log(this.tiu.length);
      })
      .catch((error) => {
        console.log(error.response.data);
      });

      this.$axios
      .get("/api/papi")
      .then((response) => {
        //assign response ke state "posts"
        this.papi = response.data.data;
        console.log(this.papi.length);
      })
      .catch((error) => {
        console.log(error.response.data);
      });

      this.$axios
      .get("/api/riasec")
      .then((response) => {
        //assign response ke state "posts"
        this.riasec = response.data.data;
        console.log(this.riasec.length);
      })
      .catch((error) => {
        console.log(error.response.data);
      });
  },

  
};
</script>


<style scoped>
.main-wrapper-1 .section .section-header {
  margin-left: -30px;
  margin-right: -30px;
  margin-top: -10px;
  border-radius: 0;
  border-top: 1px solid #f9f9f9;
  padding-left: 35px;
  padding-right: 35px;
}
</style>
