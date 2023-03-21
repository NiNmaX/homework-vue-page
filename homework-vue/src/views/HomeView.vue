<template>
    <link rel='stylesheet' href='https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.3.7/css/bootstrap.min.css'>
    <link rel='stylesheet' href='https://fonts.googleapis.com/css?family=Arvo'>
  <div>
        <div class="home">
            <div class="row">	
                <div class="col-sm-12 ">
                    <div class="col-sm-10 col-sm-offset-1  text-center">
                        <div class="four_zero_four_bg">
                            <h1 class="text-center ">Home</h1>
                        </div>
                        <div class="contant_box_404">
                            <p>Siz qidirayotgan sahifa mavjud emas!</p>
                            <a href="#" class="link_404">Bosh sahifa</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
  </div>
</template>
<script>
export default {
  
}
</script>
<style>
  .home{ 
    margin-top: 300px;
    margin-left: -1030px;

    width: 600px;
    background:#fff; 
    font-family: 'Arvo', serif;
}
.home  img{ 
    width:100%;
}
.four_zero_four_bg{
    background-image: url("https://cdn.dribbble.com/users/285475/screenshots/2083086/dribbble_1.gif");
    height: 400px;
    background-position: center;
}
.four_zero_four_bg h1{
    font-size:80px;
}
.four_zero_four_bg h3{
	font-size:80px;
}			 
.link_404{			 
	color: #fff!important;
    padding: 10px 20px;
    background: #ff0f5b;
    margin: 20px 0;
    display: inline-block;
    border-radius: 30px;
    font-size: 18px;
}
.contant_box_404{
    margin-top:-50px;
}
</style>
