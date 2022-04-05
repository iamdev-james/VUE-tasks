<template>
  <div>
    <div id='container' class='box'></div>
  </div>
</template>

<script>

</script>

<style>
.box {
  perspective: 350px;
  margin: auto;
	width:280px;
	height:280px;
	display:flex;
	align-items:center;
  overflow: hidden;
	justify-content:center;
	font-family: "Inconsolata", monospace;
	font-size: 28px;
	border:1px solid #c39f76;
	box-sizing:border-box;
}
#container:before {
  content: 'Hello World Hello World Hello World Hello World Hello World Hello World Hello World';
  text-align: center;
  width: 200px;
  transform: rotateX(60deg) translateY(170%);
  animation: scroll 10s linear infinite;
  line-height: 50px;
}
@keyframes scroll {
 from {
  transform: rotateX(65deg) translateY(160%);
 }
 to {
  transform: rotateX(65deg) translateY(-50%);
 }
}
</style>
