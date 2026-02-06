# Turtle
html = """<!DOCTYPE html>
<html>
<head>
<title>Welcome</title>

<style>
body {
    background: pink;
    text-align: center;
    font-family: Arial;
}

h1 {
    margin-top: 100px;
}

button {
    padding: 15px 30px;
    font-size: 20px;
    border-radius: 10px;
    border: none;
    cursor: pointer;
}

#yes {
    background: red;
    color: white;
}

#no {
    background: white;
}
</style>
</head>

<body>

<h1>Hey Nethh 🐨… I have something to ask you ❤️</h1>

<button id="yes" onclick="yes()">Yes</button>
<button id="no" onmouseover="move()">No</button>

<script>
function yes() {
    alert("Yay Nethh 🐨!!! 💕 You just made my day!");
}

function move() {
    let x = Math.random() * window.innerWidth;
    let y = Math.random() * window.innerHeight;

    document.getElementById("no").style.position = "absolute";
    document.getElementById("no").style.left = x + "px";
    document.getElementById("no").style.top = y + "px";
}
</script>

</body>
</html>
"""

with open("index.html", "w") as f:
    f.write(html)

print("Website created! Open index.html ❤️")
