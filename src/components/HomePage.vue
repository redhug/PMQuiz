<template>
  <div class="hello">
     
    <div class="row ml10">
    <b-card bg-variant="secondary" text-variant="white">
         {{question}}
      </b-card>
    </div><br>
    <div class="row ml10">
   
     <b-button @click="revealAns()" variant="success" class="col-md-2">Click here for answer</b-button>
     
      <h3 v-if="ans" class="ml10 rounded border border-success" 
                  style="background-color: darkseagreen;">{{ans}}</h3>
     
 
    </div>
    <br>
  </div>
</template>

<script>
export default {
  name: 'HomePage',
  data: function() {
         return  {
           ans: ''
         }
    },
  props: {
    question: String,
    answer: String
  },
  methods: {
    revealAns(){
      this.ans= this.answer
    }
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
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
.ml10{
  margin-left: 20px;
}
</style>
