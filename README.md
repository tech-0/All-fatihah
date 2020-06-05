
<!DOCTYPE html>
<html lang="en" dir="ltr">

<head>
  <meta charset="utf-8">
  <meta content='maximum-scale=1.0, initial-scale=1.0, width=device-width' name='viewport'>
  <title>COVID 19</title>
  <link rel="icon" href="/favicon.ico">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/materialize/1.0.0/css/materialize.min.css">

</head>

<body>
  <style media="screen">
    #logo {
      margin-left: 5px;
    }

    #row1 {
      margin-top: 20px;
    }
    #switch{
      margin-right: 10px;
    }
    h6{
      font-weight: 500;

    }
    #iraq{
      margin-top: -10px;
      font-weight: 500;
      font-size: 20px;
    }
  </style>

  <div class="navbar-fixed ">
    <nav class="green">
      <div class="nav-wrapper ">
        <a href="#!" class="brand-logo left" id="logo">COVID 19</a>
        <ul class="right">
          <div class="switch " id="switch">
            <label class="white-text">
              English
              <input type="checkbox" class="check">
              <span class="lever white"></span>
              کوردی
            </label>
          </div>
        </ul>
      </div>
    </nav>
  </div>
  <div class="container">
    <div class="row" id="row1">
      <div class="col l12 m12 s12 center-align">
        <h1 id="home">Stay Home</h1>
      </div>
    </div>
      <div class="row">
        <div class="col l12 m12 s12 center-align">
          <img src="world.png" width="25%" alt="">
        </div>
      </div>
    <div class="row">
      <div class="col l12 m12 s12 center-align" >

        <h2 id="case">Coronavirus Cases</h2>
        <h4> 6,747,148 </h4>

      </div>
    </div>
    <div class="row">
      <div class="col l12 m12 s12 center-align" >
        <h2 id="death">Deaths</h2>
        <h4 class="red-text"> 394,306 </h4>
      </div>
    </div>
    <div class="row">
      <div class="col l12 m12 s12 center-align" >
        <h2 id="recover">Recovered</h2>
        <h4 class="green-text text-darken-2"> 3,277,057 </h4>
      </div>
    </div>
    <div class="row">
      <div class="col l12 m12 s12 center-align">
        <div class="card grey lighten-1">
          <div class="card-content ">
            <h5 id="ncase">New Cases</h5>
            <h6>54,454</h6>
            <h5 id="ndeath">New Deaths</h5>
            <h6 class="red-text ">2,008</h6>
            <h5 id="acase">Active Cases</h5>
            <h6>3,075,785</h6>
          </div>
        </div>
      </div>
    </div>
  <div class="row">
    <div class="col l12 m12 s12 center-align">
    <h4 id="click">Click here to see corona virus stats of Iraq</h4>
      <a href="/iraq" class="red-text" id="iraq" >

    Click Here
      </a>
    </div>
  </div>

  </div>




  <script type="text/javascript">
    let checkbox = document.querySelector(".check");
    checkbox.addEventListener('change', function(){
      if(this.checked){
        //kurdi
        document.querySelector("#home").innerHTML = "لەماڵەوە بمێنەرەوە";
        document.querySelector("#case").innerHTML = "توشبوو";
        document.querySelector("#death").innerHTML = "مردن"
        document.querySelector("#recover").innerHTML = "چاکبونەوە";
        document.querySelector("#ncase").innerHTML = "توشبوانی ئەمڕۆ";
        document.querySelector("#ndeath").innerHTML = "مردوانی ئەمڕۆ";
        document.querySelector("#acase").innerHTML = "چالاک";
        document.querySelector("#click").innerHTML = "کلیک لێرە بکە بۆ بینینی رێژەی تووش بوون و چاکبوونەوەی عراق";
        document.querySelector("#iraq").innerHTML = "کلیک لێرەبکە";

      }else{
        document.querySelector("#home").innerHTML = "Stay Home";
        document.querySelector("#case").innerHTML = "Coronavirus Cases";
        document.querySelector("#death").innerHTML = "Deaths"
        document.querySelector("#recover").innerHTML = "Recovered";
        document.querySelector("#ncase").innerHTML = "New Cases";
        document.querySelector("#ndeath").innerHTML = "New Deaths";
        document.querySelector("#acase").innerHTML = "Active Cases";
        document.querySelector("#click").innerHTML = "Click here to see corona virus stats of Iraq";
        document.querySelector("#iraq").innerHTML = "Click Here";
      }
    })
  </script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/materialize/1.0.0/js/materialize.min.js"></script>
</body>

</html>
