<template>
<section class="review-section spad pb-0">
      <div class="container-fluid">
        <div class="row">
          <div class="col-xl-7 offset-xl-2">
            <div class="section-title">
              <h2>References</h2>
            </div>
            <div class="review-slider owl-carousel">
              <div class="single-review">
                <div class="qut">“</div>
                <p>Sit amet, consectetur adipiscing elit. Sed porttitor orci ut sapien scelerisque viverra. Sed trist ique justo nec mauris efficitur, ut lacinia elit dapibus. In egestas elit in dap ibus laoreet. Duis magna libero, fermentum ut facilisis id, pulvinar eget tortor. Vestibulum pelle ntesque tincidunt lorem, vitae euismod felis porttitor sed.</p>
                <h3>Robert G. Smith</h3>
                <h4>Manager, Company</h4>
              </div>
              <div class="single-review">
                <div class="qut">“</div>
                <p>Sit amet, consectetur adipiscing elit. Sed porttitor orci ut sapien scelerisque viverra. Sed trist ique justo nec mauris efficitur, ut lacinia elit dapibus. In egestas elit in dap ibus laoreet. Duis magna libero, fermentum ut facilisis id, pulvinar eget tortor. Vestibulum pelle ntesque tincidunt lorem, vitae euismod felis porttitor sed.</p>
                <h3>Robert G. Smith</h3>
                <h4>Manager, Company</h4>
              </div>
              <div class="single-review">
                <div class="qut">“</div>
                <p>Sit amet, consectetur adipiscing elit. Sed porttitor orci ut sapien scelerisque viverra. Sed trist ique justo nec mauris efficitur, ut lacinia elit dapibus. In egestas elit in dap ibus laoreet. Duis magna libero, fermentum ut facilisis id, pulvinar eget tortor. Vestibulum pelle ntesque tincidunt lorem, vitae euismod felis porttitor sed.</p>
                <h3>Robert G. Smith</h3>
                <h4>Manager, Company</h4>
              </div>
            </div>
          </div>
        </div>
      </div>

    <script src="js/owl.carousel.min.js"></script>

    </section>
</template>

<script>
export default {
  mounted (){
    $('.review-slider').owlCarousel({
      loop: true,
      nav: false,
      dots: true,
      items: 1,
      autoplay: true
    });
  }
}
</script>

<style scoped>

/*---------------------
	Review section
-----------------------*/
.review-slider {
	padding-left: 150px;
}

.review-slider .owl-dots {
	position: absolute;
	left: 50px;
	top: 70px;
}

.review-slider .owl-dots .owl-dot {
	width: 12px;
	height: 12px;
	border: 2px solid #40424a;
	border-radius: 50px;
	background: #cacaca;
	margin-bottom: 15px;
}

.review-slider .owl-dots .owl-dot.active {
	background: #40424a;
}

.single-review .qut {
	font-size: 120px;
	line-height: 0;
	color: #505259;
	margin-top: 60px;
}

.single-review p {
	margin-bottom: 40px;
}

.single-review h3 {
	font-size: 24px;
	margin-bottom: 10px;
}

.single-review h4 {
	font-size: 16px;
}

/* Large Mobile :480px. */
@media only screen and (max-width: 767px) {
	.review-slider {
		padding-left: 0;
	}
	.review-slider .owl-dots {
		position: relative;
		left: 0;
		top: 70px;
	}
	.review-slider .owl-dots .owl-dot {
		display: inline-block;
		margin-right: 15px;
	}
}



</style>
