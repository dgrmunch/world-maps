# world-maps
Traveling around the wolrd with SVG maps

[Visited U.S.A. States](https://dgrmunch.github.io/world-maps/usamap.html)

{::nomarkdown}
	
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
	
	<object id="mapsvg" data="usaTerritories.svg" type="image/svg+xml"></object>


{:/}