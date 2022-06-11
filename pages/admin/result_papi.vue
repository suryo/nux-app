<template>
  <section class="section">
    <div class>
      <div class="row">
        <div class="col-12">
          <div class="card">
            <div class="card-header">
              <h4>PAPI RESULT</h4>
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
                    <td>{{ posts[i].id }}</td>
                    <td>{{ posts[i].no_pendaftaran}}</td>
                    <td>{{ posts[i].jwb1}}</td>
                    <td>{{ posts[i].jwb2}}</td>
                    <td>{{ posts[i].jwb3}}</td>
                    <td>{{ posts[i].jwb4}}</td>
                    <td>{{ posts[i].jwb5}}</td>
                    <td>{{ posts[i].jwb6}}</td>
                    <td>{{ posts[i].jwb7}}</td>
                    <td>{{ posts[i].jwb8}}</td>
                    <td>{{ posts[i].jwb9}}</td>
                    <td>{{ posts[i].jwb10}}</td>
                    <td>{{ posts[i].jwb11}}</td>
                    <td>{{ posts[i].jwb12}}</td>
                    <td>{{ posts[i].jwb13}}</td>
                    <td>{{ posts[i].jwb14}}</td>
                    <td>{{ posts[i].jwb15}}</td>
                    <td>{{ posts[i].jwb16}}</td>
                    <td>{{ posts[i].jwb17}}</td>
                    <td>{{ posts[i].jwb18}}</td>
                    <td>{{ posts[i].jwb19}}</td>
                    <td>{{ posts[i].jwb20}}</td>
                    <td>{{ posts[i].jwb21}}</td>
                    <td>{{ posts[i].jwb22}}</td>
                    <td>{{ posts[i].jwb23}}</td>
                    <td>{{ posts[i].jwb24}}</td>
                    <td>{{ posts[i].jwb25}}</td>
                    <td>{{ posts[i].jwb26}}</td>
                    <td>{{ posts[i].jwb27}}</td>
                    <td>{{ posts[i].jwb28}}</td>
                    <td>{{ posts[i].jwb29}}</td>
                    <td>{{ posts[i].jwb30}}</td>
                    <td>{{ posts[i].jwb31}}</td>
                    <td>{{ posts[i].jwb32}}</td>
                    <td>{{ posts[i].jwb33}}</td>
                    <td>{{ posts[i].jwb34}}</td>
                    <td>{{ posts[i].jwb35}}</td>
                    <td>{{ posts[i].jwb36}}</td>
                    <td>{{ posts[i].jwb37}}</td>
                    <td>{{ posts[i].jwb38}}</td>
                    <td>{{ posts[i].jwb39}}</td>
                    <td>{{ posts[i].jwb40}}</td>
                    <td>{{ posts[i].jwb41}}</td>
                    <td>{{ posts[i].jwb42}}</td>
                    <td>{{ posts[i].jwb43}}</td>
                    <td>{{ posts[i].jwb44}}</td>
                    <td>{{ posts[i].jwb45}}</td>
                    <td>{{ posts[i].jwb46}}</td>
                    <td>{{ posts[i].jwb47}}</td>
                    <td>{{ posts[i].jwb48}}</td>
                    <td>{{ posts[i].jwb49}}</td>
                    <td>{{ posts[i].jwb50}}</td>
                    <td>{{ posts[i].jwb51}}</td>
                    <td>{{ posts[i].jwb52}}</td>
                    <td>{{ posts[i].jwb53}}</td>
                    <td>{{ posts[i].jwb54}}</td>
                    <td>{{ posts[i].jwb55}}</td>
                    <td>{{ posts[i].jwb56}}</td>
                    <td>{{ posts[i].jwb57}}</td>
                    <td>{{ posts[i].jwb58}}</td>
                    <td>{{ posts[i].jwb59}}</td>
                    <td>{{ posts[i].jwb60}}</td>
                    <td>{{ posts[i].jwb61}}</td>
                    <td>{{ posts[i].jwb62}}</td>
                    <td>{{ posts[i].jwb63}}</td>
                    <td>{{ posts[i].jwb64}}</td>
                    <td>{{ posts[i].jwb65}}</td>
                    <td>{{ posts[i].jwb66}}</td>
                    <td>{{ posts[i].jwb67}}</td>
                    <td>{{ posts[i].jwb68}}</td>
                    <td>{{ posts[i].jwb69}}</td>
                    <td>{{ posts[i].jwb70}}</td>
                    <td>{{ posts[i].jwb71}}</td>
                    <td>{{ posts[i].jwb72}}</td>
                    <td>{{ posts[i].jwb73}}</td>
                    <td>{{ posts[i].jwb74}}</td>
                    <td>{{ posts[i].jwb75}}</td>
                    <td>{{ posts[i].jwb76}}</td>
                    <td>{{ posts[i].jwb77}}</td>
                    <td>{{ posts[i].jwb78}}</td>
                    <td>{{ posts[i].jwb79}}</td>
                    <td>{{ posts[i].jwb80}}</td>
                    <td>{{ posts[i].jwb81}}</td>
                    <td>{{ posts[i].jwb82}}</td>
                    <td>{{ posts[i].jwb83}}</td>
                    <td>{{ posts[i].jwb84}}</td>
                    <td>{{ posts[i].jwb85}}</td>
                    <td>{{ posts[i].jwb86}}</td>
                    <td>{{ posts[i].jwb87}}</td>
                    <td>{{ posts[i].jwb88}}</td>
                    <td>{{ posts[i].jwb89}}</td>
                    <td>{{ posts[i].jwb90}}</td>
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
      .get("/api/papi")
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
