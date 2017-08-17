<% include includes/html-head.html %>
    <style>
        .desktop-screen {
            display: block;
        }
        
        .mobile-screen {
            display: none;
        }
        
        .feature-phone-container {
            margin-bottom: 0;
        }
        
        .voice-command-section {
            position: relative;
            padding-bottom: 50px;
            background: #02abb9;
            /* Old browsers */
            background: -moz-linear-gradient(top, #02abb9 0%, #ddeeef 100%);
            /* FF3.6-15 */
            background: -webkit-linear-gradient(top, #02abb9 0%, #ddeeef 100%);
            /* Chrome10-25,Safari5.1-6 */
            background: linear-gradient(to bottom, #02abb9 0%, #ddeeef 100%);
            /* W3C, IE10+, FF16+, Chrome26+, Opera12+, Safari7+ */
            filter: progid: DXImageTransform.Microsoft.gradient( startColorstr='#02abb9', endColorstr='#ddeeef', GradientType=0);
            /* IE6-9 */
        }
        
        .voice-command-section .voice-app {
            display: inline-block;
            margin: 0 30px 20px 0;
            width: 100px;
            position: relative;
        }
        

        
        .voice-command-section .voice-app:hover:before {
            content: "";
            top: -20px;
            left: -20px;
            background-color: rgba(255,255,255,1);
            width: 140px;
            height: 140px;
            border-radius: 100%;
            -webkit-animation-fill-mode: both;
            animation-fill-mode: both;
            position: absolute;
            opacity: 1;
            -webkit-animation: jumper 2.8s 0s ease-out infinite;
            animation: jumper 1s 0s ease-out infinite;
        }
        
        .voice-command-section .voice-app:hover:after {
            content: "";
            top: -20px;
            left: -20px;
            background-color: rgba(255,255,255,1);
            width: 140px;
            height: 140px;
            border-radius: 100%;
            -webkit-animation-fill-mode: both;
            animation-fill-mode: both;
            position: absolute;
            opacity: 1;
            -webkit-animation: jumper 2.8s 0s ease-out infinite;
            animation: jumper 1s 0s ease-out infinite;
        }
        
        .voice-command-section .voice-app img {
            width: 100%;
            position: relative;
            z-index: 2;
        }
        
        .voice-command-section .phone-screen {
            position: relative;
        }
        
        .voice-command-section .phone-screen .phone-bg {
            position: relative;
        }
        
        .voice-command-section .phone-screen .screen {
            display: none;
            position: absolute;
            left: 9px;
            top: 24px;
        }
        
        .voice {
            display: none;
            position: absolute;
            left: 29px;
            top: 30px;
        }

        
        .anim-container {
            position: absolute;
            left: 0;
            right: 0;
            bottom: 0;
            height: 100px;
        }
        
        .anim1,
        .anim2,
        .anim3,
        .anim4 {
            height: 100px;
            position: absolute;
            width: 100%;
            left: 0;
            bottom: 0;
        }
        /**/
        
        .anim1 {
            animation: animation1 3.3s infinite linear;
        }
        
        .anim2 {
            animation: animation1 2.8s infinite linear;
        }
        
        .anim3 {
            animation: animation1 4.8s infinite linear;
        }
        
        .anim4 {
            animation: animation1 1.8s infinite linear;
        }
        
        @keyframes animation1 {
            0% {
                background-position: 0 0;
            }
            100% {
                background-position: 455px 0;
            }
        }
        
        .anim1 {
            background: url('assets/images/feature-phone/wave-01.png') 0 0 repeat-x;
        }
        
        .anim2 {
            background: url('assets/images/feature-phone/wave-02.png') 80px 0 repeat-x;
        }
        
        .anim3 {
            background: url('assets/images/feature-phone/wave-03.png') 180px 0 repeat-x;
        }
        
        .anim4 {
            background: url('assets/images/feature-phone/wave-04.png') 300px 0 repeat-x;
        }
        
        @media(max-width:768px) {
            .about-me-container {
                margin: 0px 10px;
                width: auto;
            }
            .desktop-screen {
                display: none;
            }
            .mobile-screen {
                display: block;
            }
        }
        
        @-webkit-keyframes jumper {
            0% {
                opacity: 0;
                -webkit-transform: scale(0);
                -ms-transform: scale(0);
                transform: scale(0)
            }
            5% {
                opacity: 1
            }
            100% {
                -webkit-transform: scale(1);
                transform: scale(1);
                -ms-transform: scale(1);
                opacity: 0
            }
            @keyframes jumper {
                0% {
                    opacity: 0;
                    -webkit-transform: scale(0);
                    -ms-transform: scale(0);
                    transform: scale(0)
                }
                5% {
                    opacity: 1
                }
                100% {
                    -webkit-transform: scale(1);
                    transform: scale(1);
                    -ms-transform: scale(1);
                    opacity: 0
                }
            }
        }
        

        /*Yugandhara*/
		.language-support-section 
		{
			background: linear-gradient(to bottom, #29b8e5 0%, #ddeeef 100%);
		}
		
		.language-support-section .languages
		{
			padding-left:0px;
			margin-top:20%;
		}
		.language-support-section .languages li
		{
			display:inline-block;
			background:#fff;
			border-radius:100px;
			width:100px;
			height:100px;
			line-height:100px;
			text-align:center;
			color:#000;
			font-weight:bold;
			margin-right:41px;
			cursor:pointer;
		}
		
		.language-support-section .right-section h1
		{
			color:#fff !important;
		}
		
		.language-support-section .right-section p
		{
			color:#000 !important;
		}
		
		.language-support-section .left-section img
		{
			width: 100%;
			height: 474px;
			position: relative;
		}


		.language-support-section .demo1, .demo2, .demo3, .demo4
		{
			position: absolute;
			top: 10%;
			left: 44%;
			color: red;
			font-size: 20px;
		}
		
		/*snehal*/
		/* preloaded css*/

        .preloaded-apps-section .tabs-bg-color
        {
            background:#22262f;
            text-align:center;
            padding:18px 0px 10px 0px;
        }

        .preloaded-apps-section .preloaded-text p, .preloaded-apps-section .preloaded-text h3
        {
            color:#fff !important;
            
        }
        
        .preloaded-apps-section .preloaded-text p
        {
            font-size:22px !important;
        }
        .preloaded-apps-section .tab-content
        {
            display:block;
        }
         .preloaded-apps-section .nav-tabs
        {
            border-bottom:0px;
            margin-top:0px;
            margin-bottom:-12px;
        }
        .preloaded-apps-section .nav-tabs > li
        {
            display:inline-block !important;
            float:none !important;
            border:1px solid #fff ;
            background:#fff;
            border-radius:5px;
            cursor:pointer;
            width:10%;
            margin-right:7px;
            border-bottom:0px;
            border-bottom-right-radius:0px;
            border-bottom-left-radius:0px;

        }
       .preloaded-apps-section .tab-content .img-inner-wrapper h3, 
       .preloaded-apps-section 
       .tab-content .img-inner-wrapper p
        {
            color:#fff !important;
        }

        .preloaded-apps-section .tab-content .img-inner-wrapper h3
        {
            font-size:22px !important;
            font-weight:bold;
        }

        .preloaded-apps-section .tab-content .img-inner-wrapper p
        {
            font-size:18px;
        }

        .preloaded-apps-section .tab-content .img-inner-wrapper h3, .preloaded-apps-section .preloaded-text h3
        {
            margin-bottom:7px !important;
        }

       .preloaded-apps-section .tab-content
       {
            width:100%;
            background-color:#efefef;
            /*padding:40px;*/
            text-align:center;
            padding:0px;
       }


      .preloaded-apps-section .nav-tabs > li.active > a
        {
            font-weight:bold;
            color:#2f38b0 !important;
            background:none !important;
            border:0px !important;
            cursor:pointer;

        }

        .preloaded-apps-section .nav-tabs > li > a:hover
        {
            border-color:none !important;
            background:none !important;
            border:0px !important;
        }
        .preloaded-apps-section .preloaded-text
        {
            margin-bottom:30px;
        }

       .preloaded-apps-section .img-wrapper
        {
            position:relative;
        }

       .preloaded-apps-section .img-content-wrapper
        {
            position:absolute;
            top:20%;
            text-align:center;
            width:100%;
            left:4%;
        }

       .preloaded-apps-section img
        {
            width:100%;
        }

       .preloaded-apps-section .img-wrapper li
        {
            display:inline-block;
            vertical-align:top;
        }

        .preloaded-apps-section .img-inner-wrapper
        {
            max-width:400px;
            text-align:left;
        }

        .preloaded-apps-section .img-content-wrapper ul li:nth-child(2)
        {
            margin-left:10px;
        }

    </style>
    <% include includes/search-new-version.html %>
        <div id="wrap">
            <!-- Wrap Starts -->
            <div class="main-bg">
                <div class="header-container with-bg">
                    <div class="wrapMaxWidth">
                        <% include includes/site-header-new-version.html %>
                    </div>
                </div>
                <div class="header-top-space"></div>

                <div class="re-device-listing-wrap">

                    <div class="re-device-listing-container">

                        <% include includes/device-listing-menu-old-details.html %>

                            <div class="dl-banner" id="dl-banner1" style="display: block; cursor: pointer;" onclick="location.href=('pre-booking-1.html')">
                                <img class="desktop-screen" src="assets/images/device-detail/desktop-banner.png" style="width: 100%;">
                                <img class="mobile-screen" src="assets/images/device-detail/mobile-banner.png" style="width: 100%;">
                            </div>

                            <div class="feature-phone-container margin-top-10">
                                <div class="row">
                                    <div class="voice-command-section">
                                        <div class="row">
                                            <h1>Use voice assistance to control JioPhone</h1>
                                            <p>Lorem ispum lorme ispum....</p>
                                            <div class="col-sm-8 voice-command-apps">
                                                <div class="voice-app calling"><img src="assets/images/feature-phone/call01.png" alt=""></div>
                                                <div class="voice-app messaging"><img src="assets/images/feature-phone/sms01.png" alt=""></div>
                                                <div class="voice-app browsing"><img src="assets/images/feature-phone/video01.png" alt=""></div>
                                                <div class="voice-app messaging"><img src="assets/images/feature-phone/sms01.png" alt=""></div>
                                                <div class="voice-app browsing"><img src="assets/images/feature-phone/video01.png" alt=""></div>
                                            </div>                                            
                                            <div class="col-sm-4 phone-screen">
                                                <div class="phoneBg">
                                                    <img src="assets/images/feature-phone/voice-01-00.png" alt="">
                                                </div>
                                                <div class="screen screen-voice">
                                                    <div class="voice voice-off"><img src="assets/images/feature-phone/voice-01-01.png" alt=""></div>
                                                    <div class="voice voice-on"><img src="assets/images/feature-phone/voice-01-02.png" alt=""></div>
                                                    <div class="voice voice-success"><img src="assets/images/feature-phone/voice-01-03.png" alt=""></div>
                            
                                                </div>
                                                <div class="screen screen-text">
                                                    <div class="voice voice-off"><img src="assets/images/feature-phone/voice-01-01.png" alt=""></div>
                                                    <div class="voice voice-on"><img src="assets/images/feature-phone/voice-01-02.png" alt=""></div>
                                                    <div class="voice voice-success"><img src="assets/images/feature-phone/voice-01-03.png" alt=""></div>
                                                </div>
                                                <div class="screen screen-browsing">
                                                    <div class="voice voice-off"><img src="assets/images/feature-phone/voice-01-01.png" alt=""></div>
                                                    <div class="voice voice-on"><img src="assets/images/feature-phone/voice-01-02.png" alt=""></div>
                                                    <div class="voice voice-success"><img src="assets/images/feature-phone/voice-01-03.png" alt=""></div>
                                                </div>
                                                <div class="screen screen-text">
                                                    <div class="voice voice-off"><img src="assets/images/feature-phone/voice-01-01.png" alt=""></div>
                                                    <div class="voice voice-on"><img src="assets/images/feature-phone/voice-01-02.png" alt=""></div>
                                                    <div class="voice voice-success"><img src="assets/images/feature-phone/voice-01-03.png" alt=""></div>
                                                </div>
                                                <div class="screen screen-browsing">
                                                    <div class="voice voice-off"><img src="assets/images/feature-phone/voice-01-01.png" alt=""></div>
                                                    <div class="voice voice-on"><img src="assets/images/feature-phone/voice-01-02.png" alt=""></div>
                                                    <div class="voice voice-success"><img src="assets/images/feature-phone/voice-01-03.png" alt=""></div>
                                                </div>
                                            </div>
                                        </div>
                                        <div class="anim-container">
                                            <div class="anim1"></div>
                                            <div class="anim2"></div>
                                            <div class="anim3"></div>
                                            <div class="anim4"></div>
                                        </div>
                                    </div>
                                    <div class="language-support-section">
                                        <div class="row">
										<div class="col-lg-4 left-section">
												<img src="assets/images/Featurephone/Jio_Phone.png" style="width:100%; height:474px;">
											<div class="demo1">
												Marathi
											</div>
											
											<div class="demo2" style="display:none;">
												Hindi
											</div>
											
											<div class="demo3" style="display:none;">
												gujarati
											</div>
											
											<div class="demo4" style="display:none;">
												tamil
											</div>
										</div>
											
											<div class="col-lg-offset-1 col-lg-7 right-section">
											<div class="lang-content">
												<h1>Use Voice Assistance to control jioPhone</h1>
												<p>Multiple language support copy text goes here....</p>
											</div>
											
												<ul class="languages">
													<li class="marathi">Marathi</li>
													<li class="hindi">Hindi</li>
													<li class="gujarati">Gujarati</li>
													<li class="tamil">Tamil</li>
												</ul>
											</div>
                                        </div>
                                    </div>
                                    <div class="preloaded-apps-section">
                                        <div class="row tabs-bg-color">
                                        <div class="preloaded-text"> 
                                            <h3>Pre-loaded Jio Apps</h3>  <p>Compelling apps to keep you entertained</p>
                                        </div>
                                        <div class="tabs-wrapper">
                                        <ul class="nav nav-tabs">
                                            <li class="active"><a data-toggle="tab" href="#myjio">MyJio</a></li>
                                            <li><a data-toggle="tab" href="#jiomusic">JioMusic</a></li>
                                            <li><a data-toggle="tab" href="#jiocinema">JioCinema</a></li>
                                            <li><a data-toggle="tab" href="#jiotv">JioTV</a></li>
                                      </ul>
                                      </div>
                                    </div>

                                <div class="tab-content">
                                    
                                    <div id="myjio" class="tab-pane fade in active">
                                    <div class="img-wrapper">
                                        <img src="assets/images/feature-phone/my-jio-masterhead-1440x708.jpg">
                                        <div class="img-content-wrapper">
                                        <ul>
                                        <li>
                                            <img src="assets/images/feature-phone/MyJio-small.png" >
                                        </li>
                                          <li>
                                          <div class="img-inner-wrapper">
                                              <h3>MyJio, your gateway to the digital world.</h3>
                                              <p>Quick installation and easy access to Jio applications. Manage your account on-the-go.
                                              </p>
                                          
                                          </div>
                                          </li>
                                        </ul>
                                    </div>
                                    </div>
                                    
                                    </div>

                                    <div id="jiomusic" class="tab-pane fade">
                                    <div class="img-wrapper">
                                        <img src="assets/images/feature-phone/jio-music-masterhead.jpg">
                                        <div class="img-content-wrapper">
                                      <ul>
                                        <li>
                                            <img src="assets/images/feature-phone/JioMusic-small.png" >
                                        </li>
                                          <li>
                                          <div class="img-inner-wrapper">
                                          <h3>Music for you. Anytime.</h3>
                                          <p>Anywhere. Millions of HD songs in over 20 languages. Unmatched clarity. Unbeatable experience.
                                        </p>
                                          </div>
                                          </li>
                                        </ul>
                                    </div>
                                    </div>
                                    </div>
                                    
                                    
                                    <div id="jiocinema" class="tab-pane fade">
                                    <div class="img-wrapper">
                                        <img src="assets/images/feature-phone/jio-cinema-masterhead-v3-1440x708.jpg">
                                        <div class="img-content-wrapper">
                                      <ul>
                                        <li>
                                            <img src="assets/images/feature-phone/JioCinema-small.png" >
                                        </li>
                                          <li>
                                          <div class="img-inner-wrapper">
                                              <h3>Best of entertainment for you.</h3>
                                              <p>One stop destination for premium Indian movies, TV shows and music videos.
                                              </p>
                                          
                                          </div>
                                          </li>
                                        </ul>
                                    </div>
                                    </div>
                                    </div>

                                    <div id="jiotv" class="tab-pane fade">
                                    <div class="img-wrapper">
                                        <img src="assets/images/feature-phone/jiotv-masthead-desk-v1.jpg">
                                        <div class="img-content-wrapper">
                                      <ul>
                                        <li>
                                            <img src="assets/images/feature-phone/JioTv-small.png" >
                                        </li>
                                          <li>
                                          <div class="img-inner-wrapper">
                                              <h3>Instant access to TV programmes</h3>
                                              <p>A wide range of TV channels across languages and genres. Enjoy 400+ TV channels at your fingertips, including 60+ HD channels.
                                              </p>                                          
                                          </div>
                                          </li>
                                        </ul>
                                    </div>
                                    </div>
                                    
                                    </div>
                                    </div>
                                    </div>



                                    <div class="tv-connect-section">
                                        <div class="row">
                                            <h1>TV connect section</h1>
                                            <p>TV connect section copy text goes here....</p>
                                        </div>
                                    </div>
                                </div>
                            </div>

                            <!-- accordian End -->
                            <!-- Main Body Includes Ends -->
                            <!-- Includes footer links and Social media icons -->

                    </div>

                </div>

            </div>

        </div>

        <!-- Wrap end -->
        <% include includes/site-footer-apps-live.html %>
            <% include includes/html-footer.html %>
                <script>
                    $(document).ready(function() {
                        
                        //voice command section
                        $(".anim1, .anim2, .anim3, .anim4").css({
                            "animation-play-state": "paused"
                        });

                        $(".voice-app").on("click", function() {
                            var ind = $(".voice-app").index($(this));
                            $(".anim1, .anim2, .anim3, .anim4").css({
                                "animation-play-state": "running"
                            });
                            
                            $(".phone-screen .screen").fadeOut(800, function() {
                                $(".phone-screen .screen .voice").fadeOut(100);
                            });
                            $(".phone-screen .screen").eq(ind).fadeIn(100, function() {
                                
                                $(".phone-screen .screen").eq(ind).find(".voice-off").fadeIn(800, function() {
                                    $(".phone-screen .screen").eq(ind).find(".voice-on").delay(500).fadeIn(800, function() {
                                        $(".phone-screen .screen").eq(ind).find(".voice-success").delay(500).fadeIn(800);
                                        
                                        $(".anim1, .anim2, .anim3, .anim4").css({
                                            "animation-play-state": "paused"
                                        });
                                    });
                                });
                                //$(".voice-on").hide();
                            });
                            
//                            if ($(".voice-off").is(":visible")) {
//                                $(".voice-off").hide();
//                                $(".voice-on").show();
//                            } else {
//                                $(".voice-off").show();
//                                $(".voice-on").hide();
//                            }

                            
                            
                        });
                        
                        
                        //language support section
                        $('.marathi').click(function(e){
                            e.preventDefault();
                            $(".demo1").show();
                            $(".demo2").hide();
                            $(".demo3").hide();
                            $(".demo4").hide();
                             }); 

                             $('.hindi').click(function(e){
                            e.preventDefault();
                            $(".demo1").hide();
                            $(".demo2").show();
                            $(".demo3").hide();
                            $(".demo4").hide();
                             }); 


                             $('.gujarati').click(function(e){
                            e.preventDefault();
                            $(".demo3").show();
                            $(".demo1").hide();
                            $(".demo2").hide();
                            $(".demo4").hide();
                             }); 


                             $('.tamil').click(function(e){
                            e.preventDefault();
                            $(".demo4").show();
                            $(".demo1").hide();
                            $(".demo2").hide();
                            $(".demo3").hide();
			
			 }); 
                    });
                </script>
