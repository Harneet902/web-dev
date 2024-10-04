<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AccuWeather</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <nav>
            <!-- logo -->
            <div class="logo">
                <img src="https://www.accuweather.com/images/logos/accuweather.svg" >
                
            </div>

            <!-- dropdown menu -->
            <div class="dropdown">
                <button onclick="myFunction()" class="dropbtn"> ☴ </button>
                <div id="myDropdown" class="dropdown-content">

                    <!-- top -->
                    <div class="top">
                        <h3> <img src="https://th.bing.com/th/id/OIP.huwXvK-S7mYlzFkA0ObjEAHaHa?w=192&h=193&c=7&r=0&o=5&dpr=1.35&pid=1.7" width="24" height="25" > Settings</h3>
                        <h3>PUNE, MAHARASHTRA WEATHER</h3>
                        <hr>
                    </div>

                    <!-- Middle -->
                    <div class="mid">
                        <h3>Today</h3>
                        <h3>Hourly</h3>
                        <h3>Daily</h3>
                        <h3>Rader</h3>
                        <h3>MinuteCast</h3>
                        <h3>Monthly</h3>
                        <h3>Air Quality</h3>
                        <br><br>
                        <h3>ARROUND THE GLOBE</h3>
                        <hr>
                    </div>

                    <!-- bottom -->
                    <div class="bottom">
                        <h3>Hurricane Tracker</h3>
                        <h3>Severe Weather</h3>
                        <h3>Radar & Maps</h3>
                        <h3>News</h3>
                        <h3>Video</h3>
                        <h3>Podcasts</h3>
                        <h3>Winter Center</h3>
                    </div>


                </div>
              </div>
              
              <script>
              /* When the user clicks on the button, 
              toggle between hiding and showing the dropdown content */
              function myFunction() {
                document.getElementById("myDropdown").classList.toggle("show");
              }
              
              // Close the dropdown if the user clicks outside of it
              window.onclick = function(event) {
                if (!event.target.matches('.dropbtn')) {
                  var dropdowns = document.getElementsByClassName("dropdown-content");
                  var i;
                  for (i = 0; i < dropdowns.length; i++) {
                    var openDropdown = dropdowns[i];
                    if (openDropdown.classList.contains('show')) {
                      openDropdown.classList.remove('show');
                    }
                  }
                }
              }
              </script>

        </nav>

        <!-- search box -->
        <div class="search">
            <input type="text" placeholder="Search"  name="search">
            <button> <img src="./baseline_search_black_24dp.png" > </button>
        </div>
        
        <!-- floating box -->
        <div class="bar">
          <span>Pune,Maharashtra <img src="https://www.accuweather.com/images/weathericons/36.svg " width="6%"> 24°C</span>
          
        </div>


    </header>

    <section class="col1">
      <div class="c1">
        <h2>INDIA WEATHER RADAR</h2>
        <img src="https://api.accuweather.com/maps/v1/radar/static/globalSIR/tile?apikey=de13920f574d420984d3080b1fa6132b&zoom=3&lon=77.000&lat=20.000&imgwidth=768&imgheight=432&language=en-us&base_data=radar">
      </div>

      <div class="news">
        <h2>WEATHER NEWS</h2>
        <div class="newsData">
          <img src="https://cms.accuweather.com/wp-content/uploads/2022/01/Screen-Shot-2022-01-15-at-9.45.19-AM.png?h=128"  > 
          <h3>WINTER WEATHER</h3>
          <h4>
            Winter storm buries Midwest under foot of travel-snarling snow</h4>
          <h4 id="date">Jan. 15, 2022</h4>
        </div>
      </div>

      <div class="news">
        <div class="newsData">
          <img src="https://cms.accuweather.com/wp-content/uploads/2022/01/Pattern-graphic-01.15.2022.jpeg?h=128" width="180px" height="130px"> 
          <h3>WINTER WEATHER</h3>
          <h4>
            Winter storm buries Midwest under foot of travel-snarling snow</h4>
          <h4 id="date">Jan. 15, 2022</h4>
        </div>
      </div>

      <div class="news">
        <div class="newsData">
          <img src="https://cms.accuweather.com/wp-content/uploads/2022/01/Study-1000-light-year-wide-Local-Bubble-is-source-of-all-young-stars-closest-to-Earth.jpeg?h=128" > 
          <h3>WINTER WEATHER</h3>
          <h4>
            Study: 1,000-light-year-wide 'Local Bubble' is source of all young sta.</h4>
          <h4 id="date">Jan. 15, 2022</h4>
        </div>
      </div>

      <div class="news">
        <div class="newsData">
          <img src="https://cms.accuweather.com/wp-content/uploads/2022/01/AP456842954367.jpg?h=128" > 
          <h3>WINTER WEATHER</h3>
          <h4>     
          Atlanta and snowfall: A rocky history, to say the least</h4>
          <h4 id="date">Jan. 15, 2022</h4>
        </div>
      </div>
    </section>

    <!-- 2nd coloum -->
    <section class="col2">
      <div class="blog">
        <h3 class="top"><span class="blink">.</span>  LIVE BLOG </h3>
        <hr>
        <h3>
          LIVE: Snow clogs roads in Carolinas as storm strengthens</h3>
          <img src="https://cms.accuweather.com/wp-content/uploads/2022/01/Screen-Shot-2022-01-16-at-8.40.16-AM.png?w=475" >
          <h4>LATEST ENTRY</h4>
          <h4>Power outages climb across Southeast</h4>
          <p>22 minutes ago</p>
          
      </div>

      <div class="featuredNews">
        <h3 class="top"> Featured Stories </h3>
        <hr>
        <h3>
          <h4>Dog coats to keep your pup protected and warm this winter</h4>
          <hr>
          <h4>Our picks for indoor space heaters for working from home</h4>
          <hr>
          <h4>Skies went dark: Historians pinpoint the very 'worst year' ever to be ...</h4>
      </div>
    </section>

    <!-- footer -->

    <footer>
      <div class="topOfFooter">
        <h4><span>World</span><span>></span><span>Asia</span><span>></span><span>India</span><span>></span>
          <span>Maharashtra</span><span>></span><span>Pune</span></h4>
      </div>
      
      <ul class="r-footer">
        <li>
          <h2>COMPANY</h2>
        <ul class="box">
        <li><a href="#">Proven Superior Accuracy</a></li>
        <li><a href="#">About AccuWeather</a></li>
        <li><a href="#">Digital Advertising</a></li>
        <li><a href="#">Careers</a></li>
        <li><a href="#">Press</a></li>
        <li><a href="#">Contact Us</a></li>
        <div class="socal">
          <img src="https://www.accuweather.com/images/socialicons/downloads.svg" alt="">
          <img src="https://www.accuweather.com/images/socialicons/facebook.svg" alt="">
          <img src="https://www.accuweather.com/images/socialicons/twitter.svg" alt="">
          <img src="https://www.accuweather.com/images/socialicons/tv.svg" alt="">
        </div>
        </ul>
        </li>

        <li>
          <h2>PRODUCT & SERVICES</h2>
        <ul class="box">
            <li><a href="#">For Business</a></li>
            <li><a href="#">For Partners</a></li>
            <li><a href="#">AccuWeather APIs</a></li>
            <li><a href="#">Podcast</a></li>
        </ul>
        </li>

        <li>
            <h2>APPS & DOWNLOADS</h2>
          <ul class="box">
              <li><a href="#">iPhone App</a></li>
              <li><a href="#">Android App</a></li>
              <li><a href="#">See all Apps & Downloads</a></li>
              <li><a href="#">Podcast</a></li>
              <h2>SUBSCRIPTION SERVICES</h2>
              <li><a href="#">AccuWeather Premium</a></li>
              <li><a href="#">AccuWeather Professional</a></li>
          </ul>
          </li>


        <li>
          <h2>MORE</h2>
        <ul class="box">
            <li><a href="#">AccuWeather Shop</a></li>
            <li><a href="#">AccuWeather READY</a></li>
            <li><a href="#">Business</a></li>
            <li><a href="#">Health</a></li>
            <li><a href="#">Hurricane</a></li>
            <li><a href="#">Leisure and Recreation</a></li>
            <li><a href="#">Severe Weather</a></li>
            <li><a href="#">Space and Astronomy</a></li>
            <li><a href="#">Sports</a></li>
            <li><a href="#">Travel</a></li>
            <li><a href="#">Weather News</a></li>
            <li><a href="#">Weather Blogs</a></li>
            <li><a href="#">Winter Weather</a></li>


        </ul>
        </li>

        </ul>
        <hr>
        
        <div class="c">
          <p>© 2021 AccuWeather, Inc. "AccuWeather" and sun design are registered trademarks of AccuWeather, Inc. All Rights Reserved.</p>
          <br>
          <p>Terms of Use | Privacy Policy | Cookie Policy | TAG Disclosure</p>
        </div>
 

      </section>
    </footer>

</body>
</html>
