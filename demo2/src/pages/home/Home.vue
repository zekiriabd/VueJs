<template src="./Home.html"/>

<script setup>
    import {DxDataGrid,DxColumn,DxGrouping,DxGroupPanel,DxPager,DxPaging,DxSearchPanel} 
    from 'devextreme-vue/data-grid';
</script>

<script>
export default{
  data() {
    return {
      users:[
        {id:1,name:"zekiri abdelali"},
        {id:2,name:"Aloui Ali"},
        {id:3,name:"Raouf Rahich"}
      ],
      selectedUser:{},
    }
  },
  methods: {
    onSelectionChanged({ selectedRowsData }) {      
      this.selectedUser = selectedRowsData[0];     
      console.log(selectedRowsData[0]);
    },
  },
}
</script>