  <template>
    <hooper>
      <slide>
          <renderize/>
      </slide>
      <slide>
          <render2card/>
      </slide>
      <hooper-pagination slot="hooper-addons"></hooper-pagination>
    </hooper>
</template>

<script>
  import {
  Hooper,
  Slide,
  Pagination as HooperPagination 
  } from 'hooper';
  import Renderize from '../cards/renderizecardwelcome.vue'
  import Render2card from '../cards/render2card.vue'
  export default {
    data(){
        return{
            ima:[],
        }
    },
    components: {
      Hooper,
      Slide,
      HooperPagination,
      'renderize' : Renderize,
      'render2card' : Render2card 
    },
    created(){
        axios.get(`${config.apiURL}/carousel`)
        .then((response)=>{
            this.images = response.data
        })
    },
  }
</script>

<style>
  @import '../../scss/hooper.scss'
  
</style>