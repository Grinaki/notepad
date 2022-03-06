<template>
    <div class="row justify-content-md-center">
        <div  class="alert alert-dark col-6" role="alert">
            {{part.name}} 
        </div>
        <div class="alert alert-dark col-2" role="alert">
            {{part.count}} 
        </div>
        <div class="alert alert-dark col-2" role="alert">
            {{part.price}} 
        </div>
        <div class="alert alert-dark col-2" role="alert">
           {{sum}}
        </div>
    </div>    
</template>

<script>
export default{
    name: 'partNode',
    props: {
        part:{
            name:String,
            price: Number,
            count: Number
        }
      
    },
    computed:{
       sum(){
          return 5 + 12;
       }

    }
}
</script>

