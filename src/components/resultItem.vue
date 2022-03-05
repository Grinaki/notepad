<template>
<div class="row justify-content-md-center">
    <div id="labelSum" class="alert alert-light col-10" role="alert">
        Итого :
    </div>
    <div class="alert alert-primary col-1" role="alert">
        Количество
    </div>
    <div id="sum" class="alert alert-primary col-1" role="alert">
            Cумма
    </div>
</div>

</template>

<script>

export default {
    name : 'resultItem',
    data(){
        return{

        }
    }
}
</script>

<style scoped>

    .labelSum{
        font-style: italic;
    }
    #sum{
        padding-right:  5 px;
    }
</style>