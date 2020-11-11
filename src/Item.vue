<template>
    <div>
        <div v-for="milestone in milestones" v-bind:key="milestone.id"
        class="card" style="width: auto"
        v-bind:class="milestone.label"
        >
  <!-- <img v-bind:src="milestone.img" class="card-img-top"> -->
  <div class="card-body">
    <a v-bind:href="milestone.url" class="card-link"><h5 class="card-title">{{ milestone.title }}</h5></a>
    <p v-bind:class="card-text">{{ milestone.text }}</p>
  </div>
</div>
    </div>
</template>

<script>

export default {
    name: 'Item',
     data () {
    return {
      milestones: [
    {
        id: 14,
        label: 'course',
        title: 'Git How To',
        url: 'https://githowto.com/ru',
        img: 'Image',
        text: '',
    }, 
    {
        id: 13,
        label: 'course',
        title: 'Vue JS',
        url: 'https://www.youtube.com/watch?v=OlnwgS-gk8Y&t=2s',
        img: 'Image',
        text: '',
    }, 
    {
        id: 12,
        label: 'book',
        title: 'Стив Круг "Не заставляйте меня думать"',
        url: 'https://www.ozon.ru/context/detail/id/139556451/',
        img: 'Image',
        text: '',
    },       
    {
        id: 11,
        label: 'course',
        title: 'Watch and Code',
        url: 'https://watchandcode.com/p/practical-javascript',
        img: 'Image',
        text: '',
    }, 
    {
        id: 10,
        label: 'course',
        title: 'CSS Grid',
        url: 'https://cssgrid.io/',
        img: 'Image',
        text: '',
    }, 
    {
        id: 9,
        label: 'course',
        title: 'HTML5 Canvas',
        url: 'https://chriscourses.com/courses/canvas-for-beginners/resizing',
        img: 'Image',
        text: '',
    },  
    {
        id: 8,
        label: 'course',
        title: 'Internet History, Technology, and Security on Coursera',
        url: 'https://www.coursera.org/learn/internet-history/home/welcome',
        img: 'Image',
        text: '',
    },   
    {
        id: 7,
        label: 'course',
        title: 'Using Databases with Python',
        url: 'https://www.coursera.org/learn/python-databases/home/welcome',
        img: 'Image',
        text: '',
    },     
    {
        id: 6,
        label: 'course',
        title: 'Using Python to Access Web Data',
        url: 'https://www.coursera.org/learn/python-network-data/home/welcome',
        img: 'Image',
        text: '',
    },
    {
        id: 5,
        label: 'course',
        title: 'Python Data Structures',
        url: 'https://www.coursera.org/learn/python-data/home/welcome',
        img: 'Image',
        text: '',
    },
    {
        id: 4,
        label: 'course',
        title: 'Programming for Everybody (Getting Started with Python)',
        url: 'https://www.coursera.org/learn/python/home/welcome',
        img: 'Image',
        text: '',
    },
    {
        id: 3,
        label: 'course',
        title: 'Javascript on SoloLearn',
        url: 'https://www.sololearn.com/Course/JavaScript/',
        img: 'Image',
        text: '',
    },
    {
        id: 2,
        label: 'course',
        title: 'CSS on SoloLearn',
        url: 'https://www.sololearn.com/Course/CSS/',
        img: 'Image',
        text: '',
    },
    {
        id: 1,
        label: 'course',
        title: 'HTML on SoloLearn',
        url: 'https://www.sololearn.com/Course/HTML/',
        img: 'Image2',
        text: '',
    },
],
    }
  }
  
}
</script>