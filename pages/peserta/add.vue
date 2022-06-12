<template>
  <section class="section">
    <div class>
      <div class="row">
        <div class="col-12">
          <div class="card">
            <div class="card-header">
              <h4>Input Peserta</h4>
            </div>
            <div class="card-body">
              <form
                @submit="store"
                method="POST"
                action="#"
                class="needs-validation"
                novalidate=""
              >
                <div class="form-group">
                  <label>NO PENDAFTARAN</label>
                  <input type="text" v-model="peserta.no_pendaftaran" class="form-control" />
                </div>

                <div class="form-group">
                  <label>NAMA</label>
                  <input type="text" v-model="peserta.nama" class="form-control" />
                </div>

                <div class="form-group">
                  <label>ASAL SEKOLAH</label>
                  <input type="text" v-model="peserta.asal_sekolah" class="form-control" />
                </div>

                <div class="form-group">
                  <label
                    class="
                      col-form-label
                      text-md-right
                      col-12 col-md-3 col-lg-3
                    "
                  ></label>
                  <div class="col-sm-12 col-md-7">
                    <button type="submit" class="btn btn-primary">
                      SIMPAN
                    </button>
                  </div>
                </div>
              </form>
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
      //state post
      peserta: {
        no_pendaftaran: 0,
        nama: "",
        asal_sekolah: "",
        status: "",
      },
      //state validation
      validation: [],
    };
  },

  methods: {
    //method "store"
    async store(e) {
      e.preventDefault();

      //  await this.$axios
      //       .get("/api/peserta")
      // .then((response) => {
      //   console.log("masuk");
      //   //assign response ke state "posts"
      //   this.posts = response.data.data;
      //   console.log(this.posts);
      // })
      // .catch((error) => {
      //   console.log("error");
      //   // console.log(error.response.data);
      // });
 let datax = 
 {
      data: [
          {
          no_pendaftaran: this.peserta.no_pendaftaran,
          nama: this.peserta.nama,
          asal_sekolah: this.peserta.asal_sekolah,
          status:this.peserta.status,
          },
        ],
 }

      //send data ke Rest API
        await this.$axios({
        method: "post",
        headers: { "content-type": "application/json" },
        url: "/api/peserta",
        data: datax,
      })
        .then(() => {
          this.$router.push({
            name: "peserta",
          });
        })
        .catch((error) => {
          this.validation = error.response.data;
        });
    },
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
