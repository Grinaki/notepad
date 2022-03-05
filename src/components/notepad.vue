<template>
    <div class="container">
        <div id="notepad" class="row justify-content-md-center">
            <h1> Учет товаров </h1>
                <partNode :part="partItem"  v-for="partItem in this.arrPart" :key="partItem.name"  />
                <resultItem />
            <div  class="coll-8">
                <itemEditor v-on:sendItem="testFun" />
            </div>

        </div>
    </div>
</template>

<script>
import itemEditor from '@/components/itemEditor';
import partNode from '@/components/partNode';
import resultItem from '@/components/resultItem';
export default {
    name: 'notepad',
    components:{
        itemEditor,
        partNode,
        resultItem
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
    },
    methods:{
        testFun(c){
            this.arrPart.push(c);
        }
    }
}
</script>

<style scoped>
    #notepad{
        border-color:red;
        border-style: solid;
        border-width: 2px;
        padding-top: 20px;
        
    }
</style>