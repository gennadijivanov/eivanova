<template lang="pug">
section.extra-section.spad.pb-0
  .container-fluid
    .row
      .col-xl-8.offset-xl-2
        .section-title
          h2 Дополнительно
        .row
          .col-lg-3.col-md-6.pt-5
            .fact-box.trans
              .fact-content
                .circle-progress
                  #progress1.prog-circle
                  .progress-info
                    h2 100%
                  .prog-title
                    h3 Коммуникабельна
                    p Найду общий язык с бомжом и Папой Римским
          .col-lg-3.col-md-6.pt-5
            .fact-box.trans
              .fact-content
                .circle-progress
                  #progress2.prog-circle
                  .progress-info
                    h2 100%
                  .prog-title
                    h3 Великолепна
                    p а ещё скромна
          .col-lg-3.col-md-6
            .fact-box
              .fact-content
                img(src="img/icon/1-w.png" alt="")
                h2 14
                p Лет опыта
          .col-lg-3.col-md-6
            .fact-box
              .fact-content
                img(src="img/icon/2-w.png" alt="")
                h2 999
                p Наград
</template>

<script>
export default {
  mounted () {
    if($().circleProgress){

      //Set progress circle 1
      $("#progress1").circleProgress({
        value: 1,
        size: 175,
        thickness: 2,
        fill: "#40424a",
        emptyFill: "rgba(0, 0, 0, 0)"
      });
      //Set progress circle 2
      $("#progress2").circleProgress({
        value: 1,
        size: 175,
        thickness: 2,
        fill: "#40424a",
        emptyFill: "rgba(0, 0, 0, 0)"
      });
    }
  }
}
</script>

<style scoped>
.circle-progress {
	text-align: center;
	padding-top: 30px;
	display: inline-block;
}

.circle-progress .prog-circle {
	margin-bottom: -155px;
}

.circle-progress canvas {
	-webkit-transform: rotate(90deg);
	-ms-transform: rotate(90deg);
	transform: rotate(90deg);
}

.circle-progress .progress-info {
	background: #f2f7f8;
	width: 127px;
	height: 127px;
	border-radius: 150px;
	margin: 0 auto;
	padding-top: 45px;
}

.circle-progress .progress-info h2 {
	font-size: 36px;
	color: #40424a !important;
}

.circle-progress .prog-title {
	text-align: center;
	margin-top: 55px;
}

.circle-progress .prog-title h3 {
	font-size: 16px;
	text-transform: uppercase;
}

.circle-progress .prog-title p {
	font-size: 15px;
	color: #808181 !important;
}

/* Fact box */
.fact-box {
	height: 375px;
	display: table;
	width: 100%;
	background: #40424a;
}

.fact-box.trans {
	background-color: transparent;
}

.fact-box .fact-content {
	display: table-cell;
	vertical-align: middle;
	text-align: center;
}

.fact-box .fact-content img {
	width: 60px;
	margin-bottom: 30px;
}

.fact-box .fact-content h2 {
	font-size: 36px;
	color: #fff;
}

.fact-box .fact-content p {
	color: #fff;
	margin-bottom: 0;
}

/* Large Mobile :480px. */
@media only screen and (max-width: 767px) {
	.fact-box {
		margin-bottom: 30px;
	}
}

</style>
