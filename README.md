# friend-site

<html>
<head>
  <title>Friendship Question</title>
  <style>
    body {
      font-family: "Comic Sans MS", cursive, sans-serif;
      background-color: #ffeef2;
      text-align: center;
      padding: 60px;
    }

    h1 {
      font-size: 28px;
      color: #d6336c;
    }

    button {
      padding: 15px 30px;
      margin: 15px;
      font-size: 18px;
      border: none;
      border-radius: 12px;
      background-color: #f08080;
      color: white;
      cursor: pointer;
      transition: 0.3s ease;
    }

    button:hover {
      background-color: #ff5c5c;
    }

    #response {
      margin-top: 40px;
      font-size: 24px;
      color: #8e44ad;
    }
  </style>
</head>
<body>

  <h1>Question: Do you wanna be my friend?</h1>

  <button onclick="reply('yes')">Yes</button>
  <button onclick="reply('no')">No</button>

  <div id="response"></div>

  <script>
    function reply(answer) {
      const response = document.getElementById('response');
      if (answer === 'yes') {
        response.innerText = 'Yayy! 💖😊';
      } else {
        response.innerText = 'Awhh you sure? 😢';
      }
    }
  </script>

</body>
</html>
