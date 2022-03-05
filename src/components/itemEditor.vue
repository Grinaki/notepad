<template>
<div class="row justify-content-md-center">
    <div class="row justify-content-md-center">
        <div class="row g-3">
            <div class="col-8">
                <input v-model="currentName" type="text" class="form-control" placeholder="Название товара" aria-label="PartName">
            </div>
            <div class="col-2">
                <input v-model="currentPrice" type="text" class="form-control" placeholder="Цена" aria-label="Price">
            </div>
            <div class="col-2">
                <input v-model="currentCount" type="text" class="form-control" placeholder="Количество" aria-label="Count">
            </div>
        </div>
        <div class="row g-3 justify-content-end">
           <div class="col-1">
                <button v-on:click="addPart" type="button" class="btn btn-primary">Добавить</button>
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default{
    name:'itemEditor',
    data(){
        return{
            currentName: '',
            currentPrice: 0,
            currentCount: 0
        }

    },
    methods:{
        addPart(){
                alert(this.currentName + "\n" + this.currentPrice + "\n" + this.currentCount);
        }
    }
}
</script>

<style scoped>
    button{
        margin-bottom: 20px;
    }
</style>