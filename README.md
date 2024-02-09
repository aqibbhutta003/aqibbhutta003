<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Keyboard Testing Tool</title>
<style>
    body {
        font-family: Arial, sans-serif;
        text-align: center;
    }
    .key {
        display: inline-block;
        width: 40px;
        height: 40px;
        margin: 5px;
        border: 1px solid #000;
        cursor: pointer;
    }
</style>
</head>
<body>
    <h1>Keyboard Testing Tool</h1>
    <p>Click on each key to test its functionality:</p>
    <div id="keyboard">
        <div class="row">
            <div class="key" onclick="testKey('1')">1</div>
            <div class="key" onclick="testKey('2')">2</div>
            <div class="key" onclick="testKey('3')">3</div>
            <div class="key" onclick="testKey('4')">4</div>
            <div class="key" onclick="testKey('5')">5</div>
            <div class="key" onclick="testKey('6')">6</div>
            <div class="key" onclick="testKey('7')">7</div>
            <div class="key" onclick="testKey('8')">8</div>
            <div class="key" onclick="testKey('9')">9</div>
            <div class="key" onclick="testKey('0')">0</div>
        </div>
        <div class="row">
            <div class="key" onclick="testKey('Q')">Q</div>
            <div class="key" onclick="testKey('W')">W</div>
            <div class="key" onclick="testKey('E')">E</div>
            <div class="key" onclick="testKey('R')">R</div>
            <div class="key" onclick="testKey('T')">T</div>
            <div class="key" onclick="testKey('Y')">Y</div>
            <div class="key" onclick="testKey('U')">U</div>
            <div class="key" onclick="testKey('I')">I</div>
            <div class="key" onclick="testKey('O')">O</div>
            <div class="key" onclick="testKey('P')">P</div>
        </div>
        <!-- Add more rows of keys as needed -->
    </div>
    <div id="output"></div>

    <script>
        function testKey(key) {
            const output = document.getElementById('output');
            output.innerHTML = `<p>You pressed: ${key}</p>`;
        }
    </script>
</body>
</html>
