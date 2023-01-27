<h1>pizza ovn.EXE</h1>
<!-- <p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p> -->

<link href="https://fonts.cdnfonts.com/css/alarm-clock" rel="stylesheet">
<link href="https://fonts.cdnfonts.com/css/cheese-pizza" rel="stylesheet">
                
 
<body style="background-color: gray;"></body>


<style>
   
    h1{position: absolute; font-size: 50px; font-family: 'CHEESE PIZZA', sans-serif; color: rgb(214, 33, 33); text-shadow: 100px; text-decoration: underline; text-decoration-color: rgb(72, 167, 28); background-color: aliceblue; border-radius: 10px;}
    h1{left: 850px; }


    body {
  background-image: url('/brick.jpg');
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: 100% 100%;
}
   

    .div {
        text-align: center;
    }

    #button {
        position: absolute; left: 1050px; top: 130px; width: 50px; height: 50px;
    }

    #button2{
        position: absolute; left: 850px; top: 130px; width: 50px; height: 50px;
    }

    #counter{
        font-size: 50px; 
        position: absolute; left: 950px; top:80px;
        font-family: 'alarm clock', sans-serif;
        color: red;
                                                
    }
    #pizza{
        top: 200px;
        left: 620px;
        position: absolute;
    }
    
</style>


<script>

     var navn = "Leon";


    function zeroCheck(){
        if (counter == 0) {
             document.querySelector("#pizza").src ="/pizza.png"
        
            }
    }

    let counter = 0
    function increaseCounter(){
        counter += 10
        
        document.querySelector("#pizza").src ="/pizza.gif"
    }

    
    function decreaseCounter(){
      
        if (counter > 0){
            counter += -10
           
    
            zeroCheck()
        }
    }
           

</script>


<div class="div">
    <button id="button" on:click={increaseCounter}>+</button>
    <button id="button2" on:click={decreaseCounter}>-</button> 
    <p id="counter"> {counter}°</p> 
</div>

<img id="pizza" src="/pizza.png" alt="pizza" style="width:750px;height:400px;">

<p style="background-image: url('/brick.jpg');"></p>