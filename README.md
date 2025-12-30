<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Chat UI</title>
  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      font-family:Arial, Helvetica, sans-serif;
    }

    body{
      background:#e5ddd5;
      display:flex;
      justify-content:center;
      align-items:center;
      height:100vh;
    }

    .chat-container{
      width:360px;
      height:600px;
      background:#fff;
      border-radius:15px;
      box-shadow:0 10px 25px rgba(0,0,0,0.2);
      display:flex;
      flex-direction:column;
      overflow:hidden;
    }

    /* Header */
    .chat-header{
      background:#075e54;
      color:#fff;
      padding:15px;
      display:flex;
      align-items:center;
      gap:10px;
    }

    .chat-header img{
      width:40px;
      height:40px;
      border-radius:50%;
    }

    .chat-header h4{
      font-size:16px;
    }

    .chat-header p{
      font-size:12px;
      opacity:0.8;
    }

    /* Messages */
    .chat-messages{
      flex:1;
      padding:15px;
      background:#0e0d0d;
      overflow-y:auto;
    }

    .message{
      max-width:70%;
      padding:10px 14px;
      margin-bottom:10px;
      border-radius:10px;
      font-size:14px;
      line-height:1.4;
      clear:both;
    }

    .received{
      background:#efe1e1;
      float:left;
      border-top-left-radius:0;
    }

    .sent{
      background:#dcf8c6;
      float:right;
      border-top-right-radius:0;
    }

    /* Footer */
    .chat-input{
      display:flex;
      padding:10px;
      background:#f0e9e9;
      align-items:center;
      gap:10px;
    }

    .chat-input input{
      flex:1;
      padding:10px 15px;
      border:none;
      border-radius:20px;
      outline:none;
    }

    .chat-input button{
      background:#075e54;
      border:none;
      color:#e7dcdc;
      padding:10px 15px;
      border-radius:50%;
      cursor:pointer;
    }

    .chat-input button:hover{
      background:#0b806f;
    }
  </style>
</head>
<body>

  <div class="chat-container">
    <!-- Header -->
    <div class="chat-header">
      <img src="908f76ea93c49062710f069f582421e1.jpg" alt="user" />
      <div>
        <h4>Alex</h4>
        <p>online</p>
      </div>
    </div>

    <!-- Messages -->
    <div class="chat-messages">
      <div class="message received">Hi 👋</div>
      <div class="message received">How are you?</div>
      <div class="message sent">Hi! I'm good 😊</div>
      <div class="message sent">What about you?</div>
      <div class="message received">Doing great 👍</div>
    </div>

    <!-- Input -->
    <div class="chat-input">
      <input type="text" placeholder="Type a message" />
      <button>➤</button>
    </div>
  </div>

</body>
</html>
