<template>
  <div class="hello">
  <singlePiano :part="part0" :ALL="ALL0"></singlePiano>
  <singlePiano :part="part1" :ALL="ALL1"></singlePiano>
  <singlePiano :part="part2" :ALL="ALL1"></singlePiano>
  <singlePiano :part="part3" :ALL="ALL1"></singlePiano>
  <singlePiano :part="part4" :ALL="ALL1"></singlePiano>
  <singlePiano :part="part5" :ALL="ALL1"></singlePiano>
  <singlePiano :part="part6" :ALL="ALL1"></singlePiano>
  <singlePiano :part="part7" :ALL="ALL1"></singlePiano>
  <singlePiano :part="part8" :ALL="ALL2"></singlePiano>
  </div>
</template>

<script>
// import singlePiano from './singlePiano.vue' Hello1
import singlePiano from './singlePiano.vue'
export default {
  name: 'hello',
  data () {
    return {
      ALL0:[0,1,2],
      ALL1:[0,1,2,3,4,5,6,7,8,9,10,11],
      ALL2:[0],

      part0:["01-A    -大字2组","02-AP -大字2组","03-B    -大字2组"],
      part1: ["04-C  -大字1组","05-CP-大字1组","06-D  -大字1组","07-DP-大字1组","08-E  -大字1组","09-F  -大字1组","10-FP-大字1组","11-G  -大字1组","12-GP-大字1组","13-A   -大字1组","14-AP-大字1组","15-B  -大字1组"],
      part2: ["16-C  -大字组","17-CP-大字组","18-D  -大字组","19-DP -大字组","20-E -大字组","21-F -大字组","22-FP-大字组","23-G -大字组","24-GP-大字组","25-A -大字组","26-AP-大字组","27-B -大字组"],
      part3: ["28-C   -小字组","29-CP -小字组","30-D  -小字组","31-DP -小字组","32-E  -小字组","33-F  -小字组","34-FP -小字组","35-G  -小字组","36-GP -小字组","37-A  -小字组","38-AP -小字组","39-B  -小字组"],
      part4: ["40-C  -小字1组","41-CP -小字1组","42-D -小字1组","43-DP -小字1组","44-E  -小字1组","45-F   -小字1组","46-FP -小字1组","47-G  -小字1组","48-GP -小字1组","49-A  -小字1组","50-AP -小字1组","51-B    -小字1组"],
      part5: ["52-C    -小字2组","53-CP -小字2组","54-D   -小字2组","55-DP -小字2组","56-E   -小字2组","57-F   -小字2组","58-FP -小字2组","59-G   -小字2组","60-GP-小字2组","61-A  -小字2组","62-AP -小字2组","63-B   -小字2组"],
      part6: ["64-C  -小字3组","65-CP  -小字3组","66-D    -小字3组","67-DP  -小字3组","68-E   -小字3组","69-F  -小字3组","70-FP -小字3组","71-G  -小字3组","72-GP -小字3组","73-A  -小字3组","74-AP -小字3组","75-B  -小字3组"],
      part7: ["76-C  -小字4组","77-CP -小字4组","78-D  -小字4组","79-DP -小字4组","80-E  -小字4组","81-F  -小字4组","82-FP -小字4组","83-G  -小字4组","84-GP -小字4组","85-A  -小字4组","86-AP -小字4组","87-B  -小字4组"],
      part8:["88-C  -小字5组"]
    }
  },
  components:{
    singlePiano
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
