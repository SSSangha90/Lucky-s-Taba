# Lucky-s-Taba
HTML5, CSS3, JavaScript, JQuery


<script src="//ajax.googleapis.com/ajax/libs/jquery/1.10.2/jquery.min.js"></script>
<!DOCTYPE html>
<head>
<script src="/assets/jquery.js"></script>
<link href='https://fonts.googleapis.com/css?family=Londrina Shadow' rel='stylesheet' type='text/css'>
<style>
body {
  font-family: helvetica, sans-serif;
  margin: 0 auto;
  max-width: 600px;
  background: #232355;
}
div {
  height: 200px;
  background-size: cover;
  position: relative;
  margin: 40px 0 0 0;
  border-radius: 12px;
}
h1 {
  font-family: 'Londrina Shadow', cursive;
  text-align: center;
  font-size: 75px;
  color: #aaaaaa;
  margin: 60px 0 0 0;
}
h2 {
  text-align: center;
  color: #bbbbbb;
  margin: 0px 0 70px 0;
}
p {
  color: rgba(255,255,255,1);
  background: black;
  background: linear-gradient(bottom, rgba(0,0,0,1), rgba(0,0,0,.4));
  background: -webkit-linear-gradient(bottom, rgba(0,0,0,1), rgba(0,0,0,.4));
  background: -moz-linear-gradient(bottom, rgba(0,0,0,1), rgba(0,0,0,.4));
  padding: 10px;
  line-height: 28px;
  text-align: justify;
  position: absolute;
  bottom: 0;
  margin: 0;
  height: 30px;
  transition: height .5s;
  -webkit-transition: height .5s;
  -moz-transition: height .5s;
}

small {
  opacity: 0;
}

.show-description p {
  height: 150px;
}

.show-description small {
  opacity: 1;
}

.first{
  background-image: url("http://www.manjulaskitchen.com/blog/wp-content/uploads/chilli_paneer.jpg");
}
.second{
  background-image: url("https://gbc-cdn-public-media.azureedge.net/img71955.768x512.jpg");
}
.dessert{
  background-image: url("https://media.hungryforever.com/wp-content/uploads/2015/06/rasmalai1.jpg");
}
.price {
  float: right;
}
@media (max-width: 500px) {
  h1 {
    font-size: 50px;
    margin-top: 20px;
    line-height: 40px;
  }
  h2 {
    font-size: 20px;
    margin: 20px 0 30px 0;
  }
  div {
    margin: 20px 12px 0 12px;
  }
  p {
    font-size: 20px;
    line-height: 24px;
  }
  small {
    font-size: 16px;
  }
}

</style>

</head>

<body>
<h1>Lucky's Taba</h1>
<h2>The finest desi food!</h2>
<div class="first">
  <p>Chili Paneer <span class="price">�11.99</span><br />
  <small>This spicy dish is an absolute favourite, wooing customers of all backgrounds. Tender, spicy chunks of paneer in a sweet and spicy sauce.
  </small></p>
</div>

<div class="second">
  <p>Chicken Tikka <span class="price">�14.99</span><br />
  <small>An all-time classic. Succulent dices of chicken breast, roasted in a tandoor over night for a well-marinated taste. Show-stopper if you have guests around.</small></p>
</div>
  
<div class="dessert">
  <p>Ras Malai <span class="price">�6.99</span><br />
  <small>A traditional indian desert, meaning juicy cream. A sure-fire way to satisfy those with sweet taste-buds.</small></p>
</div>

<script>
  $('div').on('click', function() {
      $(this).toggleClass('show-description');
  });
</script>

</body>
