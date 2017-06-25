<template>
  <div class="singlePiano">
    <button v-for="index in ALL" :class="returnClass(index)" @click="sing(index)"></button>
  </div>
</template>

<script>

// :class="returnClass(index)

export default {
  name: 'singlePiano',
  data () {  
    return {
      // All:[0,1,2,3,4,5,6,7,8,9,10,11],
      white:[0,2,4,5,7,9,11],
      black:[1,3,6,8,10],
      src:''
    }
  },
  props: {
    part:{},
    ALL:{}
  },
  computed: {
    // a computed getter
  },
  methods: {
    increment () {
      this.count++
    },
    returnClass(index) {
  // `this` points to the vm instance
      if(this.white.indexOf(index)>=0){
        return "white";
      }else if(this.black.indexOf(index)>=0){
        return "black"
      }
    },
    play(index){
      debugger;
      var audio = new Audio("./static/钢琴音色MP3/"+this.part[index]+".mp3");
      audio.play();
    },
    sing(index){
      this.play(index);
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .black{
    width:20px;
    height:100px;
    background-color:black;
    display: initial;
    position: absolute;
    margin-left: -12.5px;
  }
  
  .white{
    width:28px;
    height:150px;
    background-color:white; 
  }
  .singlePiano{
    display: initial;
  }
</style>
