<template>
  <section class="section">
    <div class>
      <div class="row">
        <div class="col-12">
          <div class="card">
            <div class="card-header">
              <h4>RIASEC RESULT</h4>
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
                    <th>Id</th>
                    <th>No Pendaftaran</th>
                    <th>jwb1</th>
                    <th>jwb2</th>
                    <th>jwb3</th>
                    <th>jwb4</th>
                    <th>jwb5</th>
                    <th>jwb6</th>
                    <th>jwb7</th>
                    <th>jwb8</th>
                    <th>jwb9</th>
                    <th>jwb10</th>
                    <th>jwb11</th>
                    <th>jwb12</th>
                    <th>jwb13</th>
                    <th>jwb14</th>
                    <th>jwb15</th>
                    <th>jwb16</th>
                    <th>jwb17</th>
                    <th>jwb18</th>
                    <th>jwb19</th>
                    <th>jwb20</th>
                    <th>jwb21</th>
                    <th>jwb22</th>
                    <th>jwb23</th>
                    <th>jwb24</th>
                    <th>jwb25</th>
                    <th>jwb26</th>
                    <th>jwb27</th>
                    <th>jwb28</th>
                    <th>jwb29</th>
                    <th>jwb30</th>
                    <th>jwb31</th>
                    <th>jwb32</th>
                    <th>jwb33</th>
                    <th>jwb34</th>
                    <th>jwb35</th>
                    <th>jwb36</th>
                    <th>jwb37</th>
                    <th>jwb38</th>
                    <th>jwb39</th>
                    <th>jwb40</th>
                    <th>jwb41</th>
                    <th>jwb42</th>
                    <th>jwb43</th>
                    <th>jwb44</th>
                    <th>jwb45</th>
                    <th>jwb46</th>
                    <th>jwb47</th>
                    <th>jwb48</th>
                    <th>jwb49</th>
                    <th>jwb50</th>
                    <th>jwb51</th>
                    <th>jwb52</th>
                    <th>jwb53</th>
                    <th>jwb54</th>
                    <th>jwb55</th>
                    <th>jwb56</th>
                    <th>jwb57</th>
                    <th>jwb58</th>
                    <th>jwb59</th>
                    <th>jwb60</th>
                    <th>jwb61</th>
                    <th>jwb62</th>
                    <th>jwb63</th>
                    <th>jwb64</th>
                    <th>jwb65</th>
                    <th>jwb66</th>
                    <th>jwb67</th>
                    <th>jwb68</th>
                    <th>jwb69</th>
                    <th>jwb70</th>
                    <th>jwb71</th>
                    <th>jwb72</th>
                    <th>jwb73</th>
                    <th>jwb74</th>
                    <th>jwb75</th>
                    <th>jwb76</th>
                    <th>jwb77</th>
                    <th>jwb78</th>
                    <th>jwb79</th>
                    <th>jwb80</th>
                    <th>jwb81</th>
                    <th>jwb82</th>
                    <th>jwb83</th>
                    <th>jwb84</th>
                    <th>jwb85</th>
                    <th>jwb86</th>
                    <th>jwb87</th>
                    <th>jwb88</th>
                    <th>jwb89</th>
                    <th>jwb90</th>

<!-- 
                    <th>Action</th> -->
                  </tr>
                  <tr v-for="(post, i) in posts" :key="i">
                    <td>{{ posts[i].idk}}</td>
                    <td>{{ posts[i].no_pendaftaran}}</td>
                    <td>{{ posts[i].jawab1}}</td>
                    <td>{{ posts[i].jawab2}}</td>
                    <td>{{ posts[i].jawab3}}</td>
                    <td>{{ posts[i].jawab4}}</td>
                    <td>{{ posts[i].jawab5}}</td>
                    <td>{{ posts[i].jawab6}}</td>
                    <td>{{ posts[i].jawab7}}</td>
                    <td>{{ posts[i].jawab8}}</td>
                    <td>{{ posts[i].jawab9}}</td>
                    <td>{{ posts[i].jawab10}}</td>
                    <td>{{ posts[i].jawab11}}</td>
                    <td>{{ posts[i].jawab12}}</td>
                    <td>{{ posts[i].jawab13}}</td>
                    <td>{{ posts[i].jawab14}}</td>
                    <td>{{ posts[i].jawab15}}</td>
                    <td>{{ posts[i].jawab16}}</td>
                    <td>{{ posts[i].jawab17}}</td>
                    <td>{{ posts[i].jawab18}}</td>
                    <td>{{ posts[i].jawab19}}</td>
                    <td>{{ posts[i].jawab20}}</td>
                    <td>{{ posts[i].jawab21}}</td>
                    <td>{{ posts[i].jawab22}}</td>
                    <td>{{ posts[i].jawab23}}</td>
                    <td>{{ posts[i].jawab24}}</td>
                    <td>{{ posts[i].jawab25}}</td>
                    <td>{{ posts[i].jawab26}}</td>
                    <td>{{ posts[i].jawab27}}</td>
                    <td>{{ posts[i].jawab28}}</td>
                    <td>{{ posts[i].jawab29}}</td>
                    <td>{{ posts[i].jawab30}}</td>
                    <td>{{ posts[i].jawab31}}</td>
                    <td>{{ posts[i].jawab32}}</td>
                    <td>{{ posts[i].jawab33}}</td>
                    <td>{{ posts[i].jawab34}}</td>
                    <td>{{ posts[i].jawab35}}</td>
                    <td>{{ posts[i].jawab36}}</td>
                    <td>{{ posts[i].jawab37}}</td>
                    <td>{{ posts[i].jawab38}}</td>
                    <td>{{ posts[i].jawab39}}</td>
                    <td>{{ posts[i].jawab40}}</td>
                    <td>{{ posts[i].jawab41}}</td>
                    <td>{{ posts[i].jawab42}}</td>
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
      .get("/api/riasec")
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
