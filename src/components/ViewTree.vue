<template>
  <ul id="app">
    <app-item
      class="item"
      :model="treeData">
    </app-item>
  </ul>
</template>

<script>
import Item from './Tree.vue';
  export default {
    components: {
      appItem: Item
    },
    data () {
      return {
        treeData: {
            name: 'My Tree',
            children: [
              { name: 'hello' },
              { name: 'wat' },
              {
                name: 'child folder',
                children: [
                  {
                    name: 'child folder',
                    children: [
                      { name: 'hello' },
                      { name: 'wat' }
                    ]
                  },
                  { name: 'hello' },
                  { name: 'wat' },
                  {
                    name: 'child folder',
                    children: [
                      { name: 'hello' },
                      { name: 'wat' }
                    ]
                  }
                ]
              }
            ]
          }
      }
    }
  } 
</script> 