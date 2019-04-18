<template>
  <div class="hello">
    <div id="bgndVideo" class="player" data-property="{videoURL:'https://www.youtube.com/watch?v=a3ICNMQW7Ok',containment:'body', mute:false, startAt:0, opacity:1}">My video</div>
  </div>
</template>

<script>
/* eslint-disable */
export default {
  name: 'HelloWorld',

  props: {
    msg: String
  },

  data () {
    return {
      player: null,
    }
  },

  mounted () {
    this.player = $("#bgndVideo").YTPlayer()

    setTimeout(() => {
      this.player.YTPlayer()
    }, 1000)
  },
}
</script>