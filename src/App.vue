<!-- <template>
  <div id="app">
      <h3>{{title}}</h3>
      <div class="mygrid">
          <character
          v-for="(id,index) in initial_ids"
          :id="id"
          key="index" />
      </div>
  </div>
</template> -->

<template>
  <div class="tile">
    <character
    v-for="(id,index) in initial_ids"
    :id="id"
    key="index" />
  </div>
</template>


<script>
import character from './components/character.vue'

export default {
  name:'app',
  data(){
    return {
      title:'Games of Thrones : Characters',
      //initial_ids:['56ffc5bf04324408193858ec']
      initial_ids:['56ffc5bf04324408193858ec','56ffc5bf0432440819385b09','56ffc5bf04324408193858b3','56ffc5c00432440819385ddd','56ffc5c00432440819385eab']
    }
  },
  components:{
    character
  }
}
</script>
