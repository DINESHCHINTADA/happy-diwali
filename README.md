
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Diwali</title>
    <link rel="stylesheet" href="happy_diwali.css">
</head>
<body>
    <div class="container">
        <h1 class="title1">Wishing You & Your Family a very</h1>
        <h2 class="title">Happy Christmas</h2>
        <ul class="fireworks">
            <li><span></span></li>
            <li><span></span></li>
            <li><span></span></li>
            <li><span></span></li>
            <li><span></span></li>
            <li><span></span></li>
        </ul>
    </div>

    <div class="fireworks-container">
        <div class="firework"></div>
        <div class="firework"></div> 
        <div class="firework"></div>
        <div class="firework"></div>
        <div class="firework"></div>
        <div class="firework"></div>
    </div>

    <footer>
        <h4 class="from">@mr_Dinu_065</h4>
        <div>
            <img class="logo" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQf3Z1_o9Bli5OnIq_1e3Xy1rCu8xsc4ErSUA&s" 
                alt="NVR College of Engineering Logo" width="120" height="120">
        </div>
        <div class="form2">NVR</div>
        <div class="form">COLLEGE OF ENGINEERING</div>
        <div class="form1">& TECHNOLOGY</div>
    </footer>
</body>
</html>
body {
  background-color: #212121;
  font-family: Pacifico;
}
.container {
  position: absolute;
  height: 20px;
  width: 600px;
  left: 450px;
  top: 330px;
}
.title1 {
  position: relative;
  color: rgba(132, 128, 128, 0.5);
  padding-left: 20px;
  text-shadow: 0px 2px 1px orange, 0px 0px 6px orangered, 0px 5px 10px rgba(0, 0, 0, 1);
  font-size: xx-large;
  width: 600px;
  font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
}
.container .title {
  margin-left: 20px;
  font-size: 4rem;
  color: rgba(132, 128, 128, 0.5);
  text-align: center;
  width: 500px;
  text-shadow: 0px 2px 1px orange, 0px 0px 6px orangered, 0px 5px 10px rgba(0, 0, 0, 1);
}
.fireworks {
  list-style-type: none;
  padding: 0;
}
.fireworks li {
  display: inline-block;
  margin: 20px;
  height: 50px;
  width: 50px;
  border-radius: 500px;
  position: relative;
  background-color: #8d6e63;
  box-shadow: 0px 2px 5px rgba(0, 0, 0, 0.5);
}
.fireworks li::before, .fireworks li::after {
  content: "";
  position: absolute;
  height: 100%;
  background-color: #212121;
  width: 100%;
  border-radius: 500px;
  top: -40%;
}
.fireworks li span {
  display: inline-block;
  height: 20px;
  width: 20px;
  position: absolute;
  left: 0;
  right: 0;
  margin: auto;
  z-index: 1;
  border-bottom-left-radius: 50px;
  border-bottom-right-radius: 50px;
  border-top-right-radius: 50px;
  transform: rotate(45deg);
  animation: fire 0.3s ease infinite;
}
@keyframes fire {
  0%, 100% {
    transform: rotate(55deg);
    width: 20px;
    background: linear-gradient(90deg, orange, orangered);
  }
  50% {
    transform: rotate(35deg);
    width: 18px;
    background: linear-gradient(90deg, orangered, orange);
  }
}
/* Add the rest of your CSS from the given code here */
