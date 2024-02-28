<script>
// import {ref} from "vue"
// import ListItem from './ListItem.vue'
// let v = ref("");
export default{
    data() {
        return {
            values : ["",],
            totalPrice : 0,
        }
    },
    methods:{
        calc(){
            let num = 0;
            for(let i = 0;i < this.values.length;i++){
                if(this.values[i] != -1){
                    num += this.values[i] * 1
                }
            }
            if ( this.totalPrice * 1 + num  == NaN){
                return 0;
            }else{
                return this.totalPrice * 1 + num * 1
            }
        },
        add(){
            this.values.push("");
        },
        del(index){
            this.values[index] = -1;
        },
    }
}
</script>

<template>
    <div class="my-5 pb-3">
        <div class="text-center">
            <span>現在の合計金額</span>
            <h2 class="text-center">{{ calc() }}円</h2>
        </div>
        <div class="mt-3">
            <div class="m-auto mt-3 px-2" style="max-width: 800px;">
                <div v-for="(value,index) in values">
                    <div v-if="value != -1" class="input-group mb-1">
                        <!-- <div class="input-group-text">
                            <input class="form-check-input mt-0" type="checkbox" value="" aria-label="Checkbox for following text input">
                        </div>                 -->
                        <input type="text" class="form-control" placeholder="商品名" aria-label="name">
                        <!-- <span class="input-group-text">値段</span> -->
                        <input type="text" class="form-control" placeholder="値段" v-model="values[index]">
                        <span class="input-group-text">円</span>
                        <button class="btn btn-danger" type="button" id="button-addon2" @click="del(index)">削除</button>
                    </div>
                </div>
            </div>
        </div>
        <div class="d-grid gap-2 d-md-block mx-auto pt-4" style="max-width: 50px;">
            <button class="btn btn btn-outline-primary text-center" type="button" @click="add"><i class="bi bi-plus-lg"></i></button>
        </div>
    </div>
</template>
