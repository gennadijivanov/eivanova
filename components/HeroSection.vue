<template>
  <section class="hero-section spad">
    <div class="container-fluid">
      <div class="row">
        <div class="col-xl-10 offset-xl-1">
          <div class="row">
            <div class="col-lg-6">
              <div class="hero-text">
                <h2>Елена Иванова</h2>
                <p>Я - риелтор с живым и пытливым умом. Очень умная, красивая и коммуникабельная. И люблю котиков.</p>
              </div>
              <div class="hero-info">
                <h2>Общая информация</h2>
                <ul>
                  <li>
                    <span>Дата рождения</span>24 августа 1982
                  </li>
                  <li>
                    <span>Адрес</span>Москва
                  </li>
                  <li>
                    <span>E-mail</span>shee@bk.ru
                  </li>
                  <li>
                    <span>Телефон</span>+7(926)622-48-22
                  </li>
                </ul>
              </div>
            </div>
            <div class="col-lg-6">
              <figure class="hero-image">
                <img src="img/hero.jpg" alt="5" />
              </figure>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
/*---------------------
	Hero section
-----------------------*/
.hero-section {
	background: #f2f7f8;
}

.hero-text {
	margin-bottom: 80px;
}

.hero-text h2 {
	font-size: 170px;
	line-height: normal;
	margin-bottom: 20px;
}

.hero-text p {
	font-size: 33px;
	line-height: 1.3;
}

.hero-image {
	padding-top: 70px;
}

.hero-info h2 {
	margin-bottom: 30px;
}

.hero-info ul {
	list-style: none;
}

.hero-info ul li {
	font-size: 24px;
	color: #808181;
	margin-bottom: 15px;
}

.hero-info ul li span {
	color: #40424a;
	display: inline-block;
	min-width: 220px;
}

.hero-info ul li:last-child {
	margin-bottom: 0;
}

@media only screen and (max-width: 1600px) {
	.hero-text h2 {
		font-size: 120px;
	}
}

@media only screen and (max-width: 1366px) and (min-width: 1200px) {
  .container-warp {
		min-width: 80%;
		margin-left: 10%;
	}
	.hero-info ul li span {
		min-width: 180px;
	}
}

/* Tablet :768px. */
@media only screen and (min-width: 768px) and (max-width: 991px) {
	.hero-info ul li {
		margin-bottom: 30px;
	}
	.hero-info ul li span {
		display: block;
	}
}

/* Large Mobile :480px. */
@media only screen and (max-width: 767px) {
	.hero-text h2 {
		font-size: 80px;
	}
}

/* small Mobile :320px. */
@media only screen and (max-width: 479px) {
	.hero-text h2 {
		font-size: 50px;
	}
	.hero-info ul li {
		font-size: 18px;
	}
	.hero-info ul li span {
		display: block;
	}
}

</style>
