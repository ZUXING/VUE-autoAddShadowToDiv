<template>
	<div :style='{width:fullWidth+"px",height:fullHeight+"px"}'>
		<div class="content" :style='{width:width+"px",height:height+"px",lineHeight:height+"px"}'>{{content}}</div>
		<div class='shadow' :style='{width:width+"px",height:height+"px",top:shifting+"px",left:shifting+"px"}'></div>
	</div>
</template>

<script>
export default {
	props:["content","width","height","shifting","selected"],
	/*data(){
		let fullWidth=parseInt(width)+parseInt(shifting)
		let fullHeight=parseInt(height)+parseInt(shifting)
		return{
			fullWidth,
			fullHeight
		}
	}*/
}
</script>

<style scoped>
	div{
		text-align: center;
		position: relative;
	}
	div.content{
		background-color: #FFF;
		border: 2px solid #333;
		position: absolute;
		z-index: 2;
	}
	div.shadow{
		background-image: url(./bgp.png);
		border: 2px solid #333;
		position: absolute;
		z-index: 1;
	}
	
	div.selected{
		color: #FFF;
		background-color: #ff6100;
	}
	div.box-content *{vertical-align: top;}
</style>
