<template lang="pug">
header.header-section
  .container-fluid
    .row
      .col-md-4
        //- .site-logo
        //-   h2
        //-     a(href="#") Civic
        //-   p Enhance your online presence
      .col-md-8.text-md-right.header-buttons
        a.site-btn(href="#") Скачать резюме
        a.site-btn(href="#") Напишите мне
</template>

<style scoped>
/*---------------------
	Header section
-----------------------*/
.header-section {
	padding: 50px 40px;
	background: #f2f7f8;
}

.site-logo h2 {
	font-size: 36px;
}

.site-logo h2 a {
	color: #40424a;
}

.site-logo p {
	font-size: 14px;
	line-height: normal;
}

.header-buttons a {
	margin-top: 15px;
}

	/* Large Mobile :480px. */
@media only screen and (max-width: 767px) {
	.header-section {
		padding: 50px 0;
	}
}

</style>
