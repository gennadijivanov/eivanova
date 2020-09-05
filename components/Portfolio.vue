<template>
  <section class="portfolio-section spad pb-0">
      <div class="container-fluid">
        <div class="row">
          <div class="col-xl-4 col-md-8 offset-xl-2">
            <div class="section-title">
              <h2>Portfolio</h2>
            </div>
          </div>
          <div class="col-md-4 text-md-right">
            <a href="#" class="site-btn mb-5">See All Portfolio</a>
          </div>
        </div>
        <div class="portfolio-warp">
          <div class="row">
            <div class="col-xl-3 col-lg-6 col-md-6">
              <div class="portfolio-item">
                <a
                  href="img/portfolio/1.jpg"
                  class="set-bg port-pic"
                  data-setbg="img/portfolio/1.jpg"
                ></a>
                <h2>Brand Campaign</h2>
                <p>Graphic design</p>
              </div>
            </div>
            <div class="col-xl-3 col-lg-6 col-md-6">
              <div class="portfolio-item">
                <a
                  href="img/portfolio/2.jpg"
                  class="set-bg port-pic"
                  data-setbg="img/portfolio/2.jpg"
                ></a>
                <h2>A Corporate Identity</h2>
                <p>Graphic design</p>
              </div>
            </div>
            <div class="col-xl-3 col-lg-6 col-md-6">
              <div class="portfolio-item">
                <a
                  href="img/portfolio/3.jpg"
                  class="set-bg port-pic"
                  data-setbg="img/portfolio/3.jpg"
                ></a>
                <h2>Web Design Website</h2>
                <p>Graphic design</p>
              </div>
            </div>
            <div class="col-xl-3 col-lg-6 col-md-6">
              <div class="portfolio-item">
                <a
                  href="img/portfolio/4.jpg"
                  class="set-bg port-pic"
                  data-setbg="img/portfolio/4.jpg"
                ></a>
                <h2>Logo design</h2>
                <p>Graphic design</p>
              </div>
            </div>
          </div>
        </div>
      </div>

      <script src="js/magnific-popup.min.js"></script>
    </section>
</template>

<script>
export default {
  mounted () {
    $('.portfolio-item .port-pic').magnificPopup({
      type: 'image',
      mainClass: 'img-popup-warp',
      removalDelay: 500,
    });
  }
}
</script>

<style scoped>
/* Image Popup */
.img-popup-warp .mfp-content,
.img-popup-warp.mfp-ready.mfp-removing .mfp-content {
	opacity: 0;
	-webkit-transform: scale(0.8);
	-ms-transform: scale(0.8);
	transform: scale(0.8);
	-webkit-transition: all 0.4s;
	-o-transition: all 0.4s;
	transition: all 0.4s;
}

.img-popup-warp.mfp-ready .mfp-content {
	opacity: 1;
	-webkit-transform: scale(1);
	-ms-transform: scale(1);
	transform: scale(1);
}


/*---------------------
	Portfolio section
----------------------*/
.portfolio-warp {
	padding: 0 60px;
}

.portfolio-item h2 {
	font-size: 24px;
	margin-bottom: 5px;
}

.portfolio-item p {
	font-size: 14px;
	margin-bottom: 0;
}

.portfolio-item .port-pic {
	margin-bottom: 30px;
	display: block;
	height: 480px;
	background: #333;
	background-position: center center;
	background-size: cover;
	overflow: hidden;
	position: relative;
}

.portfolio-item .port-pic:after {
	position: absolute;
	content: '';
	left: 0;
	bottom: 0;
	width: 100%;
	height: 0;
	background: #000;
	opacity: 0;
	z-index: 2;
	-webkit-transition: all 0.4s cubic-bezier(0.55, 0.09, 0.68, 0.53) 0s;
	-o-transition: all 0.4s cubic-bezier(0.55, 0.09, 0.68, 0.53) 0s;
	transition: all 0.4s cubic-bezier(0.55, 0.09, 0.68, 0.53) 0s;
}

.portfolio-item:hover .port-pic:after {
	opacity: 0.8;
	height: 100%;
	top: 0;
}

@media only screen and (max-width: 1366px) and (min-width: 1200px) {
	.portfolio-item .port-pic {
		height: 310px;
	}
}

/* Medium screen : 992px. */
@media only screen and (min-width: 992px) and (max-width: 1199px) {
	.portfolio-warp {
		padding: 0;
	}

	.portfolio-item .port-pic {
		height: 310px;
	}
	.portfolio-item {
		margin-bottom: 30px;
	}
}

/* Tablet :768px. */
@media only screen and (min-width: 768px) and (max-width: 991px) {
	.portfolio-warp {
		padding: 0;
	}
	.portfolio-item {
		margin-bottom: 30px;
	}
}

/* Large Mobile :480px. */
@media only screen and (max-width: 767px) {
	.portfolio-warp {
		padding: 0;
	}
	.portfolio-item {
		margin-bottom: 30px;
	}
}

/* small Mobile :320px. */
@media only screen and (max-width: 479px) {
	.portfolio-item {
		margin-bottom: 30px;
	}
}


</style>
