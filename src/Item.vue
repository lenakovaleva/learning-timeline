<template>
    <div>
        <div v-for="milestone in milestones" v-bind:key="milestone.id"
        class="card" style="width: auto"
        v-bind:class="milestone.label"
        >
  <img v-bind:src="milestone.img" class="card-img-top">
  <div class="card-body">
    <a v-bind:href="milestone.url" class="card-link"><h5 class="card-title">{{ milestone.title }}</h5></a>
    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
  </div>
  {{ milestones }}
</div>
        <Data 
        v-bind:milestones="milestones"
        />
    </div>
</template>

<script>

export default {
    name: 'Item',
     data () {
    return {
      milestones: [
    {
        id: 1,
        label: 'course',
        title: 'Title',
        url: 'URL',
        img: 'Image',
    },
    {
        id: 2,
        label: 'course',
        title: 'Title2',
        url: 'URL2',
        img: 'Image2',
    },
],
    }
  }
  
}
</script>