<template>
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <paper-table :title="table1.title" :sub-title="table1.subTitle" :data="table1.data" :columns="table1.columns">

          </paper-table>
        </div>
      </div>

    </div>
</template>
<script>
  import PaperTable from 'components/UIComponents/PaperTable.vue'
  const tableColumns = ['Id', 'Name', 'Price', 'CreatedAt', 'UpdatedAt', 'SellerName']
  const tableData = [{
    id: 1,
    name: 'Backpack',
    price: '$30',
    createdat: '15/2/2018',
    updatedat: '16/2/2018',
    sellername: 'Nadine Adel'
  },
  {
    id: 2,
    name: 'Clock',
    price: '$40',
    createdat: '11/2/2018',
    updatedat: '17/4/2018',
    sellername: 'Dona Jaradah'
  },
  {
    id: 3,
    name: 'Laptops',
    price: '$55',
    createdat: '18/9/2018',
    updatedat: '16/2/2018',
    sellername: 'Lina Hany'
  },
  {
    id: 4,
    name: 'Bottles',
    price: '$70',
    createdat: '19/2/2018',
    updatedat: '13/2/2018',
    sellername: 'David Hany'
  },
  {
    id: 5,
    name: 'Clothes',
    price: '$100',
    createdat: '15/2/2018',
    updatedat: '16/2/2018',
    sellername: 'Menna Wael'
  }
]

  export default {
    components: {
      PaperTable
    },
    data () {
      return {
        table1: {
          title: 'Component 2',
          subTitle: ' Amazon ',
          columns: [...tableColumns],
          data: [...tableData]
        },
        table2: {
          title: 'Table on Plain Background',
          subTitle: 'Here is a subtitle for this table',
          columns: [...tableColumns],
          data: [...tableData]
        }
      }
    }
  }

</script>
<style>

</style>
