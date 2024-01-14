<script>
import Draggable from 'vuedraggable'

export default {
  data() {
    return {
      courses: [
        { title: 'Cloud Strategy', id: 1, detail: 'abc' },
        { title: 'Cloud Solutioning', id: 2, detail: '123' },
        { title: 'Cloud Delivery', id: 3, detail: 'abc' },
      ],
    };
  },
};
</script>

<template>
  <h1>Courses A</h1>
  <Draggable v-model="courses" group="course" @start="drag=true" @end="drag=false">
    <div v-for="course in courses" :key="course.id" class="course">
      <router-link :to="{ name: 'CourseDetail', params: { id: course.id}}">
        <h2>{{ course.title}}</h2>
      </router-link>
    </div>
  </Draggable>
</template>

<style>
  .course h2 {
    background: #f4f4f4;
    padding: 20px;
    border-radius: 10px;
    margin: 10px auto;
    max-width: 600px;
    cursor: pointer;
    color: #444;
  }

  .course h2:hover{
    background: #d3d3d3;
  }

  .course a {
    text-decoration: none;
  }
</style>
