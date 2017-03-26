# world-maps
Traveling around the wolrd with SVG maps

[Visited U.S.A. States](https://dgrmunch.github.io/world-maps/usamap.html)

{::nomarkdown}

 <!DOCTYPE html>
<html>
<head>
	<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>
	<script type="text/javascript" src="http://ariutta.github.io/svg-pan-zoom/dist/svg-pan-zoom.min.js"></script>
	<script type="text/javascript">
	
	$(document).ready(function(){
		var svgElement = document.querySelector('#mapsvg').getSVGDocument().querySelector('#world-maps');
		var panZoomTiger = svgPanZoom(svgElement);
	});
	</script>
</head>
<body>
	
	<style>
	html, body { 
		margin:0; 
		padding:0; 
		overflow:hidden 
	}
	
	#mapsvg{ 
		position:fixed;
		top:0; 
		bottom:0; 
		left:0; 
		right:0; 
		width: 100%;
		height: 100%;
		background-color: lightblue;
		
	}
	
	#topbar{
		position: fixed;
		background-color: black;
		width: 100%;
		height: 20px;
		color: white;
		text-align: right;
		z-index: 100;
	}
	
	#pan-zoom{
		display:none;
		position: fixed;
		top: 0;
		left: 0;
		z-index: 200;
		margin: 10px;
		border: 1px solid white;
		width: 20px;
		height: 20px;
		text-align: center;
		background-color: lightseagreen;
	}
	
	</style>
	
	<div id="pan-zoom" class="svg-pan-zoom_viewport">+</div>
	<object id="mapsvg" data="usaTerritories.svg" type="image/svg+xml"></object>


 
</body>
</html> 

{:/}