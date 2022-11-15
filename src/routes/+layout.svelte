  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">


<style>

  
  
	.bot {
		
		display: flex;
	}

	.nav {
		background-color: white;
		z-index: 2;
		
	}





.header {
  position: fixed;
	top:0px;
	margin:-10px;
  padding: 40px;
  width:100%;
  text-align: left;
  background: black;
  color: white;
}



.footer {
	margin:-10px;
  position: fixed;
 	bottom: 0;
  width: 100%;
  background-color: black;
  color: white;
  text-align: center;
	padding:20px;
}

.sidepanel  {
  width: 0;
  position: fixed;
  z-index: 1;
  height: 100%;
  top: 0;
  right: 60;
  background-color: purple;
  background: linear-gradient(purple, pink);
  letter-spacing: 1.4rem;
  overflow-x: hidden;
  transition: 0.5s;
  padding-top: 60px;
  text-align: center;
  
}

.sidepanel a {
  padding: 8px 8px 8px 32px;
  text-decoration: none;
  font-size: 60px;
  color: white;
  display: block;
  transition: 0.3s;
}

.sidepanel a:hover {
  color: #f1f1f1;
}

.sidepanel .closebtn {
  position: flex;
  top: 0;
  right: 25px;
  font-size: 100px;
}

.openbtn {
  font-size: 30px;
  cursor: pointer;
  position: fixed;
  color: black;
  padding: 20px 40px;
  border: none;
	margin-top:-400px;
  margin-left:-100px;
}

.openbtn:hover {
  background-color:#444;
}


</style> 


<div class="body"> 

	<div class="header">

	</div>

	<div class ="bot">



	



	<slot />
	</div>

	<div class="footer">
 	 	<a class="active" href="#"><i class="fa fa-facebook-official w3-hover-opacity"></i><a> 
		<a class="active" href="#"><i class="fa fa-instagram w3-hover-opacity"></i></a> 
		<a class="active" href="#"><i class="fa fa-linkedin w3-hover-opacity"></i></a>
	</div>

<div align="right">
  <div id="mySidepanel" class="sidepanel">
  <a href="javascript:void(0)" class="closebtn" onclick="closeNav()">×</a>
  <a href="#">HOME</a>
  <a href="#">STUDIES</a>
  <a href="#">WORKS</a>
  <a href="#">ABOUT ME</a>
  <a href="#">CONTACT</a>
</div>

<button class="openbtn" onclick="openNav()">☰</button>
  
  <script>
function openNav() {
  document.getElementById("mySidepanel").style.width = "100%";
}

function closeNav() {
  document.getElementById("mySidepanel").style.width = "0";
}
</script>
</div>

</div> 


