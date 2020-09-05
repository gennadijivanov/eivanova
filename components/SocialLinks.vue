<template>
  <div class="social-section">
    <div class="container-fluid">
      <div class="row">
        <div class="col-xl-10 offset-xl-1">
          <div class="social-link-warp">
            <div class="social-links">
              <!-- <a href>
                <i class="fa fa-pinterest"></i>
              </a>
              <a href>
                <i class="fa fa-linkedin"></i>
              </a> -->
              <a href="https://www.instagram.com/elena.ivanova.rielter/" target="__blank">
                <i class="fa fa-instagram"></i>
              </a>
              <a href="https://www.facebook.com/profile.php?id=100001570811983" target="__blank">
                <i class="fa fa-facebook"></i>
              </a>
              <!-- <a href>
                <i class="fa fa-twitter"></i>
              </a> -->
            </div>
            <h2 class="hidden-md hidden-sm">Социальные сети</h2>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.social-links a {
	-webkit-transition: all 0.3s;
	-o-transition: all 0.3s;
	transition: all 0.3s;
}


/*---------------------
	Social section
-----------------------*/
.social-section {
	background: #f9f9f9;
	padding: 80px 0;
}

.social-section .social-links {
	display: inline-block;
	background: #f9f9f9;
	position: relative;
	z-index: 5;
}

.social-section .social-links a {
	color: #484848;
	font-size: 36px;
	margin-right: 40px;
}

.social-section .social-link-warp {
	position: relative;
}

.social-section .social-link-warp h2 {
	display: inline-block;
	float: right;
	font-weight: 400;
	padding-left: 30px;
	background: #f9f9f9;
	position: relative;
	z-index: 5;
}

.social-section .social-link-warp:after {
	position: absolute;
	content: '';
	width: 50%;
	height: 2px;
	left: 23%;
	top: 50%;
	margin-top: 1px;
	background: #cbcbcb;
}

/* Tablet :768px. */
@media only screen and (min-width: 768px) and (max-width: 991px) {
	.hidden-md {
		display: none !important;
	}
	.social-section .social-links {
		display: block;
		text-align: center;
	}
	.social-link-warp:after {
		display: none;
	}
}

/* Large Mobile :480px. */
@media only screen and (max-width: 767px) {
	.hidden-md {
		display: none !important;
	}
	.social-section .social-links {
		display: block;
		text-align: center;
	}
}

/* small Mobile :320px. */
@media only screen and (max-width: 479px) {
	.social-section .social-links a {
		margin-right: 30px;
	}
}


</style>
