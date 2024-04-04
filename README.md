
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Odd/Even Checker and Sum Calculator</title>
    <style>
        body {
            background-image: url(https://img.freepik.com/premium-photo/purple-flowers-purple-background_7566-2736.jpg);
            background-repeat: no-repeat;
            text-align: center;
            background-size: 1000px;
            font-size: x-large;
            
        }
        h1 {
           font-size: xx-large;
           font-style: oblique;
           
           
        }
        #bordering {
            border: 10px solid transparent;
           padding: 15px;
           border-image: url(border.png) 30 stretch;
        }
    </style>
</head>
<body>
    <h1>ITERATION STATEMENTS</h1>

    <script>
        // Function to check if a number is odd or even and calculate the sum
        function checkNumber() {
            let num = parseInt(prompt("Enter an integer:"));
            let sum = 0;
            let output = '';

            for (let i = 1; i <= num; i++) {
                sum += i;
                output += i + (i % 2 === 0 ? ' (Even)' : ' (Odd)') + '<br>';
            }

            output += '<br>Sum of all numbers from 1 to ' + num + ' is: ' + sum;
            document.body.innerHTML += output;
        }

        // Call the function when the page loads
        checkNumber();
    </script>
</body>
</html>
