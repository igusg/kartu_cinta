<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>Kartu Cinta Untukmu ❤️</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      margin: 0;
      padding: 0;
      background: linear-gradient(to top right, #ffccd5, #ffe4ec);
      font-family: 'Segoe UI', sans-serif;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      min-height: 100vh;
      color: #d6336c;
      text-align: center;
    }

    .heart {
      font-size: 60px;
      animation: pulse 1s infinite;
    }

    @keyframes pulse {
      0%, 100% { transform: scale(1); }
      50% { transform: scale(1.2); }
    }

    .card {
      background-color: white;
      border-radius: 20px;
      padding: 30px;
      max-width: 500px;
      box-shadow: 0 0 15px rgba(0,0,0,0.1);
      margin: 20px;
    }

    .message {
      white-space: pre-line;
      margin-top: 20px;
      font-size: 1.2em;
    }

    button {
      margin-top: 30px;
      padding: 10px 20px;
      font-size: 1em;
      background-color: #ff85a2;
      color: white;
      border: none;
      border-radius: 8px;
      cursor: pointer;
    }

    button:hover {
      background-color: #ff4f7a;
    }

    footer {
      margin-top: 20px;
      font-size: 0.9em;
      color: #555;
    }
  </style>
</head>
<body>

  <div class="heart">❤️</div>
  <div class="card">
    <h2>Hai Kamu... 😊</h2>
    <div class="message" id="message"></div>
    <button onclick="nextMessage()">Lanjut</button>
  </div>

  <footer>
    Dibuat dengan ❤️ oleh seseorang yang mikirin kamu
  </footer>

  <script>
    const lines = [
      "Aku cuma mau bilang sesuatu...",
      "Sejak aku kenal kamu, hari-hariku jadi beda.",
      "Kamu itu kayak kunci dalam algoritma bahagia aku 🧠💘",
      "Setiap detik bareng kamu, kayak loop yang nggak pengen berhenti.",
      "Jadi... maukah kamu jadi pasangan `True` dalam hidupku? 😍"
    ];

    let index = 0;

    function nextMessage() {
      const msg = document.getElementById("message");
      if (index < lines.length) {
        msg.innerHTML += lines[index] + "\n\n";
        index++;
      } else {
        alert("Udah selesai, tapi rasa sayangnya nggak pernah selesai ❤️");
      }
    }
  </script>

</body>
</html>
