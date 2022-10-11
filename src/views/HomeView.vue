<template>
  <div class="home">

    <TableComponent :headers="headersName" :keys="keysName" :data="bdData"></TableComponent>
  </div>
</template>

<script>
import TableComponent from '@/components/TableComponent.vue'

export default {
  name: 'HomeView',
  components: {
    TableComponent
  },
  data(){
        return {
            headersName: ['Conutry', 'Division', 'District'],
            keysName: ['country', 'division', 'district'],
            bdData: [
                {
                    country: 'Bangladesh',
                    division: 'Dhaka',
                    district: 'Madaripur'
                },
                {
                    country: 'Bangladesh',
                    division: 'Sylhet',
                    district: 'Sunamgang'
                },
                {
                    country: 'Bangladesh',
                    division: 'Chitagong',
                    district: 'Bandarban'
                },
                {
                    country: 'Bangladesh',
                    division: 'Khulna',
                    district: 'Satkhira'
                },
                {
                    country: 'Bangladesh',
                    division: 'Mymensing',
                    district: 'Sherpur'
                },
                {
                    country: 'Bangladesh',
                    division: 'Dhaka',
                    district: 'Dhaka'
                },
                {
                    country: 'Bangladesh',
                    division: 'Barisal',
                    district: 'Bhola'
                }
            ]
        }
    }

}
</script>
