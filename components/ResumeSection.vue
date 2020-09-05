<template>
  <section class="resume-section spad" :class="{'with-bg': withBackground}">
    <div class="container-fluid">
      <div class="row">
        <div class="col-xl-7 offset-xl-2">
          <div class="section-title">
            <h2>{{ title }}</h2>
          </div>
          <ul class="resume-list">
            <li v-for="item in items" :key="item.period">
              <h2>{{ item.period }}</h2>
              <h3>{{ item.workplace }}</h3>
              <h4>{{ item.occupation }}</h4>
              <p>{{ item.description }}</p>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  props: {
    title: String,
    items: Array,
    withBackground: Boolean,
  },
};
</script>
