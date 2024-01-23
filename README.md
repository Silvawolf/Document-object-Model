# Document-object-Model
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>DOM Manipulation Example</title>
  <style>
    .highlight {
      color: red;
      font-weight: bold;
    }
  </style>
</head>
<body>

  <h1 id="main-heading">Welcome to DOM Manipulation</h1>
  <p id="demo-paragraph">This is a sample paragraph.</p>
  <button id="change-content-btn">Change Content</button>

  <script>
    // Accessing elements in the DOM
    const headingElement = document.getElementById('main-heading');
    const paragraphElement = document.getElementById('demo-paragraph');
    const buttonElement = document.getElementById('change-content-btn');

    // Changing content and style
    headingElement.textContent = 'New Heading';
    paragraphElement.innerHTML = 'This paragraph has been <span class="highlight">modified</span>.';

    // Adding an event listener to the button
    buttonElement.addEventListener('click', function() {
      // Changing content and style dynamically on button click
      headingElement.textContent = 'Content Changed!';
      paragraphElement.classList.add('highlight');
    });
  </script>

</body>
</html>
