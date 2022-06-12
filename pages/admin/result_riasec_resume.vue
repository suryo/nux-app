<template>
  <section class="section">
    <div class>
      <div class="row">
        <div class="col-12">
          <div class="card">
            <div class="card-header">
              <h4>RIASEC RESULT RESUME</h4>
              <!-- <a href="/provinsi/add/" class="btn btn-primary">add</a> -->

              <div class="card-header-form">
                <form>
                  <div class="input-group">
                    <!-- <input
                      type="text"
                      class="form-control"
                      placeholder="Search"
                    /> -->
                    <!-- <div class="input-group-btn">
                      <button class="btn btn-primary">Search</button>
                    </div> -->
                  </div>
                </form>
              </div>
            </div>
            <div class="card-body p-0">
              <div class="table-responsive">
                <table class="table table-bordered">
                  <tr>
                    <th>NO PENDAFTARAN</th>
                    <th>NAMA</th>
                    <th>R</th>
                    <th>I</th>
                    <th>A</th>
                    <th>S</th>
                    <th>E</th>
                    <th>C</th>
                    <th>DESKRIPSI</th>

<!-- 
                    <th>Action</th> -->
                  </tr>
                  <tr v-for="(post, i) in posts" :key="i">
                    <td>{{ posts[i].no_pendaftaran}}</td>
                    <td>{{ posts[i].username}}</td>
                    <td>{{ posts[i].r}}</td>
                    <td>{{ posts[i].i}}</td>
                    <td>{{ posts[i].a}}</td>
                    <td>{{ posts[i].s}}</td>
                    <td>{{ posts[i].e}}</td>
                    <td>{{ posts[i].c}}</td>
                    <td>{{ posts[i].deskripsi}}</td>
                    <!-- <td>
                      <div class="buttons">
                        <nuxt-link
                          class="btn btn-info"
                          :to="`/provinsi/edit/${posts[i].id}`"
                          >EDIT</nuxt-link
                        >

                        <button
                          type="button"
                          class="btn btn-danger"
                          size="sm"
                          @click="deleteProvinsi(posts[i], i)"
                        >
                          DELETE
                        </button>
                      </div>
                    </td> -->
                  </tr>
                </table>
              </div>
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
          link: "/public",
        },

        {
          icon: "github-circle",
          title: "Refview",
          content: `<span>Open source on <a href="https://github.com/buefy/buefy"> GitHub</a></span>`,
          link: "/refview",
        },
        {
          icon: "cellphone-link",
          title: "Advanced Search",
          content: `<span><b class="has-text-grey">Every</b> component is responsive</span>`,
          link: "/coach",
        },
      ],
      posts: [],
      sales: [
        [{ Year: 2018 }, { Year: 2018 }],
        [{ Year: 2017 }, { Year: 2017 }],
      ],
    };
  },

  mounted() {
    console.log("test");
    //fething ke Rest API
    this.$axios
      .get("/api/riasecresult")
      .then((response) => {
        //assign response ke state "posts"
        this.posts = response.data.data;
        console.log(this.posts);
      })
      .catch((error) => {
        console.log(error.response.data);
      });
  },

  methods: {
    async deleteProvinsi(posts, i) {
      //delete data post by ID
      console.log(i);
      await this.$axios.delete(`api/provinsi/${posts.id}`).then(() => {
        //   //remove item array by index
        this.posts.splice(i, 1);
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
