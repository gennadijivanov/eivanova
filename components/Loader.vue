<template lang="pug">
.fader
  .loader
</template>

<script>
export default {
  mounted() {
    $(window).on('load', function() {
      $(".loader").fadeOut();
      $(".fader").fadeOut("slow");
    });
  }
}
</script>

<style scoped>
/* Preloder */
.fader {
	position: fixed;
	width: 100%;
	height: 100%;
	top: 0;
	left: 0;
	z-index: 999999;
	background: #fff;
}

.loader {
	width: 30px;
	height: 30px;
	border: 3px solid #000;
	position: absolute;
	top: 50%;
	left: 50%;
	margin-top: -13px;
	margin-left: -13px;
	border-radius: 60px;
	border-left-color: transparent;
	animation: loader 0.8s linear infinite;
	-webkit-animation: loader 0.8s linear infinite;
}

@keyframes loader {
	0% {
		-webkit-transform: rotate(0deg);
		        transform: rotate(0deg);
	}
	50% {
		-webkit-transform: rotate(180deg);
		        transform: rotate(180deg);
	}
	100% {
		-webkit-transform: rotate(360deg);
		        transform: rotate(360deg);
	}
}

@-webkit-keyframes loader {
	0% {
		-webkit-transform: rotate(0deg);
	}
	50% {
		-webkit-transform: rotate(180deg);
	}
	100% {
		-webkit-transform: rotate(360deg);
	}
}
</style>
