<template>
  <div class="container">
    <section class="vote">
      <h3 class="give-your-vote">
        Silahkan berikan penilaian anda terhadap pelayanan kami
      </h3>

      <div class="emoticons">
        <Vote />
      </div>
    </section>
    <section class="finish">
      <h4>Terima kasih telah memberikan penilaian anda</h4>
    </section>
  </div>
</template>
<script>
import Vote from "@/components/Vote.vue";
export default {
    name: "home",
    components: {Vote},
    methods:{
      vote(){
        this.show = true;
      }
    }
};
</script>
<style type="text/css">

  .fade-enter-active, .fade-leave-active{
    transition: opacity 1s;
  }
  .fade-enter, .fade-leave-to{
    opacity: 0;
  }
  .container{
    display: flex;
    flex-wrap: wrap;
    height: 100vh;
    align-items: center;
  }
  section{
    width: 100%;
  }
.emoticons{
  display: flex;
  justify-content: center;
}
.finish{
  position: absolute;
  bottom: 20px;
}

.give-your-vote{
  font-size: 21px;
}
</style>

