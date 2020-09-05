<template>
  <section class="extra-section spad pb-0">
      <div class="container-fluid">
        <div class="row">
          <div class="col-xl-8 offset-xl-2">
            <div class="section-title">
              <h2>Дополнительно</h2>
            </div>

            <div class="row">
              <div class="col-lg-3 col-md-6 pt-5">
                <div class="fact-box trans">
                  <div class="fact-content">
                    <div class="circle-progress">
                      <div id="progress1" class="prog-circle"></div>
                      <div class="progress-info">
                        <h2>100%</h2>
                      </div>
                      <div class="prog-title">
                        <h3>Коммуникабельна</h3>
                        <p>Найду общий язык с бомжом и Папой Римским</p>
                      </div>
                    </div>
                  </div>
                </div>
              </div>

              <div class="col-lg-3 col-md-6 pt-5">
                <div class="fact-box trans">
                  <div class="fact-content">
                    <div class="circle-progress">
                      <div id="progress2" class="prog-circle"></div>
                      <div class="progress-info">
                        <h2>100%</h2>
                      </div>
                      <div class="prog-title">
                        <h3>Великолепна</h3>
                        <p>а ещё скромна</p>
                      </div>
                    </div>
                  </div>
                </div>
              </div>

              <div class="col-lg-3 col-md-6">
                <div class="fact-box">
                  <div class="fact-content">
                    <img src="img/icon/1-w.png" alt />
                    <h2>14</h2>
                    <p>Лет опыта</p>
                  </div>
                </div>
              </div>

              <div class="col-lg-3 col-md-6">
                <div class="fact-box">
                  <div class="fact-content">
                    <img src="img/icon/2-w.png" alt />
                    <h2>999</h2>
                    <p>Наград</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
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
