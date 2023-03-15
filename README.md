<!DOCTYPE html>
<html>
	<head>
	<title>ScalingCards and More</title>
	<style>
	/*For Every P In document*/
	p::first-letter {color: #EF4C10; font-family: sans-serif;}
	/*Below is the color of the header (and then the text for the header)*/
	header {background-color: #56a1a9; margin: auto; width: 50%; border-radius: 10px; color: white; border: 1px solid purple; letter-spacing: 5px; overflow: hidden;}
	.TopParagraph {text-align: center;}
     nav {display: flex; justify-content: center;}
	 /*Below Displays None Unless You Hover THen Disengaes Display: none*/
	.navagationbar1 .dropdownlist1 {display: none;}
	.navagationbar1:hover .dropdownlist1 {display: block; border: 1px solid red; border-radius: 10px; position: absolute;}
	/*Drop Down Menu Links That are Under .dropdownlist*/
	.dropdownlist1  a {background-color: lightblue; text-align: center; overflow: hidden;}
	/*Below Changes When you Hover over the buttons on the Drop Down Menu*/
	.navagationbar1 .dropdownlist1 a:hover {background-color: yellow; color: Green;}
	/*Below Affects The Text of The drop down menu*/
	.navagationbar1 .dropdownlist1  a {text-decoration: none; color: white; display: block; max-width: 100px; border-radius: 5px;}
	/*Below is the color of the nav buttions*/
	.navbuttion1 {background-color: #B8FF00; color: white; border: none; border-radius: 5px; width: 100px;}
	footer {background-color: yellow; border: 1px solid purple; border-radius: 1px; margin: auto; width: 50%; text-align: center; display: block; overflow: hidden; z-index: -1}
	body {background: red url('data:image/png;base64,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') repeat-y fixed center center;}
	/*Section of Document Going to Serve as Main Body*/
	.Section {border: 0px solid blue; margin: auto; width: 80%; background: LightGreen; overflow: hidden; float: left;}
	.Section > p {text-align: center;}
	#rocket {border: 1px dashed navy;}
	#sidebar {background-color: #B935CA; margin: 0 auto; width: 10%; overflow: hidden; border-radius: 10px; border: 0px solid red; float: left;}
	#mainbody {background-color: orange; margin: 0 auto; width: 50%;}
	</style>
	</head>
	<body>
	<center>
	<audio controls loop autoplay>
		<source src="https://file-examples-com.github.io/uploads/2017/11/file_example_MP3_700KB.mp3" type="audio/mpeg">
	</audio>
	</center>
	<header>
		<p class = "TopParagraph">Welcome to My Site These are my Interests<p>
	</header>
	<nav>
		<div class="navagationbar1">
			<button class="navbuttion1">The Stuff I DO</button>
			<div class="dropdownlist1">
				<a href="https://www.youtube.com/watch?v=Z259mjdP-sQ" target="_blank">Throwing Cards</a>
				<a href="https://www.google.com/" target = "_blank" class = "dropdownmenuitems1">aaa</a>
				<a href="https://www.google.com/" target = "_blank">LINK3</a>
				<a href="https://www.google.com/" target = "_blank">LINK4</a>
				<a href="https://www.google.com/" target = "_blank">LINK5</a>
				<a href="https://www.google.com/" target = "_blank">Link6</a>
				<a href="https://www.google.com/" target = "_blank">Link7</a>
			</div>
		</div>
	</nav>
	<div id="mainbody">
	<aside id = "sidebar">
		<p>DRAGONBALLZ</p>
	</aside>
	<section class = "Section">
		<p>Video Imbed Here</p>
		<hr>
		<iframe src="https://www.youtube.com/embed/Ws7GtQGUHQU" id = "rocket"></iframe>
	</section>
	</div>
	<footer class = "CopyRight">
		<p>CopyRight Brett Thanks to W3Schools, canva.com for easy color wheel</p>
	</footer>
	</body>
</html>
