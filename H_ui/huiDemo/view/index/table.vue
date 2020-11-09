
<template>
    <div>
        <h-table :data="tData" :columns="columns">
        </h-table>
        <h-page :total="totalNum" @on-change="dataChange" show-elevator show-total :page-size="5"></h-page>
        <select-box :index="tData.length"></select-box>
    </div>
</template>
<script>
    import select_box from "./selectBox";


    var dataList =[
            {
                name: '王小明',
                age: 18,
                address: '北京市朝阳区芍药居',
                authority:1
            },
            {
                name: '张小刚',
                age: 25,
                address: '北京市海淀区西二旗',
                authority:1
            },
            {
                name: '李小红',
                age: 30,
                address: '上海市浦东新区世纪大道',
                authority:1
            },
            {
                name: '周小伟',
                age: 26,
                address: '深圳市南山区深南大道',
                authority:1
            },
            {
                name: '王小明',
                age: 18,
                address: '北京市朝阳区芍药居',
                authority:1
            },
            {
                name: '张小刚',
                age: 25,
                address: '北京市海淀区西二旗',
                authority:1
            },
            {
                name: '李小红',
                age: 30,
                address: '上海市浦东新区世纪大道',
                authority:1
            },
            {
                name: '周小伟',
                age: 26,
                address: '深圳市南山区深南大道',
                authority:1
            },
            {
                name: '11',
                age: 18,
                address: '北京市朝阳区芍药居',
                authority:1
            },
            {
                name: '12',
                age: 25,
                address: '北京市海淀区西二旗',
                authority:1
            },
            {
                name: '13',
                age: 18,
                address: '北京市朝阳区芍药居',
                authority:1
            },
            {
                name: '14',
                age: 25,
                address: '北京市海淀区西二旗',
                authority:1
            },
            {
                name: '15',
                age: 18,
                address: '北京市朝阳区芍药居',
                authority:1
            },
            {
                name: '16',
                age: 25,
                address: '北京市海淀区西二旗',
                authority:1
            },
            {
                name: '17',
                age: 18,
                address: '北京市朝阳区芍药居',
                authority:1
            },
            {
                name: '18',
                age: 25,
                address: '北京市海淀区西二旗',
                authority:1
            },
            {
                name: '19',
                age: 18,
                address: '北京市朝阳区芍药居',
                authority:1
            },
            {
                name: '20',
                age: 25,
                address: '北京市海淀区西二旗',
                authority:1
            },
            {
                name: '21',
                age: 25,
                address: '北京市海淀区西二旗',
                authority:1
            },
            {
                name: '22',
                age: 25,
                address: '北京市海淀区西二旗',
                authority:1
            },
            {
                name: '23',
                age: 25,
                address: '北京市海淀区西二旗',
                authority:1
            },
            {
                name: '24',
                age: 25,
                address: '北京市海淀区西二旗',
                authority:1
            },
            {
                name: '25',
                age: 25,
                address: '北京市海淀区西二旗',
                authority:1
            },
        ]
    export default {
        data(){
            return {
                tData:dataList.slice(0,5),
                totalNum:dataList.length,
                model11: '',
                model12: [],
                columns :[
                    {
                        title: '姓名',
                        key: 'name'
                    },
                    {
                        title: '年龄',
                        key: 'age'
                    },
                    {
                        title: '地址',
                        key: 'address'
                    },
                    {
                        title: '权限级别',
                        key:'authority',
                        // render: (h, params) => {
                        //     let value=this.tData[params.index].authority
                        //     console.log(this.tData)
                        //     return h('select-box', {
                        //         // title可以显示成任意值
                        //         data: {
                        //             value
                        //         }
                        //     } ,value)
                        // }
                    },
                    {
                        title: '操作',
                        render: (h, params) => {
                            return h("select-box",{
                                props:{
                                    type:Number
                                }
                            },params.index);
                        }
                    }
                ]
            }
        },

        components:{
            select_box
        },
        methods:{

            pageChange(index){
                // console.log(index);
            },
            numChange(value){
                console.log(value)
            },
            dataChange(i){
                this.tData=dataList.slice((i-1)*5,i*5);
                console.log(this.tData)
            }

        }
    }
</script>
