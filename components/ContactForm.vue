<template>
  <section class="contact-section spad">
      <div class="container-fluid">
        <div class="row">
          <div class="col-xl-8 offset-xl-2">
            <div class="section-title">
              <h2>Contact Me</h2>
            </div>
            <form class="contact-form">
              <div class="row">
                <div class="col-md-6">
                  <input type="text" placeholder="Name" />
                </div>
                <div class="col-md-6">
                  <input type="text" placeholder="E-mail" />
                </div>
                <div class="col-md-12">
                  <input type="text" placeholder="Subject" />
                  <textarea placeholder="Message"></textarea>
                </div>
              </div>
              <div class="text-md-right">
                <button class="site-btn">Send message</button>
              </div>
            </form>
          </div>
        </div>
      </div>
    </section>
</template>

<style scoped>

/*---------------------
	Contact section
-----------------------*/
.contact-form {
	display: block;
	width: 100%;
}

.contact-form input {
	background-color: transparent;
	padding-left: 25px;
	height: 60px;
	width: 100%;
	border: none;
	border-bottom: 2px solid #cacaca;
	margin-bottom: 30px;
	font-size: 13px;
}

.contact-form textarea {
	padding-left: 25px;
	height: 200px;
	width: 100%;
	border: none;
	border-bottom: 2px solid #cacaca;
	margin-bottom: 30px;
	font-size: 13px;
	background-color: transparent;
}

.contact-form ::-webkit-input-placeholder {
	font-style: italic;
}

.contact-form :-ms-input-placeholder {
	font-style: italic;
}

.contact-form ::-ms-input-placeholder {
	font-style: italic;
}

.contact-form ::placeholder {
	font-style: italic;
}


</style>
