<template>
  <div>推荐页面</div>
</template>

<script>
import axios from 'axios'
import {getRecommend} from 'api/recommend'
import {ERR_OK} from 'api/config' 
export default {
  data(){
    return {}
  },
  created(){
   this._getRecommend();
  },
  methods: {
    _getRecommend(){
      getRecommend().then((res) => {
        if(res.code === ERR_OK){
          console.log(res.data.slider);
        }
      })
    }
  }
}
</script>

<style>

</style>
