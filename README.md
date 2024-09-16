<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charaset="UTF-8">
        <title>js</title>
        <style>
            div{
                width:200px;
                height:400px;
                background: #0f5898;
                margin:auto;
                padding:50px;
            }
        </style>
    </head>
    <body>
        <div>
            <h3>Simple Interest Calc</h3>
            <label>Principal Amount</label><br>
            <input type="text" id="pamt"/><span>&#8377;</span><br>

            <label>Rate of Interest</label><br>
            <input type="text" id="roi"/><span>(%)</span><br>

            <label>Time</label><br>
            <input type="text" id="tim"/><span>Year(s)</span><br>
            <button onclick="compute() ">Calculate</button>
            <br><br>
            <output id="result"></output>
        </div>
        <script>
            function compute()
            {
                let p,r,t,si;
                p= pamt.value;
                r= roi.value;
                t = tim.value;
                si = p*t*r/100;
                result.value="Interest Amount:"+si;
            }
        </script>
    </body>
</html>
