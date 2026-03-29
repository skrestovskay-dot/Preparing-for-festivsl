<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
    <title>Phonics Warm-Up | Funny Festival Speech | Grade 3 ESL</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Comic Neue', 'Segoe UI', 'Comic Neue', 'Comic Sans MS', cursive, sans-serif;
            background: linear-gradient(135deg, #FFDEE9 0%, #B5FFFC 100%);
            min-height: 100vh;
            padding: 20px;
        }

        .container {
            max-width: 1400px;
            margin: 0 auto;
        }

        /* Funny characters floating animation */
        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-15px); }
        }

        @keyframes bounce {
            0%, 100% { transform: translateX(0px); }
            50% { transform: translateX(10px); }
        }

        @keyframes wiggle {
            0%, 100% { transform: rotate(0deg); }
            25% { transform: rotate(5deg); }
            75% { transform: rotate(-5deg); }
        }

        @keyframes spin {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }

        @keyframes jump {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-20px); }
        }

        .float-emoji {
            animation: float 3s ease-in-out infinite;
            display: inline-block;
        }

        .bounce-emoji {
            animation: bounce 2s ease-in-out infinite;
            display: inline-block;
        }

        .wiggle-emoji {
            animation: wiggle 1.5s ease-in-out infinite;
            display: inline-block;
        }

        .spin-emoji {
            animation: spin 4s linear infinite;
            display: inline-block;
        }

        .header {
            text-align: center;
            margin-bottom: 20px;
            background: rgba(255,255,255,0.9);
            padding: 20px;
            border-radius: 60px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
        }

        .header h1 {
            font-size: 2rem;
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            margin-bottom: 5px;
        }

        .header p {
            color: #555;
            font-size: 0.9rem;
        }

        .funny-characters {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 15px;
            flex-wrap: wrap;
        }

        .funny-char {
            font-size: 2.5rem;
            cursor: pointer;
            transition: all 0.3s;
            background: white;
            padding: 10px 20px;
            border-radius: 60px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .funny-char:hover {
            transform: scale(1.2);
            background: #f0f0f0;
        }

        .exercise-card {
            background: white;
            border-radius: 50px;
            padding: 25px;
            margin-bottom: 20px;
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
            transition: all 0.3s;
            position: relative;
            overflow: hidden;
        }

        .exercise-card::before {
            content: "🎉";
            position: absolute;
            top: 10px;
            right: 10px;
            font-size: 3rem;
            opacity: 0.1;
            pointer-events: none;
        }

        .exercise-card:hover {
            transform: translateY(-5px);
        }

        .exercise-header {
            display: flex;
            align-items: center;
            gap: 15px;
            margin-bottom: 20px;
            flex-wrap: wrap;
        }

        .exercise-number {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            font-weight: bold;
        }

        .exercise-title {
            font-size: 1.4rem;
            color: #2c3e50;
            flex: 1;
        }

        .sound-icon {
            font-size: 2rem;
            cursor: pointer;
            transition: transform 0.2s;
        }

        .sound-icon:hover {
            transform: scale(1.1);
        }

        .sound-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
            justify-content: center;
            margin: 20px 0;
        }

        .sound-card {
            background: linear-gradient(135deg, #e0c3fc 0%, #8ec5fc 100%);
            border-radius: 30px;
            padding: 20px;
            text-align: center;
            cursor: pointer;
            transition: all 0.3s;
            min-width: 140px;
            position: relative;
            overflow: hidden;
        }

        .sound-card:hover {
            transform: scale(1.05) rotate(2deg);
            box-shadow: 0 15px 30px rgba(0,0,0,0.2);
        }

        .sound-card:active {
            transform: scale(0.98);
        }

        .sound-letter {
            font-size: 2.5rem;
            font-weight: bold;
            margin-bottom: 10px;
        }

        .sound-word {
            font-size: 1.1rem;
            color: #2c3e50;
        }

        .sound-picture {
            font-size: 2rem;
            margin-top: 10px;
        }

        .phrase-card {
            background: linear-gradient(135deg, #ffe6f0 0%, #ffd6e0 100%);
            border-radius: 30px;
            padding: 15px;
            text-align: center;
            cursor: pointer;
            transition: all 0.3s;
            min-width: 200px;
            position: relative;
        }

        .phrase-card:hover {
            transform: scale(1.02) translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }

        .phrase-text {
            font-size: 1.2rem;
            font-weight: bold;
            color: #c0392b;
        }

        .lip-exercise {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
        }

        .lip-card {
            background: #f8f9ff;
            border-radius: 30px;
            padding: 20px;
            text-align: center;
            cursor: pointer;
            transition: all 0.3s;
            min-width: 150px;
            border: 3px solid transparent;
        }

        .lip-card:hover {
            border-color: #f5576c;
            transform: translateY(-10px) rotate(2deg);
            background: #fff0f5;
        }

        .lip-emoji {
            font-size: 3rem;
            margin-bottom: 10px;
            display: inline-block;
        }

        .lip-sound {
            font-size: 1.8rem;
            font-weight: bold;
            color: #667eea;
            margin: 10px 0;
        }

        .tongue-box {
            background: linear-gradient(135deg, #ffe6f0 0%, #ffd6e0 100%);
            border-radius: 40px;
            padding: 25px;
            text-align: center;
            margin: 15px 0;
            position: relative;
        }

        .tongue-text {
            font-size: 1.5rem;
            font-weight: bold;
            color: #c0392b;
            margin-bottom: 15px;
        }

        .repeat-btn {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            border: none;
            padding: 10px 25px;
            border-radius: 60px;
            font-size: 1rem;
            cursor: pointer;
            font-family: inherit;
            margin: 5px;
            transition: all 0.3s;
        }

        .repeat-btn:hover {
            transform: scale(1.05);
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }

        .progress-container {
            margin-top: 20px;
        }

        .progress-label {
            display: flex;
            justify-content: space-between;
            margin-bottom: 8px;
            font-size: 0.9rem;
        }

        .progress-bar-bg {
            background: #e0e0e0;
            border-radius: 20px;
            height: 10px;
            overflow: hidden;
        }

        .progress-fill {
            background: linear-gradient(135deg, #11998e 0%, #38ef7d 100%);
            height: 100%;
            width: 0%;
            transition: width 0.5s ease;
            border-radius: 20px;
        }

        .complete-btn {
            background: linear-gradient(135deg, #11998e 0%, #38ef7d 100%);
            color: white;
            border: none;
            padding: 15px 40px;
            border-radius: 60px;
            font-size: 1.2rem;
            font-weight: bold;
            cursor: pointer;
            display: block;
            margin: 20px auto 0;
            font-family: inherit;
            transition: all 0.3s;
        }

        .complete-btn:hover {
            transform: scale(1.05);
            box-shadow: 0 10px 20px rgba(0,0,0,0.2);
        }

        .celebration {
            text-align: center;
            padding: 30px;
            background: linear-gradient(135deg, #ffe6f0 0%, #ffd6e0 100%);
            border-radius: 40px;
            margin-top: 20px;
        }

        .festival-teaser {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            border-radius: 40px;
            padding: 25px;
            margin-top: 20px;
            text-align: center;
        }

        .festival-teaser h3 {
            font-size: 1.8rem;
            margin-bottom: 15px;
        }

        .festival-buttons {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
            justify-content: center;
        }

        .festival-btn {
            background: white;
            color: #667eea;
            border: none;
            padding: 12px 25px;
            border-radius: 60px;
            font-size: 1rem;
            font-weight: bold;
            cursor: pointer;
            transition: all 0.3s;
        }

        .festival-btn:hover {
            transform: scale(1.05);
            background: #f093fb;
            color: white;
        }

        .hidden {
            display: none;
        }

        .checkmark {
            font-size: 1.5rem;
            margin-left: 10px;
        }

        .breathing-circle {
            width: 150px;
            height: 150px;
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            border-radius: 50%;
            margin: 20px auto;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            transition: all 0.3s;
        }

        @keyframes breathe {
            0%, 100% { transform: scale(1); opacity: 0.7; }
            50% { transform: scale(1.2); opacity: 1; }
        }

        .animate-breathe {
            animation: breathe 4s ease-in-out infinite;
        }

        .festival-word {
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            color: white;
            padding: 5px 12px;
            border-radius: 30px;
            display: inline-block;
            margin: 5px;
        }

        /* Funny GIF replacements */
        .funny-gif {
            font-size: 3rem;
            display: inline-block;
            transition: all 0.3s;
        }

        .funny-gif:hover {
            transform: scale(1.3);
        }

        .dancing-monkey {
            animation: bounce 1s ease-in-out infinite;
            display: inline-block;
            font-size: 2.5rem;
        }

        @keyframes shake {
            0%, 100% { transform: translateX(0); }
            25% { transform: translateX(-5px); }
            75% { transform: translateX(5px); }
        }

        .shake {
            animation: shake 0.3s ease-in-out;
        }

        @media (max-width: 700px) {
            .exercise-card {
                padding: 15px;
            }
            .sound-letter {
                font-size: 1.8rem;
            }
            .phrase-text {
                font-size: 1rem;
            }
            .festival-teaser h3 {
                font-size: 1.4rem;
            }
            .funny-char {
                font-size: 1.5rem;
                padding: 5px 12px;
            }
        }
    </style>
</head>
<body>
<div class="container">
    <div class="header">
        <h1>🗣️ Let's Warm Up Our Mouth! 🎤</h1>
        <p>Today we will learn about <span class="festival-word">🎭 FESTIVALS</span> around the world!</p>
        
        <!-- Funny characters for good mood -->
        <div class="funny-characters">
            <div class="funny-char" onclick="playFunnySound('monkey')">
                <span class="float-emoji">🐒</span> <span class="wiggle-emoji">🙈</span> <span class="bounce-emoji">🙉</span>
            </div>
            <div class="funny-char" onclick="playFunnySound('dance')">
                <span class="spin-emoji">💃</span> <span class="float-emoji">🕺</span>
            </div>
            <div class="funny-char" onclick="playFunnySound('alien')">
                <span class="bounce-emoji">👽</span> <span class="wiggle-emoji">🤪</span>
            </div>
            <div class="funny-char" onclick="playFunnySound('cat')">
                <span class="float-emoji">🐱</span> <span class="spin-emoji">🐶</span> <span class="bounce-emoji">🐭</span>
            </div>
        </div>
    </div>

    <!-- Exercise 1: Breathing with funny animal -->
    <div class="exercise-card" id="exercise1">
        <div class="exercise-header">
            <div class="exercise-number">1</div>
            <div class="exercise-title">🌬️ Breathing with Funny Frog 🐸</div>
            <div class="sound-icon" onclick="speak('Breathe in through your nose, breathe out through your mouth. Like a happy frog!')">🔊</div>
        </div>
        <div class="exercise-content" style="text-align: center;">
            <p>💨 Breathe like a <span class="float-emoji" style="font-size:2rem;">🐸</span> frog! In... and out... Let's get ready for <strong class="festival-word">FESTIVALS</strong>! 💨</p>
            <div class="breathing-circle" id="breathingCircle" onclick="startBreathing()">
                <div class="breathing-text" style="color:white; font-weight:bold;">🐸 Ribbit!<br>Breathe</div>
            </div>
            <p>👃 Inhale... (1,2,3,4) like a frog puffing up!<br>👄 Exhale... (1,2,3,4,5,6) like a frog relaxing!</p>
            <button class="repeat-btn" onclick="startBreathing()">Start Breathing with Frog 🐸</button>
        </div>
    </div>

    <!-- Exercise 2: Vowel Sounds with Funny Animals -->
    <div class="exercise-card" id="exercise2">
        <div class="exercise-header">
            <div class="exercise-number">2</div>
            <div class="exercise-title">🎵 Vowel Sounds + Funny Animals 🦁</div>
            <div class="sound-icon" onclick="speak('Let's practice vowel sounds with funny animals! A, E, I, O, U. Repeat after me!')">🔊</div>
        </div>
        <div class="exercise-content">
            <div class="sound-grid">
                <div class="sound-card" onclick="saySoundWithAnimal('A a', 'Apple', '/æ/', 'Apple apple apple', '🐒 Monkey says A!')">
                    <div class="sound-letter">A a <span class="float-emoji">🐒</span></div>
                    <div class="sound-word">Apple 🍎</div>
                    <div class="sound-picture">/æ/</div>
                </div>
                <div class="sound-card" onclick="saySoundWithAnimal('E e', 'Elephant', '/e/', 'Elephant elephant elephant', '🐘 Elephant says E!')">
                    <div class="sound-letter">E e <span class="wiggle-emoji">🐘</span></div>
                    <div class="sound-word">Elephant 🐘</div>
                    <div class="sound-picture">/e/</div>
                </div>
                <div class="sound-card" onclick="saySoundWithAnimal('I i', 'Iguana', '/ɪ/', 'Iguana iguana iguana', '🦎 Iguana says I!')">
                    <div class="sound-letter">I i <span class="bounce-emoji">🦎</span></div>
                    <div class="sound-word">Iguana 🦎</div>
                    <div class="sound-picture">/ɪ/</div>
                </div>
                <div class="sound-card" onclick="saySoundWithAnimal('O o', 'Octopus', '/ɒ/', 'Octopus octopus octopus', '🐙 Octopus says O!')">
                    <div class="sound-letter">O o <span class="spin-emoji">🐙</span></div>
                    <div class="sound-word">Octopus 🐙</div>
                    <div class="sound-picture">/ɒ/</div>
                </div>
                <div class="sound-card" onclick="saySoundWithAnimal('U u', 'Umbrella bird', '/ʌ/', 'Umbrella umbrella umbrella', '🐦 Umbrella bird says U!')">
                    <div class="sound-letter">U u <span class="float-emoji">🐦</span></div>
                    <div class="sound-word">Umbrella Bird ☔🐦</div>
                    <div class="sound-picture">/ʌ/</div>
                </div>
            </div>
        </div>
    </div>

    <!-- Exercise 3: Festival Words with Funny Pictures -->
    <div class="exercise-card" id="exercise3">
        <div class="exercise-header">
            <div class="exercise-number">3</div>
            <div class="exercise-title">🎪 Festival Words + Silly Characters 🤪</div>
            <div class="sound-icon" onclick="speak('Let's learn festival words with silly characters! Mask, bells, tomato, altar, costume, parade, music, dance, flower, spirit. Repeat!')">🔊</div>
        </div>
        <div class="exercise-content">
            <div class="sound-grid">
                <div class="sound-card" onclick="sayFestivalWordFunny('Mask', 'Mask', '/mæsk/', '🎭 Wear a funny mask! BOO! 👻')">
                    <div class="sound-letter">🎭 <span class="wiggle-emoji">👻</span></div>
                    <div class="sound-word">Mask</div>
                    <div class="sound-picture">/mæsk/</div>
                </div>
                <div class="sound-card" onclick="sayFestivalWordFunny('Bells', 'Bells', '/belz/', '🔔 Ding dong! Silly bells! 🎄')">
                    <div class="sound-letter">🔔 <span class="bounce-emoji">🛷</span></div>
                    <div class="sound-word">Bells</div>
                    <div class="sound-picture">/belz/</div>
                </div>
                <div class="sound-card" onclick="sayFestivalWordFunny('Tomato', 'Tomato', '/təˈmɑːtəʊ/', '🍅 Squishy tomato! SPLAT! 💥')">
                    <div class="sound-letter">🍅 <span class="float-emoji">💥</span></div>
                    <div class="sound-word">Tomato</div>
                    <div class="sound-picture">/təˈmɑːtəʊ/</div>
                </div>
                <div class="sound-card" onclick="sayFestivalWordFunny('Altar', 'Altar', '/ˈɔːltə/', '🕯️ Magic altar with flowers! ✨')">
                    <div class="sound-letter">🕯️ <span class="spin-emoji">✨</span></div>
                    <div class="sound-word">Altar</div>
                    <div class="sound-picture">/ˈɔːltə/</div>
                </div>
                <div class="sound-card" onclick="sayFestivalWordFunny('Costume', 'Costume', '/ˈkɒstjuːm/', '👘 Funny costume! Look at me! 🤡')">
                    <div class="sound-letter">👘 <span class="wiggle-emoji">🤡</span></div>
                    <div class="sound-word">Costume</div>
                    <div class="sound-picture">/ˈkɒstjuːm/</div>
                </div>
                <div class="sound-card" onclick="sayFestivalWordFunny('Parade', 'Parade', '/pəˈreɪd/', '🎺 March in the parade! Toot toot! 🎵')">
                    <div class="sound-letter">🎺 <span class="bounce-emoji">🎵</span></div>
                    <div class="sound-word">Parade</div>
                    <div class="sound-picture">/pəˈreɪd/</div>
                </div>
                <div class="sound-card" onclick="sayFestivalWordFunny('Music', 'Music', '/ˈmjuːzɪk/', '🎵 Dance to the music! Boogie woogie! 💃')">
                    <div class="sound-letter">🎵 <span class="float-emoji">💃</span></div>
                    <div class="sound-word">Music</div>
                    <div class="sound-picture">/ˈmjuːzɪk/</div>
                </div>
                <div class="sound-card" onclick="sayFestivalWordFunny('Dance', 'Dance', '/dɑːns/', '💃 Dance like a chicken! 🐔🕺')">
                    <div class="sound-letter">💃 <span class="spin-emoji">🐔</span></div>
                    <div class="sound-word">Dance</div>
                    <div class="sound-picture">/dɑːns/</div>
                </div>
                <div class="sound-card" onclick="sayFestivalWordFunny('Flower', 'Flower', '/ˈflaʊə/', '🌼 Smell the flower! ACHOO! 🤧')">
                    <div class="sound-letter">🌼 <span class="wiggle-emoji">🤧</span></div>
                    <div class="sound-word">Flower</div>
                    <div class="sound-picture">/ˈflaʊə/</div>
                </div>
                <div class="sound-card" onclick="sayFestivalWordFunny('Spirit', 'Spirit', '/ˈspɪrɪt/', '👻 Boo! A friendly spirit! Hi! 👋')">
                    <div class="sound-letter">👻 <span class="float-emoji">👋</span></div>
                    <div class="sound-word">Spirit</div>
                    <div class="sound-picture">/ˈspɪrɪt/</div>
                </div>
            </div>
        </div>
    </div>

    <!-- Exercise 4: Funny Festival Phrases -->
    <div class="exercise-card" id="exercise4">
        <div class="exercise-header">
            <div class="exercise-number">4</div>
            <div class="exercise-title">😂 Funny Festival Phrases 😂</div>
            <div class="sound-icon" onclick="speak('Let's practice funny phrases about festivals! Repeat with a smile!')">🔊</div>
        </div>
        <div class="exercise-content">
            <div class="sound-grid">
                <div class="phrase-card" onclick="sayFunnyPhrase('I love festivals!', 'I love festivals! Yay yay yay! Festivals are the best! 🎉')">
                    <div class="phrase-text">🎪 I love festivals! <span class="float-emoji">🎉</span></div>
                </div>
                <div class="phrase-card" onclick="sayFunnyPhrase('Let\'s party!', 'Let\'s party! Woohoo! Dance dance dance! 🕺💃')">
                    <div class="phrase-text">🎈 Let's party! <span class="spin-emoji">🕺</span></div>
                </div>
                <div class="phrase-card" onclick="sayFunnyPhrase('Look at that funny mask!', 'Look at that funny mask! Hahaha! It is so silly! 🤪🎭')">
                    <div class="phrase-text">🎭 Look at that funny mask! <span class="wiggle-emoji">🤪</span></div>
                </div>
                <div class="phrase-card" onclick="sayFunnyPhrase('Tomato on my nose!', 'Tomato on my nose! Squish squash! So messy! 🍅👃')">
                    <div class="phrase-text">🍅 Tomato on my nose! <span class="bounce-emoji">👃</span></div>
                </div>
                <div class="phrase-card" onclick="sayFunnyPhrase('Dancing like a monkey!', 'Dancing like a monkey! Ooh ooh ah ah! Watch me dance! 🐒💃')">
                    <div class="phrase-text">🐒 Dancing like a monkey! <span class="float-emoji">🐒</span></div>
                </div>
                <div class="phrase-card" onclick="sayFunnyPhrase('Happy festival everyone!', 'Happy festival everyone! Let\'s eat cake! Yummy! 🎂🎉')">
                    <div class="phrase-text">🎉 Happy festival everyone! <span class="spin-emoji">🎂</span></div>
                </div>
            </div>
        </div>
    </div>

    <!-- Exercise 5: Silly Tongue Twisters -->
    <div class="exercise-card" id="exercise5">
        <div class="exercise-header">
            <div class="exercise-number">5</div>
            <div class="exercise-title">😜 Silly Festival Tongue Twisters 😜</div>
            <div class="sound-icon" onclick="speak(sillyTwisters[currentTongueIndex].sound)">🔊</div>
        </div>
        <div class="exercise-content">
            <div class="tongue-box">
                <div class="tongue-text" id="tongueText">🐒 Funny monkeys make music at the festival! 🎵</div>
                <div>
                    <button class="repeat-btn" onclick="saySillyTwister(currentTongueIndex)">🔊 Listen & Laugh</button>
                    <button class="repeat-btn" onclick="nextSillyTwister()">➡️ Next Silly One</button>
                </div>
            </div>
            <p style="text-align: center; font-size: 0.9rem;">✨ Say each twister 3 times fast with a big smile! ✨</p>
        </div>
    </div>

    <!-- Exercise 6: Funny Face Exercises -->
    <div class="exercise-card" id="exercise6">
        <div class="exercise-header">
            <div class="exercise-number">6</div>
            <div class="exercise-title">🤪 Make Funny Faces for Festival Words! 🤪</div>
            <div class="sound-icon" onclick="speak('Let's make funny faces while practicing festival words!')">🔊</div>
        </div>
        <div class="exercise-content">
            <div class="lip-exercise">
                <div class="lip-card" onclick="makeFunnyFace('smile', '😁 Big smile! Say Festival! Feees-tii-val! 😁')">
                    <div class="lip-emoji">😁➡️😆➡️😄</div>
                    <div class="lip-sound">Fes - ti - val!</div>
                    <div class="lip-word">Big Smile Festival!</div>
                </div>
                <div class="lip-card" onclick="makeFunnyFace('fish', '🐟 Fish face! Pucker up! Say Mask! Maa-aa-sk 🎭')">
                    <div class="lip-emoji">🐟👄</div>
                    <div class="lip-sound">Maa - sk!</div>
                    <div class="lip-word">Fish Face Mask!</div>
                </div>
                <div class="lip-card" onclick="makeFunnyFace('tongue', '👅 Tongue out! Say Tomato! Ta-ma-to! 🍅')">
                    <div class="lip-emoji">😛👅</div>
                    <div class="lip-sound">To - ma - to!</div>
                    <div class="lip-word">Tongue Out Tomato!</div>
                </div>
                <div class="lip-card" onclick="makeFunnyFace('monkey', '🐒 Monkey face! Ooh ooh! Say Parade! Pa-rade! 🎺')">
                    <div class="lip-emoji">🐒🙊</div>
                    <div class="lip-sound">Pa - rade!</div>
                    <div class="lip-word">Monkey Parade!</div>
                </div>
                <div class="lip-card" onclick="makeFunnyFace('crazy', '🤪 Crazy eyes! Say Celebration! Cele-bra-tion! 🎉')">
                    <div class="lip-emoji">🤪🌀</div>
                    <div class="lip-sound">Cele - bra - tion!</div>
                    <div class="lip-word">Crazy Celebration!</div>
                </div>
                <div class="lip-card" onclick="makeFunnyFace('surprise', '😲 Surprise face! Say Wow! WOW Festival! 🎊')">
                    <div class="lip-emoji">😲➡️😮➡️😯</div>
                    <div class="lip-sound">WOW!</div>
                    <div class="lip-word">Surprise Festival!</div>
                </div>
            </div>
        </div>
    </div>

    <!-- Progress and Complete -->
    <div class="exercise-card">
        <div class="progress-container">
            <div class="progress-label">
                <span>🎯 Warm-up Progress (6 funny exercises)</span>
                <span id="progressPercent">0%</span>
            </div>
            <div class="progress-bar-bg">
                <div class="progress-fill" id="progressFill"></div>
            </div>
        </div>
        <button class="complete-btn" id="completeBtn">✅ Ready for Festivals! 🎉 ✅</button>
    </div>

    <!-- Celebration + Transition to Festivals -->
    <div id="celebration" class="celebration hidden">
        <h2>🎉 Amazing Funny Job! 🎉</h2>
        <div style="font-size: 3rem; margin: 15px;">
            <span class="float-emoji">🎭</span>
            <span class="spin-emoji">🎪</span>
            <span class="bounce-emoji">🎉</span>
            <span class="wiggle-emoji">🍅</span>
            <span class="float-emoji">🎵</span>
        </div>
        <p>You made funny faces and practiced festival words!</p>
        <p>🌟 Your mouth is SUPER ready to learn about <strong>FESTIVALS AROUND THE WORLD</strong>! 🌟</p>
        
        <div class="festival-teaser">
            <h3>🎭 Ready for a FUNNY festival trip? 🌎</h3>
            <p>Let's visit <strong>3 amazing festivals</strong> with silly characters!</p>
            <div class="festival-buttons">
                <div class="festival-btn" onclick="showFestival('bulgaria')">🇧🇬 Kukeri 🤪🎭</div>
                <div class="festival-btn" onclick="showFestival('mexico')">🇲🇽 Day of the Dead 💀🌼</div>
                <div class="festival-btn" onclick="showFestival('spain')">🇪🇸 La Tomatina 🍅💥</div>
            </div>
            <p style="margin-top: 20px; font-size: 0.9rem;">👉 Click on any festival to start the main lesson! 👈</p>
        </div>
        
        <button class="repeat-btn" style="margin-top: 20px;" onclick="closeCelebration()">Start Main Lesson 📖</button>
    </div>
</div>

<script>
    let completed = {
        exercise1: false, exercise2: false, exercise3: false,
        exercise4: false, exercise5: false, exercise6: false
    };
    
    let currentTongueIndex = 0;
    const sillyTwisters = [
        { text: "🐒 Funny monkeys make music at the festival! 🎵", sound: "Funny monkeys make music at the festival! Funny monkeys! Ooh ooh!" },
        { text: "🎭 Silly Sally sells scary masks at the market 🎭", sound: "Silly Sally sells scary masks at the market! Silly Sally!" },
        { text: "🍅 Ten ticklish tomatoes tumbled on the table 🍅", sound: "Ten ticklish tomatoes tumbled on the table! Hahaha!" },
        { text: "🔔 Big
