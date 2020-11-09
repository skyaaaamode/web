<template>
    <div>
        <h-edit-gird :columns="columns1" :data="data1"
                     @on-editselect-change="updateAuth"	></h-edit-gird>
        <div class="box" >
            <h-page :total="totalNum" @on-change="dataChange" show-elevator show-total :page-size="5"></h-page>
        <div class="btnGroup"><h-button type="info" @click="submitUpdate">确认</h-button>
        <h-button @click="quitUpdate">取消</h-button>
        </div>
        </div>

    </div>
</template>
<style>
    .box{
        display: flex;
        justify-items: center;
        flex-direction: column;
    }
    .btnGroup{
        display: flex;
        flex-direction: row;
    }
</style>
<script>
    var dataList02=[
        {
            h5app_id: '王小明',
            name: '北京市朝阳区芍药居',
            resource_id: 1,
            authority: 1,
        },
        {
            h5app_id: '王小明',
            name: '北京市朝阳区芍药居',
            resource_id: 2,
            authority: 1,
        },
        {
            h5app_id: '王小明',
            name: '北京市朝阳区芍药居',
            resource_id: 3,
            authority: 1,
        },
        {
            h5app_id: '王小明',
            name: '北京市朝阳区芍药居',
            resource_id: 4,
            authority: 1,
        },
        {
            h5app_id: '王小明',
            name: '北京市朝阳区芍药居',
            resource_id: 5,
            authority: 1,
        },
        {
            h5app_id: '王小明',
            name: '北京市朝阳区芍药居',
            resource_id: 6,
            authority: 1,
        }];
    export default {

        data () {
            return {

                totalNum:dataList02.length,
                pageNum:5,
                partner_resourcea_updata_list:[],
                columns1: [
                    {
                        type: 'text',
                        title: '离线包ID',
                        key: 'h5app_id',
                        // width: 200,
                        viewValue:true
                    },
                    {
                        type: 'text',
                        title: '离线包名称',
                        // width: 200,
                        key: 'name',
                        hiddenCol:false,
                        viewValue:true
                    },
                    {
                        type: 'text',
                        title: '离线包资源Id',
                        key: 'resource_id',
                        // width: 200,
                        viewValue:true
                    },
                    {
                        type: 'select',
                        title: '编辑权限(双击单元格)',
                        width: 200,
                        key: 'authority',
                        multiple:false,
                        transfer:true,
                        customOption(row) {
                            let options = []
                                options = [
                                    {
                                        label: '可见',
                                        value: '1'
                                    },
                                    {
                                        label: '隐藏',
                                        value: '3'
                                    }
                                ]
                            return options
                        }
                    },
                ],
                data1: dataList02.slice(0,this.pageNum),
                options1: [],
            }
        },
        mounted(){
            this.options1=[{label:'可见',value:'1'},{label:'隐藏',value:'3'}]
        },
        methods: {
            dataChange(i){
                this.data1=dataList02.slice((i-1)*this.pageNum,i*this.pageNum);
                console.log(dataList02);
                console.log(this.pageNum)
            },
            updateAuth(val,i,j){
                console.log(val);
                console.log(i);
                console.log(j);
                this.data1[j].authority=val;
                var item=this.data1[j];
                console.log(item)
                this.partner_resourcea_updata_list.push(item);
            },
            submitUpdate(){
                console.log(this.partner_resourcea_updata_list)
            },
            quitUpdate(){
                this.partner_resourcea_updata_list=[];
                this.data1=this.dataList02.slice(0,this.pageNum),
                console.log(this.partner_resourcea_updata_list);
            }
        }
    }
</script>
