<template>
  <div id="preloder">
      <div class="loader"></div>
    </div>
</template>

<script>
export default {
  mounted() {
    $(window).on('load', function() {
      $(".loader").fadeOut();
      $("#preloder").fadeOut("slow");
    });
  }
}
</script>
