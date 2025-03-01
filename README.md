# New<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>First 10 Natural Numbers</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 40px;
    }
    h1 {
      color: #333;
    }
    ul {
      list-style-type: none;
      padding: 0;
    }
    li {
      background: #f0f0f0;
      margin: 5px 0;
      padding: 10px;
      border-radius: 4px;
    }
  </style>
</head>
<body>
  <h1>First 10 Natural Numbers</h1>
  <ul id="numberList"></ul>

  <script>
    // Function to generate the first n natural numbers
    function naturalNumbers(n) {
      const numbers = [];
      for (let i = 1; i <= n; i++) {
        numbers.push(i);
      }
      return numbers;
    }

    // Set the number of natural numbers to generate
    const n = 10;
    const numbers = naturalNumbers(n);

    // Get the ul element where the numbers will be displayed
    const listElement = document.getElementById('numberList');

    // Loop through the numbers and add each as a list item
    numbers.forEach(function(number) {
      const li = document.createElement('li');
      li.textContent = number;
      listElement.appendChild(li);
    });
  </script>
</body>
</html>
