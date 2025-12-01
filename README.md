# Python
Just a simple word finder in paragraph with the help of python (basically i am figuring github) this code is juat a joke :

<!DOCTYPE html>
<html>
<head>
    <title>Word Search</title>
</head>
<body>

<h2>Word Search Tool</h2>

<textarea id="para" rows="5" cols="40" placeholder="Enter your paragraph here"></textarea>
<br><br>

<input id="word" type="text" placeholder="Enter the word you want to search">
<br><br>

<button onclick="searchWord()">Search</button>

<p id="result"></p>

<script>
function searchWord() {
    let para = document.getElementById("para").value.toLowerCase();
    let word = document.getElementById("word").value.toLowerCase();

    if (para.includes(word)) {
        document.getElementById("result").innerHTML = 
            "Your word is in the paragraph: " + word;
    } else {
        document.getElementById("result").innerHTML = 
            "Your searched word is not in the paragraph.";
    }
}
</script>

</body>
</html>

