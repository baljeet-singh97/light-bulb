<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Switch Bulb</title>

    <style>
    .center {
        display: block;
        margin-left: auto;
        margin-right: auto;

       
    }
    .btn{
        padding: 20px;
        background-color: green;
        color: aliceblue;
    }
    </style>
</head>
<body style="background-color: black;">
    <img id="bulb" src="/img/offbulb.jpg" alt="" class="center" width="400px" height="500px">
    <button id="toggleBtn" class="center btn" >Turn On</button>



    <script>

        let btn = document.getElementById('toggleBtn')
        let bulb = document.getElementById('bulb')
        
        btn.addEventListener('click', toggleBulb)

        //event - every event listner has an event property we have to pass
        //here as an argumnet with the help of this we get to know about
        // where this event came from what this want to do
        function toggleBulb(e) {
            if(btn.textContent.includes('On'))
            {
                bulb.src = "img/onbulb.jpg"
                btn.textContent = " Turn Off"
            }
            else
            {
                bulb.src = "img/offbulb.jpg"
                btn.textContent = " Turn On"
            }
            

        }
        


    </script>

    
</body>
</html>
