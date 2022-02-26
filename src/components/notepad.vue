<template>
    <div class="container">
        <div id="notepad" class="row justify-content-md-center">
        
            <div  v-for="partItem in this.arrPart" :key="partItem.name" >
                <partNode :part="partItem" />
               
            </div>
            <div  class="coll-8">
                <itemEditor/>
            </div>

        </div>
    </div>
</template>

<script>
import itemEditor from '@/components/itemEditor';
import partNode from '@/components/partNode';
export default {
    name: 'notepad',
    components:{
        itemEditor,
        partNode
    },
    data(){
        return{
            arrPart:[
                {
                    name: "test1",
                    price: 2,
                    count: 3
                },
                {
                    name: "test2",
                    price: 3,
                    count: 4
                },
                {
                    name: "test3",
                    price: 4,
                    count: 5
                }

             ]
        }
    }
}
</script>

<style scoped>
    #notepad{
        border-color:red;
        border-style: solid;
        border-width: 2px;
        
    }
</style>