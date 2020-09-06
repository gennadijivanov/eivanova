<template lang="pug">
section.resume-section.spad(:class="{'with-bg': withBackground}")
  .container-fluid
    .row
      .col-xl-7.offset-xl-2
        .section-title
          h2 {{ title }}
        ul.resume-list
          li(v-for="item in items" :key="item.period")
            h2 {{ item.period }}
            h3 {{ item.workplace }}
            h4 {{ item.occupation }}
            p {{ item.description }}
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

<style scoped>

/*---------------------
	Resume section
----------------------*/
.resume-section.with-bg {
	background-image: url(/img/resume-bg.jpg);
	background-repeat: no-repeat;
	background-size: cover;
}

.resume-list {
	list-style: none;
	margin-left: 60px;
	padding-left: 110px;
	border-left: 2px solid #40424a;
}

.resume-list li {
	margin-bottom: 120px;
	position: relative;
}

.resume-list li:last-child {
	margin-bottom: 0;
}

.resume-list li:after {
	position: absolute;
	content: '';
	width: 15px;
	height: 15px;
	border: 2px solid #40424a;
	border-radius: 50px;
	background: #cacaca;
	top: 30px;
	left: -118px;
}

.resume-list h2 {
	font-size: 72px;
	margin-bottom: 10px;
}

.resume-list h4 {
	font-size: 16px;
	text-transform: uppercase;
	color: #808181;
	margin-top: 10px;
	margin-bottom: 45px;
}

.resume-list p {
	margin-bottom: 0;
}

/* Large Mobile :480px. */
@media only screen and (max-width: 767px) {
	.resume-list {
		margin-left: 0;
		padding-left: 0;
		border-left: none;
	}
}

/* small Mobile :320px. */
@media only screen and (max-width: 479px) {
	.resume-list h2 {
		font-size: 50px;
	}
}


</style>
