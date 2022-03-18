<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>jQuery UI Draggable - Default functionality</title>
  <link rel="stylesheet" href="//code.jquery.com/ui/1.13.1/themes/base/jquery-ui.css">
  <link rel="stylesheet" href="/resources/demos/style.css">
  <style>
  #draggable { width: 150px; height: 150px; padding: 0.5em; }
  </style>
  <script src="https://code.jquery.com/jquery-3.6.0.js"></script>
  <script src="https://code.jquery.com/ui/1.13.1/jquery-ui.js"></script>
  <script>
  $( function() {
    $( "#draggable" ).draggable();
  } );
  </script>
</head>
<body>
<section>
    <p class="explanation">Below, a For Statement is calculating and printing the sum and product of every fourth integer from 5 - 21 inclusive. In the second section, a While Statement is calculating and printing the sum and product of every third integer from 3 - 21 inclusive.</p>
    <div id="drag" class="hw4-part1-divbox ui-draggable ui-draggable-handle" style="position: relative; width: 720px; inset: -9px auto auto -94px; height: 361.188px;">
      <h2>For Statement:</h2>
      <p id="for-sum">The sum of 5 + 9 + 13 + 17 + 21 is 65.</p>
      <p id="for-product">The product of 5 * 9 * 13 * 17 * 21 is 208,845.</p>
      <h2>While Statement:</h2>
      <p id="while-sum">The sum of 3 + 6 + 9 + 12 + 15 + 18 + 21 is 84.</p>
      <p id="while-product">The product of 3 * 6 * 9 * 12 * 15 * 18 * 21 is 11,022,480.</p>
      <p class="drag-box">*(drag the results area around, it moves!)</p>
    </div>
    <!-- <div class="explanation">
      <h3>Use Cases:</h3>
      <p>Study tool for elementary students.</p>
    </div> -->
  </section>
  <br>
  <script>
    var sum = 0;
    for (var number = 5; number <= 21; number += 4){
    sum += number;
  }
  document.getElementById("for-sum").innerHTML = "The sum of 5 + 9 + 13 + 17 + 21 is " + sum + ".";
                                     var product = 1;
                                     for (var x = 5; x <= 21; x += 4){
    product = product * x;
    }
  document.getElementById("for-product").innerHTML = "The product of 5 * 9 * 13 * 17 * 21 is " + product.toLocaleString(2) + ".";
    var x = 0;
    var sum = 0;
    while (x < 21){
                   x = 3 + x;
                   sum = x + sum;
                   }
                   document.getElementById("while-sum").innerHTML = "The sum of 3 + 6 + 9 + 12 + 15 + 18 + 21 is " + sum + ".";
                   var whileProduct = 1;
                   var y = 3;
                   while (y <= 21) {
    whileProduct *= y;
    y = y + 3;
    }
    document.getElementById("while-product").innerHTML = "The product of 3 * 6 * 9 * 12 * 15 * 18 * 21 is " + whileProduct.toLocaleString(2) + ".";
</script>
<!-- Bootstrap JS CDN Links -->
<script src="https://code.jquery.com/jquery-3.4.1.slim.min.js" integrity="sha384-J6qa4849blE2+poT4WnyKhv5vZF5SrPo0iEjwBvKU7imGFAV0wwj1yYfoRSJoZ+n" crossorigin="anonymous"></script>
  <script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.0/dist/umd/popper.min.js" integrity="sha384-Q6E9RHvbIyZFJoft+2mJbHaEWldlvI9IOYy5n3zV9zzTtmI3UksdQRVvoxMfooAo" crossorigin="anonymous"></script>
 <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/js/bootstrap.min.js" integrity="sha384-wfSDF2E50Y2D1uUdj0O3uMBJnjuUD4Ih7YwaYd1iqfktj0Uod8GCExl3Og8ifwB6" crossorigin="anonymous"></script>
 <!-- jQuery UI CDN Link-->  
  <script src="https://code.jquery.com/ui/1.11.4/jquery-ui.min.js" integrity="sha256-xNjb53/rY+WmG+4L6tTl9m6PpqknWZvRt0rO1SRnJzw=" crossorigin="anonymous"></script>
  <!-- placed after the jquery ui cdn link -->  
  <script>
   $(function() {
     $( "#drag" ).draggable();
    });
</script>
</body>
