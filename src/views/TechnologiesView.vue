<script>
export default {
  data() {
    return {
      technologies: [
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
      <div v-for="tech in technologies" class="mb-10 item">
        <span class="tech-d">{{ tech.exp }} Year(s) Experience</span>
        <span class="tech">{{ tech.name }}</span>
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
.tech {
  font-size: 36px;
}
.tech-d{
  font-size: 16px;
  margin-right: 5px;
}
@media only screen and (max-width: 1000px) {
  .item {
    display: flex;
    flex-direction: column-reverse;
  }
  .tech {
    font-size: 16px;
  }
  .tech-d {
    font-size: 12px;
  }
}
</style>
