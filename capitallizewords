<?php
function capitalizeWords($input)
{
    // Explode the input string into an array of words
    $words = explode(" ", $input);
    
    // Loop through each word and capitalize the first letter
    foreach ($words as &$word) {
        $word = ucfirst($word);
    }
    
    // Join the words back into a string
    $result = implode(" ", $words);
    
    return $result;
}


?>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
</head>
<body>
    <?php
    echo "<h2>Capitalize word using PHP function</h2>";echo "<hr>";
$input = "hello world";
$result = capitalizeWords($input);
echo $result; // Outputs: "Hello World"

?>

<hr>
<?php
echo "<h2>Capitalize word using Javascript function</h2>";echo "<hr>";?>
<input type="text" id="myInput" oninput="capitalizeWords('myInput')">






<?php
echo "<h2>Capitalize word using Jquery function</h2>";echo "<hr>";?>
<input type="text" id="jqinput">








<script>
    function capitalizeWords(inputId) {
  // Get the input element by its ID
  var input = document.getElementById(inputId);
  
  // Get the input value
  var inputValue = input.value;
  
  // Split the input value by space to get an array of words
  var words = inputValue.split(" ");
  
  // Loop through each word in the array
  for (var i = 0; i < words.length; i++) {
    // Get the current word
    var word = words[i];
    
    // Capitalize the first letter of the word
    var capitalizedWord = word.charAt(0).toUpperCase() + word.slice(1);
    
    // Replace the original word with the capitalized word in the array
    words[i] = capitalizedWord;
  }
  
  // Join the words back into a single string separated by spaces
  var capitalizedInputValue = words.join(" ");
  
  // Set the input value to the capitalized string
  input.value = capitalizedInputValue;
}



</script>
<script>
    $("#jqinput").on("input", function() {

  var inputValue = $(this).val();
  var words = inputValue.split(" ");
  
  for (var i = 0; i < words.length; i++) {
    var word = words[i];
    var capitalizedWord = word.charAt(0).toUpperCase() + word.slice(1);
    words[i] = capitalizedWord;
  }
  
  var capitalizedInputValue = words.join(" ");
  $(this).val(capitalizedInputValue);
});
</script>
</body>
</html>
