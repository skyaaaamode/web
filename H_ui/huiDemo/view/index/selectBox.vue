<template>
    <div>
        <h-select style="width:200px" @on-change="method01"
                  placeholder="请选择用户权限" v-on:on-change="">
            <h-option value="1" label="可编辑">
                <span>Edit</span>
                <span style="float:right;color:#ccc">可编辑</span>
            </h-option>
            <h-option value="2" label="可读" setDefSelect="true">
                <span>ReadOnly</span>
                <span style="float:right;color:#ccc">可读</span>
            </h-option>
            <h-option value="3" label="隐藏">
                <span>Hidden</span>
                <span style="float:right;color:#ccc">隐藏</span>
            </h-option>
        </h-select>
    </div>
</template>
<script>
    export default {
        data(){
            return{
                model9:1
            }
        },
        props:{
            index:Number
        },
        methods:{
            method01:function(){
                console.log(this.father)
            }

        }
    }
</script>
