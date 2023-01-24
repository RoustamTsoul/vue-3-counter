<template>
  <div class="block">
    <h1>{{text}} : {{count}}</h1>
    <div class="buttons">
        <button v-on:click="add" type="button" class="btn btn-succes">Add</button>
        <button v-on:click="subtract" type="button" class="btn btn-danger">Subtract</button>
    </div>
  </div>
</template>

<script>
export default {
    data(){
        return{
            text:'Count',
            count:0
        }
    },

    methods:{
        add(){
            this.count++
        },

        subtract(){
            this.count--
        }
    }
}
</script>

<style scoped>
.block{
/* border: 5px solid black; */
width: 650px;
height: 450px;
margin: auto;
padding: 25px;
display: flex;
justify-content: center;
align-items: center;
text-align: center;
flex-direction: column;
background-color: rgba(232, 51, 147, 0.774);
border-radius: 10px;
box-shadow: 5px 5px 5px 5px rgb(188, 43, 188);
}

h1{
font-size: 3rem;
}

.btn{
font-size: 1rem;
font-family: 'Rubik Gemstones', cursive;
width: 115px;
height: 65px;
border-radius: 100px;
padding: 15px;
margin: 5px;
}

.btn-succes{
background: radial-gradient(circle, rgba(238,174,202,1) 15%, rgba(148,187,233,1) 94%);
}

.btn-succes:hover{
background: radial-gradient(circle, rgb(175, 37, 97) 15%, rgb(69, 133, 206) 94%);
}

.btn-danger{
background: linear-gradient(90deg, rgba(131,58,180,1) 6%, rgba(246,0,0,1) 47%, rgba(252,176,69,1) 89%);
}

.btn-danger:hover{
background: linear-gradient(90deg, rgb(66, 6, 106) 6%, rgb(110, 8, 8) 47%, rgb(200, 124, 17) 89%);
}
</style>