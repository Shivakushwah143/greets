

code file

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Greeting</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            min-height: 100vh; /* Set minimum height for full viewport */
            /* background-color: #f5f5f5; */
            background-color: aquamarine;
        }
        h1 {
            font-size: 2em;
            margin-bottom: 20px;
        }
        #greeting {
            font-size: 1.5em;
            margin-bottom: 10px;
        }
        #name-input {
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 1em;
        }
        #greet-button {
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            background-color: #333;
            color: #fff;
            cursor: pointer;
            font-size: 1em;
            margin-top: 10px;
        }
        #greet-button:hover {
            background-color: #444;
        }
        .image-container {
            margin-bottom: 20px;
        }
        img {
            width: 200px; /* Adjust image width as needed */
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <h1>Interactive Greeting</h1>
    <div class="image-container">
        <img src="https://www.shutterstock.com/shutterstock/photos/1766312297/display_1500/stock-vector-we-wish-you-all-the-best-birthday-greeting-quote-lettering-typography-phrase-by-hand-with-speech-1766312297.jpg" alt="Greeting Image">
    </div>
    <p id="greeting"></p>
    <input type="text" id="name-input" placeholder="Enter your name">
    <button id="greet-button">Greet Me!</button>
    <script>
        const greetingElement = document.getElementById('greeting');
        const nameInput = document.getElementById('name-input');
        const greetButton = document.getElementById('greet-button');

        greetButton.addEventListener('click', function() {
          const name = nameInput.value.trim();
          if (name) {
            greetingElement.textContent = `Hello, ${name}!`;
            nameInput.value = ''; // Clear the input field after greeting
          } else {
            alert("Please enter your name!");
          }
        });
    </script>
</body>
</html>
# greets
