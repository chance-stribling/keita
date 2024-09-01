<script>
export default {
  data() {
    return {
      projects: [
        {
          name: 'Laravel',
          exp: 2
        },
        {
          name: 'PHP',
          exp: 2
        },
        {
          name: 'React',
          exp: 1
        },
        {
          name: 'Swift UI',
          exp: 3
        },
        {
          name: 'Three JS',
          exp: 1
        },
        {
          name: 'Vue JS',
          exp: 3
        },
        {
          name: 'Wix',
          exp: 3
        },
        {
          name: 'WordPress',
          exp: 1
        }
      ]
    }
  }
}
</script>

<template>
  <div class="main">
    <div class="content">
      <div v-for="project in projects" class="mb-10 item">
        <span class="project">{{ project.name }}</span>
      </div>
    </div>
  </div>
</template>
<style scoped>
.main {
  display: flex;
  flex-direction: column;
  align-items: end;
  justify-content: end;
  height: 100%;
  padding: 2rem;
  color: white;
  overflow: hidden;
}
.content {
  display: flex;
  flex-direction: column;
  align-items: end;

  overflow: auto;
  -ms-overflow-style: none;
  overflow: -moz-scrollbars-none;
  scrollbar-width: none;
}
.content::-webkit-scrollbar {
  display: none; /* Safari and Chrome */
}
.project {
  font-size: 48px;
}
@media only screen and (max-width: 1000px) {
  .item {
    display: flex;
    flex-direction: column-reverse;
  }
  .project {
    font-size: 20px;
  }
}
</style>
