<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Birthday Celebration</title>
    <style>
        body {
            margin: 0;
            overflow: hidden;
            display: flex;
            justify-content: center;
            align-items: center;
            font-family: 'Arial', sans-serif;
        }
        .hidden {
            display: none;
        }
        .message {
            font-size: 2em;
            text-align: center;
            margin: 20px;
        }
        .background {
            position: absolute; 
            top: 0; 
            left: 0; 
            width: 100%; 
            height: 100%; 
            background: url('https://i.imgur.com/V7Pzi7k.png'); /* Y2K-style confetti */
            background-size: cover; 
            opacity: 0.9;
        }
        .button {
            padding: 10px 20px; 
            font-size: 1.5em; 
            cursor: pointer; 
            background-color: lightblue; 
            border: none; 
            border-radius: 5px; 
            margin: 10px;
        }
        .balloons {
            display: none;
            position: absolute; 
            top: 40%; 
            left: 50%; 
            transform: translate(-50%, -50%);
        }
        .cake {
            display: none;
            position: absolute; 
            top: 40%; 
            left: 50%; 
            transform: translate(-50%, -50%);
        }
        .lights {
            display: none;
            background-color: black;
            color: white;
            height: 100%;
            width: 100%;
        }
    </style>
</head>
<body>

    <div class="background"></div>
    
    <div id="content" class="message">
        <p id="mainMessage">It's your special day, yayaya!</p>
        <button id="nextButton" class="button">Next</button>
    </div>
    
    <div id="gifts" class="hidden message">
        <p>TO MAKE YOUR BIRTHDAY SPECIAL, I HAVE SOMETHING FOR YOU!</p>
        <button id="seeGiftButton" class="button">See Gift?</button>
        <button id="noGiftButton" class="button">No, thanks</button>
    </div>

    <div id="question" class="hidden message">
        <p>Do you want to see it?</p>
        <button id="yesButton" class="button">Yes</button>
        <button id="noButton" class="button">No</button>
    </div>

    <div id="lights" class="hidden lights">
        <p>Lights ON!</p>
        <button id="lightsOnButton" class="button">Turn On Lights!</button>
    </div>

    <div id="decorate" class="hidden message">
        <p>Let's decorate!</p>
        <button id="decorateButton" class="button">Happy Birthday!</button>
        <button id="noDecorateButton" class="button">No, thanks</button>
    </div>

    <div id="audioSection" class="hidden message">
        <p>Let's play music!</p>
        <button id="playMusicButton" class="button">Play</button>
    </div>

    <div id="cakeSection" class="hidden message">
        <p>Let's cut the cake!</p>
        <button id="yesToCakeButton" class="button">Yes!</button>
        <button id="noToCakeButton" class="button">No, thanks</button>
    </div>

    <div id="finalMessage" class="hidden message">
        <p style="font-weight: bold;">HAPPY BIRTHDAY DUDE! STAY BLESSED!</p>
    </div>
    
    <img src="https://i.imgur.com/2Hf3Dha.png" alt="Cake" class="cake" width="300" />
    <img src="https://i.imgur.com/PzhJTZx.png" alt="Balloons" class="balloons" width="300" />

    <audio id="happyBirthdayMusic" src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3"></audio>

    <script>
        const mainMessage = document.getElementById

