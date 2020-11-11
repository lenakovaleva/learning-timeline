<template>
 <section>
    <div class="container">
      <div class="row">
        <div class="col-12">
         <div class="wrapper">
           <Item />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Item from "./Item.vue"

export default {
  name: 'Timeline',
    components: {
    Item
  }, 
  props: {
    msg: String
  },
};
</script>


<style scoped>

</style>
