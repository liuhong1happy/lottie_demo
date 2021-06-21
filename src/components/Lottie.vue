<template>
    <lottie-player
    autoplay
    controls
    loop
    mode="normal"
    src="https://assets5.lottiefiles.com/packages/lf20_8q8dz850.json"
    ></lottie-player>
</template>

<script>
  import "@lottiefiles/lottie-player";
  export default {
    props: {
      options: {
        type: Object,
        required: true
      },
      height: Number,
      width: Number,
    },
    // components: {
    //     LottiePlayer
    // },
    data () {
      return {
        style: {
            width: '100%',
            height: '100%'
        }
      }
    },
    // mounted () {
    //   this.anim = lottie.loadAnimation({
    //       container: this.$refs.lavContainer,
    //       renderer: 'svg',
    //       loop: true,
    //       autoplay: true,
    //       animationData: this.options.animationData,
    //       path: this.options.path,
    //     }
    //   );
    //   this.anim.play();
    //   this.anim.addEventListener('complete', (res)=> {
    //       console.log('complete', res)
    //   })
    //   this.anim.addEventListener('enterFrame', ()=> {
    //     //   console.log('enterFrame', res)
    //   })
    //   this.$emit('animCreated', this.anim)
    // }
  }
</script>