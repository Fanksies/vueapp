<template>
<div class="MainContainer">

  <div class="ParallaxContainer gradient">
   <div class="m-1">
     Maybe navbar
   </div>
    <div class="text-center">
      <h1 class="swag">MARM</h1>
      <p class="m-1 ">Front End Developer | Person | Thing</p>
    </div>
    <div class="m-1">
      Buttons to github, codepen, linkedin
    </div>
  </div>

  <div class="ContentContainer">
    <div class="Content">
      <h1>About</h1>
      <p>ʻO Lorem Ipsum kahi haʻahaʻa wale nō o ka paʻi a me keʻano o nāʻoihana. ʻO Lorem Ipsum ka 'ōlelo papahana maʻamau o kaʻoihana o ka makahiki 1500, i ka wā i lawe ai kekahi mea paʻi kiʻiʻole i keʻano o ka type a scrambled iā ia e hana i kahi puke kiko'ī. ʻAʻole i ola wale i kaʻelima mau kenekulia, akā,ʻo ka leleʻana hoʻi i nāʻano o ka lolouila, e hoʻololiʻoleʻia ana. Ua hoʻolahaʻia i nā makahiki 1960 me ka hoʻokuʻuʻana i nā pepa Letraset i loko o nā moʻolelo Lorem Ipsum, a me nā mea hou aku me ka polokalamu hoʻopuka pākī e like me Aldus PageMaker me nā papa o Lorem Ipsum.</p>
     </div>
  </div>

</div>

</template>

<script>
import AppLogo from '~/components/AppLogo.vue'

export default {
  components: {
    AppLogo
  }
}
</script>

<style>

html, body {
  /* font-family: Open Sans; */
  font-size: 18px;
  line-height: 28px;
  scroll-behavior: smooth;
  color: white;
  background: #333;
}

.swag {
  letter-spacing: -15px;
  font-family: Open Sans;
  font-size: 24vw;
  font-weight: 800;
  line-height: 200px;
}

.text-center {
  text-align: center;  
}

.MainContainer {
  perspective: 1px;
  transform-style: preserve-3d;
  height: 100vh;
  overflow-x: hidden;
  overflow-y: scroll;
}

.ContentContainer {
  position: relative;
  display: block;
  background-color: #333;
  z-index: 1;
}

.Content {
  max-width: 750px;
  margin: 0 auto;
  padding: 75px 0;
}

p {
  margin: 75px 0;
}

.m-1 {
  margin: .75rem 0;
}

.ParallaxContainer {
  display: flex;
  flex-direction: column;
  height: 100vh;
  justify-content: center;
  /* align-items: center;  */
  justify-content: space-between;
  position: relative;
  z-index: -1;
  transform: translateZ(-1px) scale(2);
}

@import url('https://fonts.googleapis.com/css?family=Open+Sans:400,800');

.gradient {
  background: linear-gradient(-45deg, #EE7752 , #E73C7E,  #23A6D5, #23D5AB);
	background-size: 400% 400%;
	-webkit-animation: Gradient 9s ease infinite;
	-moz-animation: Gradient 9s ease infinite;
	animation: Gradient 9s ease infinite;
}

@-webkit-keyframes Gradient {
	0% {
		background-position: 0% 50%
	}
	50% {
		background-position: 100% 50%
	}
	100% {
		background-position: 0% 50%
	}
}

@-moz-keyframes Gradient {
	0% {
		background-position: 0% 50%
	}
	50% {
		background-position: 100% 50%
	}
	100% {
		background-position: 0% 50%
	}
}

@keyframes Gradient {
	0% {
		background-position: 0% 50%
	}
	50% {
		background-position: 100% 50%
	}
	100% {
		background-position: 0% 50%
	}
}

</style>

