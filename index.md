<!DOCTYPE html>
<head>
	<title>C10933043 陳鈊娜</title>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<!--------------------------------------這些是CSS設定--------------------------------------->
	<link rel="stylesheet" href="css/bootstrap.min.css"/>
	<link rel="stylesheet" href="css/font-awesome.min.css"/> <!--臉書等小圖示-->
	<link rel="stylesheet" href="css/slicknav.min.css"/>
	<link rel="stylesheet" href="css/fresco.css"/>
	<link rel="stylesheet" href="css/slick.css"/>
	<link rel="stylesheet" href="css/style.css"/>
	<!---------------------------------------------------------------------------------------->
</head>
<body>
	<!-- 執行預先載入的工作 -->
	<div id="preloader">
		<div class="loader"></div>
	</div>

	<!-- 標頭區塊 -->
	<header class="header">
		<div class="container-fluid">
			<div class="row">
				<div class="col-sm-4 col-md-3 order-2 order-sm-1">
					<div class="header__social">
						<a href="https://zh-tw.facebook.com/netflix"><i class="fa fa-facebook"></i></a>
						<a href="https://twitter.com/netflix"><i class="fa fa-twitter"></i></a>
						<a href="https://www.instagram.com/netflixtw/?hl=zh-tw"><i class="fa fa-instagram"></i></a>
					</div>
				</div>
				<div class="col-sm-4 col-md-6 order-1  order-md-2 text-center">
					<a href="./index.html" class="site-logo">
						<img src="img/logo.png" >
					</a>
				</div>
			</div>
			<nav class="main__menu">
				<ul class="nav__menu">
					<li><a href="./index.html" class="button">Home</a></li>
					<li><a href="./name.html" class="button">About</a></li>
					<li><a href="./habits.html" class="button">Hobbies</a></li>
					<li><a href="./final.html"class="button">Bucket List </a></li>
					<li><a href="./contact.html"class="button">Contact</a></li>
				</ul>
			</nav>
		</div>
	</header>
	<!-- 標頭區塊結束 -->

	<!-- 利用brootstrap的Hero Section讓圖片產生旋轉木馬效果 -->
	<section class="hero__section">
		<div class="hero-slider">
			<div class="slide-item">
				<a class="fresco" href="img/hero-slider/1.jpg" data-fresco-group="projects">
					<img src="img/hero-slider/1.jpg" >
				</a>
			</div>
			<div class="slide-item">
				<a class="fresco" href="img/hero-slider/2.jpg" data-fresco-group="projects">
					<img src="img/hero-slider/2.jpg" >
					</a>
			</div>
			<div class="slide-item">
				<a class="fresco" href="img/hero-slider/3.jpg" data-fresco-group="projects">
					<img src="img/hero-slider/3.jpg" >
				</a>	
			</div>
			<div class="slide-item">
				<a class="fresco" href="img/hero-slider/4.jpg" data-fresco-group="projects">
					<img src="img/hero-slider/4.jpg" >
				</a>	
			</div>
			<div class="slide-item">
				<a class="fresco" href="img/hero-slider/5.jpg" data-fresco-group="projects">
					<img src="img/hero-slider/5.jpg" >
				</a>	
			</div>
			<div class="slide-item">
				<a class="fresco" href="img/hero-slider/6.jpg" data-fresco-group="projects">
					<img src="img/hero-slider/6.jpg" >
				</a>	
			</div>
			<div class="slide-item">
				<a class="fresco" href="img/hero-slider/7.jpg" data-fresco-group="projects">
					<img src="img/hero-slider/7.jpg" >
				</a>	
			</div>
		</div>
		<div class="hero-text-slider">
			<div class="text-item">
				<h2>Emily in Paris</h2>
				<p>You live to work, we work to live. </p>
			</div>
			<div class="text-item">
				<h2>The Queen's Gambit</h2>
				<p>Intuition can't be found in books.</p>
			</div>
			<div class="text-item">
				<h2>The Umbrella Academy</h2>
				<p>Maybe your appetite is disproportionate to the size of your abilities.</p>
			</div>
			<div class="text-item">
				<h2>Designated Survivor</h2>
				<p>There are times when we make history, and there are times when history makes us.</p>
			</div>
			<div class="text-item">
				<h2>Dash & Lily</h2>
				<p>If you really care about her, you need to go to her as you.</p>
			</div>
			<div class="text-item">
				<h2>YOU</h2>
				<p>I'm not an option, I'm the chosen one.</p>
			</div>
			<div class="text-item">
				<h2>Black Mirror</h2>
				<p>I never expected to live in the future, but I am in the future now.</p>
			</div>
		</div>
	</section>
	<!-- 圖片旋轉效果結束 -->

	<!-- 頁尾區塊 -->
	<footer class="footer__section">	
		<div class="container">	
			<div class="footer__copyright__text">
				<Video autoplay controls>
    			<source src="music/04.mp3" />
			    </Video>
				<p>Copyright &copy; <script>document.write(new Date().getFullYear());</script> All rights reserved | This template is made with <em class="fa fa-heart" aria-hidden="true"></em> by<a href="mailto:c10933043@gapps.uch.edu.tw" target="_blank"> C10933043 Regina C</a></p>
			</div>
		</div>
	</footer>
	<!-- 頁尾區塊結束-->

	<!--====== Javascripts & Jquery ======-->
	<script src="js/vendor/jquery-3.2.1.min.js"></script>
	<script src="js/jquery.slicknav.min.js"></script>
	<script src="js/slick.min.js"></script>
	<script src="js/fresco.min.js"></script>
	<script src="js/main.js"></script>
	<script>
		$(document).ready(function() {
    
  		var audio  = new Audio('https://s3-us-west-2.amazonaws.com/s.cdpn.io/242518/click.mp3');
  		var audio2 = new Audio('https://s3-us-west-2.amazonaws.com/s.cdpn.io/242518/clickUp.mp3')

	    $(".button").mousedown(function() {
			audio2.load();
			audio2.play();
	    });

		$(".button").mouseup(function() {
			audio.load();
			audio.play();
			});
	    });
	</script>
	</body>
</html>
