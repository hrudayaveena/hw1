# hw1
<!DOCTYPE html>
<html>
<head>

	<title>hrudayaveena</title>

<link href='https://fonts.googleapis.com/css?family=Raleway:400,500,600,700,800,900,300,200,100' rel='stylesheet' type='text/css'>

	<style>

	

		/*the sky*/

/*transition from dawn to dusk*/

body {
  height: 100%;
  -webkit-animation-name: flash;
  -webkit-animation-duration: 5s ;

  background:linear-gradient(95deg,#E06E54,#FFFA67);/*http://codepen.io/team/css-tricks/pen/ZGYZBx*/
}


  
  @-webkit-keyframes flash {
  0% {
    background: linear-gradient(95deg,#85F9FF,#D8EDF2);
 
  }
  100% {
    background: linear-gradient(95deg,#E06E54,#FFFA67);
    
  }
}
/*clouds animation*/
#cloudsimage{
		margin:0 auto;
		width:960px;
		height:200px;
		background-image: url(images/clouds.png);
		/*animation of cloud-codepen-http://codepen.io/rachelcope/pen/YPzZrg*/
			animation: slideOver 8s infinite Alternate-reverse both;
  -webkit-animation: slideOver 8s infinite Alternate-reverse both;
	}
	@-webkit-keyframes slideOver {
  0% {
    opacity: 0;
    transform: translateX(-50px);
    -webkit-transform: translateX(-50px);
  }

  20% {
    opacity: 1;
  }
  
  90% {
    opacity: 1;
  }
  
  100% {
    opacity: 0;
    transform: translateX(200px);
    -webkit-transform: translateX(200px);
  }
}
/*placement of grass*/
		#grassimage{
			margin:0 auto;
			width:960px;
			height:100px;
			top:200px;
			position:relative;
			background-image: url(images/grass.png);/*png credits:RVA CHAKRAVARTHY*/;
		}

	/*container green for grass as navigation bar*/		
		
#container{
	margin:0 auto;
	width:960px;
	height:180px;
	top:200px;
	position:relative;
	background-color: #558C03;

	display:flex;
	justify-content:center;
	align-items:center;

}
a{
	text-decoration: none;
	display:block;
	width:150px;
	height:40px;
	background-color:#558C03 ;
	color:pink;
	font-size: 18px;
	font-family:'Raleway';
	text-align:center;
	display: block;

	transition:all 1s;
	
}
	a:hover /*hovering for the names on the navigation bar when you click on it*/

{
	transition:all 1s;
	background-color:#94BF54;
	height:180px;
	width:150px;
	color:blue;

/*transition of text colour*/
}


	
.intro{ /*css for "about me"*/

		margin:0 auto;
		
		top:230px;
		position:absolute;
		left:490px;
		float:left;
		text-align:center;
		z-index: 1;
		font-family:'Raleway';
		
		font-size:14px;
		
		-webkit-animation-name:sunset; /*animations for "about me"*/
		-webkit-animation-direction:normal;
		-webkit-animation-duration:3s;
		  }
		  @-webkit-keyframes sunset{
		  	0%{
		  		bottom:0;
		  		top:0px;
		  	}
		  	
		 100%{
		 
		 	top:230px;
		 }

		  }
}

		

	</style>
</head>
<body>

<div id="cloudsimage"></div>
<div class="intro">
<p>I am Hrudaya veena.</p>
<p>I love to travel.</p>
<p>Every little thing around me inspires me,
<p>I love to observe such small details and capture those</p> 
<p>amazing things through art and design.</p>
</div>
<div id="grassimage"></div>
<div id="container">
     <a href="index.html">home</a>
	<a href="about.html"><span style="color:yellow;"> about</a>
	<a href="photography.html"> photography</a>
	<a href="illustrations.html">illustrations</a>
	<a href="design.html">design</a>
	<a href="contact.html">contact</a>
	<a href="resume.html">resume</a>
</div>

 
</body>
</html>
