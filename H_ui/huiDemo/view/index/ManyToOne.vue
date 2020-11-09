<template>
<h-table highlight-row border :columns="columns17" :data="data17"></h-table>
</template>
<script>
    import selectbox from "./selectBox"
export default {
    data () {
        return {
            columns17: [
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
                title: '性别',
                key: 'sex',
                // render: (h, params) => {
                //     let sexWord = params.row.sex === 1 ? '男' : '女'
                //     return h('div', {
                //         // title可以显示成任意值
                //         attrs: {
                //             title: sexWord
                //         }
                //     }, sexWord)
                // }
                render: (h, params) => {
            return h('div', [
              h('h-button', {
                props: {
                  type: 'info',
                  size: 'small'
                }
              }, '查看'),
              h('h-button', {
                props: {
                  type: 'error',
                  size: 'small'
                }
              }, '编辑')
            ]);
          },
            }
        ],
            components: {
              selectbox
            },
        data17: [
            {
                name: '王小明',
                age: 18,
                address: '北京市朝阳区芍药居',
                sex: 1
            },
            {
                name: '张小刚',
                age: 25,
                address: '北京市海淀区西二旗',
                sex: 1
            },
            {
                name: '李小红',
                age: 30,
                address: '上海市浦东新区世纪大道',
                sex: 2
            },
            {
                name: '周小伟',
                age: 26,
                address: '深圳市南山区深南大道',
                sex: 1
            },
            {
                name: '王小英',
                age: 26,
                address: '深圳市南山区深南大道',
                sex: 2
            },
        ],
      }
    }
}
</script>
