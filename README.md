<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>
<script>
  $(function() {
    //caches a jQuery object containing the header element
    var header = $("#wrap2");
    $(window).scroll(function() {
        var scroll = $(window).scrollTop();

        if (scroll >= 400) {
            header.addClass("sticky");
        } else {
            header.removeClass("sticky");
        }
	    
    });
	   

});
</script>

/*------------- Css starts Here ------------------*/

.sticky{
  position:fixed !important;
  top:21%;
  padding-bottom:600px;
  max-width:200px;
  width:100%;
}

.wrap {
  position: relative;
  max-width:200px;
  width:100%; 
}

nav2{
  float: none; 
  clear: both;
  max-width:200px;
  width: 100%; 
  margin: 10% auto;
  text-align:center;
}

nav2 a {
  position: relative;
  display: block;
  padding: 10px 20px;
  border-left: 5px solid #B75155;
  font-size: 14px;
  z-index: 1;
  margin-bottom:2px;
  color:#111;
  font-weight:normal;
}

i {
  text-decoration: none;
  
}

nav2 a i {
  padding: 15px 25px;
  font-family: 'FontAwesome', sans-serif;
  color: #444;
}

nav2 > span { z-index: 3;}

nav2 a:before {
  content: "";
  position: absolute; 
  background: #E16267;
  height: 100%;
  width: 0px;
  top: 0;
  left: 0;
  transition: all 0.3s ease 0s; 
  -webkit-transition: all 0.3s ease 0s; 
  z-index: -1;
}

nav2 a:hover:before { width: 100%;}

nav2 a:hover span{ color: white;}
nav2 a:hover i{ color: white;}



/*---------------------- End of Css -------------------*/


<!-- start of html -->

<div class="wrap" id="wrap2">
  <nav2>
	<a data-req="anchor" href="#this-is-the-anchor-tag"><span>Place Text Here</span></a>
	<a data-req="anchor" href="#this-is-the-anchor-tag"><span>Place Text Here</span></a>
	<a data-req="anchor" href="#this-is-the-anchor-tag"><span>Place Text Here</span></a>

  </nav2>
</div>
