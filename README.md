
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>THE REALM</title>
  <style>
    body {
      background: black;
      color: white;
      font-family: 'Courier New', Courier, monospace;
      margin: 0;
      padding: 0;
    }
    nav {
      background: #100010;
      padding: 10px;
      border-bottom: 2px solid purple;
    }
    nav ul {
      display: flex;
      justify-content: space-around;
      list-style: none;
      margin: 0;
      padding: 0;
    }
    nav a {
      text-decoration: none;
      color: #87ceeb;
      font-weight: bold;
    }
    h2 {
      text-decoration: underline;
      color: gold;
    }
    section {
      padding: 20px;
    }
    .about, .myself, .blogs {
      background: linear-gradient(to bottom, #000000, #2e0854);
      margin-bottom: 20px;
    }
    img.small-img {
      width: 100px;
      height: auto;
      border-radius: 10px;
      border: 2px solid purple;
    }
    .spotify, .games, .quiz, .calendar {
      background: #111;
      color: #eee;
      padding: 20px;
      margin-bottom: 20px;
    }
    .adios {
      background: linear-gradient(to bottom, #2e0854, #000000);
      text-align: center;
      padding: 30px;
    }
    .game-box, .quiz-box {
      background: #222;
      padding: 15px;
      margin: 10px 0;
      border: 2px solid purple;
      border-radius: 10px;
    }
    .hunt-box {
  margin-top: 40px;
  padding: 20px;
  background-color: #1a001a;
  border: 2px dashed violet;
  color: white;
  position: relative;
}

.hunt-item {
  width: 40px;
  position: absolute;
  cursor: pointer;
  display: none;
  z-index: 10;
}

#item-bone { top: 120px; left: 60px; }
#item-vial { top: 200px; left: 300px; }
#item-herb { top: 350px; left: 180px; }

.hunt-box ul li.found {
  text-decoration: line-through;
  color: lime;
}
#scareContainer {
  display: none;
  position: fixed;
  top: 0;
  left: 0;
  width: 100vw;
  height: 100vh;
  background: rgba(0, 0, 0, 0.9);
  z-index: 9999;
  justify-content: center;
  align-items: center;
}

#scareContainer img {
  max-width: 80%;
  max-height: 80%;
  box-shadow: 0 0 30px red;
  animation: pulse 0.5s infinite alternate;
}

@keyframes pulse {
  from {
    transform: scale(1);
  }
  to {
    transform: scale(1.05);
  }
} 
#scareContainer {
  display: none;
  position: fixed;
  top: 0; left: 0;
  width: 100vw; height: 100vh;
  background: rgba(0, 0, 0, 0.95);
  z-index: 9999;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  animation: shake 0.3s ease-in-out infinite;
}

#scareImage {
  max-width: 80%;
  max-height: 80%;
  animation: pulse 0.5s infinite alternate;
  z-index: 10001;
}

#bloodFlash {
  position: absolute;
  top: 0; left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  z-index: 10000;
  display: none;
  animation: flash 0.5s ease;
}

@keyframes pulse {
  from { transform: scale(1); }
  to { transform: scale(1.05); }
}

@keyframes shake {
  0% { transform: translate(1px, 1px) rotate(0deg); }
  10% { transform: translate(-1px, -2px) rotate(-1deg); }
  20% { transform: translate(-3px, 0px) rotate(1deg); }
  30% { transform: translate(3px, 2px) rotate(0deg); }
  40% { transform: translate(1px, -1px) rotate(1deg); }
  50% { transform: translate(-1px, 2px) rotate(-1deg); }
  60% { transform: translate(-3px, 1px) rotate(0deg); }
  70% { transform: translate(3px, 1px) rotate(-1deg); }
  80% { transform: translate(-1px, -1px) rotate(1deg); }
  90% { transform: translate(1px, 2px) rotate(0deg); }
  100% { transform: translate(1px, -2px) rotate(-1deg); }
}

@keyframes flash {
  0% { opacity: 0; }
  50% { opacity: 0.8; }
  100% { opacity: 0; }
}
.vertical-nav {
  position: fixed;
  top: 0;
  left: 0;
  height: 100vh;
  width: 180px;
  background-color: #0b0019;
  padding-top: 40px;
  z-index: 1000;
  box-shadow: 4px 0 10px rgba(0, 0, 0, 0.7);
}

.vertical-nav ul {
  list-style-type: none;
  padding: 0;
  margin: 0;
}

.vertical-nav ul li {
  margin: 20px 0;
  text-align: center;
}

.vertical-nav ul li a {
  color: violet;
  text-decoration: none;
  font-family: 'Creepster', cursive;
  font-size: 18px;
  display: block;
  padding: 10px;
  transition: background 0.3s;
}

.vertical-nav ul li a:hover {
  background-color: #1e0033;
  color: white;
  text-shadow: 0 0 5px magenta;
  border-left: 4px solid violet;
}
body {
  margin-left: 180px; /* leaves room for vertical nav */
}
.echos-section {
  background-color: #0d0017;
  padding: 40px 20px;
  color: lavender;
  border-top: 2px solid violet;
  border-bottom: 2px solid violet;
}
.echos-section {
  background-color: #0d0017;
  padding: 40px 20px;
  color: lavender;
  border-top: 2px solid violet;
  border-bottom: 2px solid violet;
}

.echo-entry {
  margin-bottom: 30px;
  background-color: #1c002a;
  padding: 15px;
  border-left: 4px solid magenta;
  box-shadow: 0 0 10px rgba(255, 0, 255, 0.2);
}

.echo-entry h3 {
  font-family: 'Creepster', cursive;
  color: violet;
  margin-bottom: 10px;
  text-shadow: 0 0 3px magenta;
}
.echo-form {
  margin-top: 40px;
  background-color: #14001a;
  padding: 20px;
  border: 2px dashed violet;
  color: white;
  box-shadow: 0 0 10px rgba(200, 0, 255, 0.3);
}

.echo-form textarea {
  width: 100%;
  height: 100px;
  background-color: #1d002a;
  border: 1px solid violet;
  color: lavender;
  padding: 10px;
  font-family: 'Georgia', serif;
  margin-bottom: 10px;
}

.echo-form button {
  background-color: violet;
  color: black;
  font-weight: bold;
  border: none;
  padding: 8px 16px;
  cursor: pointer;
  transition: all 0.3s ease;
}

.echo-form button:hover {
  background-color: magenta;
  color: white;
  text-shadow: 0 0 5px black;
}

.user-echos {
  margin-top: 30px;
  background-color: #100014;
  padding: 15px;
  border-top: 1px solid magenta;
}

.user-echos .entry {
  background-color: #1c002a;
  margin-top: 10px;
  padding: 10px;
  color: lavender;
  border-left: 4px solid violet;
  font-style: italic;
}

</style>
</head>
<body>
  <nav class="vertical-nav">
  <ul>
    <li><a href="#home">🏠 Home</a></li>
    <li><a href="#about">🕯️ About</a></li>
    <li><a href="#myself">🧙‍♀️ Myself</a></li>
    <li><a href="#blogs">📜 Blogs</a></li>
    <li><a href="#games">🧩 Games</a></li>
    <li><a href="#echos">🫧 Echos</a></li>
    <li><a href="#playlist">🎶 Playlist</a></li>
    <li><a href="#adios">🔮 Adios</a></li>
  </ul>
  </nav>  <section id="home">
    <h2>Welcome to the Realm 🌒</h2>
    <p>Step into a space of magic, mystery, and fun. Welcome to my ghosty-cool web realm!</p>
  </section>  <section id="about" class="about">
    <h2>About Me</h2>
    <img src="file_0000000094d461f5a206b05a4e4ec2ed.png" alt="About image" class="small-img" />
    <p>I'm <strong>Kamakshi</strong>, your local gaming witch coder ✨. I build magic through code, poems, and pain. This place is all me — haunting, healing, and hella fun.</p>
  </section>  <section id="myself" class="myself">
    <h2>This Witchy</h2>
    <img src="5A6ABF91B5E13A4E907FE5B2CDCA7C31F748AD45" alt="Myself image" class="small-img" />
    <p>Hi there! I'm Kamakshi and this is my first time creating a website where I blog and maybe live. About myself I'm 18 and I'm very much interested in gaming and doing nothing but also a little bit of coding. I love making friends, and in person I maybe an extrovert but I'm not much confident if you ask me but that's ok. That's how life works right!?. I might not be perfect and neither is this website but I hope y'all like it 😄. Thanks for being here. Toodles!</p>
  </section>  <section id="blogs" class="blogs">
    <h2>Blogs</h2>
    <h3>Blog 1: 23/06/2025</h3>
    <p>Its been a rough day and while blaming god for everything that's happening in my life I realised what the actual problem was and so here I'm discussing about THE REAL PROBLEM......with this poem-----> There's nothing more important to me than to be... to live...to feel but still the question echoes: is it truly necessary? Alone without love, no tender care to cradle my heart, seeking souls to halt this solitude, but shadows chase me still, like demons dancing in the dark of my restless mind. The world once sparkled bright in solitary glow, but now I'm encircled by strangers whose hearts are void, each glance a dagger, every word a wound, they bury my hope deeper than any weapon can wound. Innocence was my shroud, believing in binds of closeness, convincing myself it’s me, that I’m the flaw, but no, no, no— I’m just a marionette, strings pulled for their delight, yet I’ve grown; perhaps my heart remains a timid child, screaming silently, longing to cry, longing to be whole, and still I know, the mirror reflects the problem within me, cause yes! the problem is me.....
</p>
    <h3>Blog 2: 24/06/2025</h3>
    <p>I've been realising lately that everything I do will never be enough or maybe...... I'M NOT ACTUALLY DOING ENOUGH------>

Crying in silence, running through pain, Screaming inside like a voice in the rain. I've given my all, done more than I could, Yet still I'm unseen, misunderstood.

For those that I love, I’ve carried the weight, Faced every storm, surrendered to fate. But they look at me with eyes so cold, And I’m lost in stories I've already told.

Lost in the past, in shadows I flee, Trapped in a place I never wished to be. I wonder aloud—what do I desire? When did my soul lose its fire?

I’ve become someone I never planned, A stranger shaped by unseen hands. Not cruel, not heartless, not a foe— Just tired, just broken, moving slow.

They say I’m wrong, they think I’m weak, But maybe I’m just too soft to speak. Maybe my love was never enough To heal the cracks, to smooth the rough.

I’ve searched within, I’ve tried my best, But some battles don’t end in rest. Now I stand with nothing left to prove, Just the ache of all I couldn’t move.

So if I seem like I’m drifting apart, Know it’s not hate—it’s a heavy heart. I gave my all, yet here I stand, Still wondering if I was ever enough... in anyone’s hands......
</p>
<h3>Blog 3: 25/06/2025</h3>
    <p>"Temporary"-->
I always knew who I was
a shadow I never truly liked.
Maybe God had plans to heal me,
or maybe… to break me twice.

Then you came—
like sunlight through a stormed sky,
told me I was special,
held me like no one else tried.
Loved me loud,
until I believed maybe I was worth it,
even though deep down,
I knew… it was temporary.

I’ve always feared the end.
The leaving.
The silence after "forever" fades.
And now I see it—
the slow turning of the tables,
the way your eyes no longer stay.

It’s not your fault.
I know.
But it still hurts to see you
look at me like the rest do—
like I’m the villain in a story
I never meant to write.

I want to let you go,
to watch you fly,
to see you smile even if
that smile isn’t mine.
But the selfish ache in me
clings to the memory
of when we were us
—not just me.

We promised, didn’t we?
To always be.
But even forever can be
just a fleeting dream.
And I thought knowing the end
would make it easier—
but I was wrong.

Now I can’t eat,
can’t sleep,
can’t even swallow
without pain sinking deep.
Each time your lips
speak another girl's name,
I swear—
it carves me like a flame.

I know I’m not enough.
Maybe I never was.
But you…
you deserved the stars,
and I was just a moment
on your map of Mars.

Still, those small, glowing moments—
even if they were just pixels and light—
were the best chapters of my life.

I’m sorry
for the chaos I brought.
I’m sorry
for being a storm you never sought.
But if love counts for anything—
I swear,
I loved you with all I had to give.

I just want to rewind—
just once—
to feel whole again.
But maybe this pain…
maybe it’s mine to bear.
Maybe I deserve it.

Maybe I was never meant
to be anything
but
Temporary.</p>
<section id="echos" class="echos-section">
  <h2 class="spooky-heading">🫧 Echos from Beyond</h2>
  <article class="echo-entry">
    <h3>“She Spoke at Midnight”</h3>
    <p>The spirit whispered through the mirror, revealing a secret forgotten by time...</p>
  </article>

  <article class="echo-entry">
    <h3>“Voices in the Fog”</h3>
    <p>I followed the sound… and found more than a voice waiting beyond the veil.</p>
  </article>
<div id="echo-submission" class="echo-form">
  <h3>🫧 Whisper Your Own Echo...</h3>
  <textarea id="userStory" placeholder="The spirit moved, and I heard it say..."></textarea>
  <button onclick="submitEcho()">Submit</button>
</div>

<div id="userEchos" class="user-echos">
  <h3>🔮 Other Echos</h3>
</div>
</section>
 <section id="mirror" class="spooky-mirror">
  <h2 class="spooky-heading">🪞 Haunted Mirror</h2>
  <p id="mirrorMessage">Peer into the mirror... what do you seek?</p>
  <button onclick="talkToSpirit()">Speak to the Spirit</button>
  </section>
  <section id="quiz" class="quiz">
    <h2>🔮 What Kind of Witch Are You?</h2>
    <div class="quiz-box">
      <p><strong>Q1:</strong> What time of day or place calls to your soul?</p>
<input type="radio" name="q1" value="forest" /> A misty forest at dawn 🌲<br />
<input type="radio" name="q1" value="storm" /> Thunderstorms in the evening 🌩️<br />
<input type="radio" name="q1" value="shadow" /> Midnight shadows 🌑<br />
<input type="radio" name="q1" value="fire" /> Blazing sunlight and fire rituals 🔥<br />
<input type="radio" name="q1" value="ice" /> Snow-covered silence ❄️<br />
<input type="radio" name="q1" value="sea" /> Waves crashing at night 🌊<br />
<input type="radio" name="q1" value="bone" /> Dusty bones and forgotten whispers 🦴<br />
<input type="radio" name="q1" value="cosmic" /> Stargazing from your window 💫<br />
      <button onclick="getWitchResult()">Reveal My Witch Type</button>
      <p id="witchResult"></p>
    </div>
  </section> 
  <div id="secretTrigger" style="text-align: center; margin: 60px 0;">
  <p style="color: #999;">
    ⚠️ <span onclick="triggerScare()" style="cursor: pointer; text-decoration: underline;">Do not click this</span>
  </p>
  <div id="scareContainer">
    <img
      id="scareImage"
      src="Horror.jpg"
      alt="Scary Face"
    />

  </div>
  </div>

  <section id="games" class="games">
    <h2>🕹️ Witchy Games</h2>
    <div class="game-box">
      <h3>🃏 Tarot Card Generator</h3>
      <button onclick="drawTarot()">Draw a Card</button>
      <p id="tarotResult"></p>
    </div>
    <div class="game-box">
      <h3>✨ Spell Generator</h3>
      <button onclick="generateSpell()">Cast Spell</button>
      <p id="spellResult"></p>
    </div>
    <div class="game-box">
      <h3>🧪 Potion Maker</h3>
      <button onclick="makePotion()">Brew Potion</button>
      <p id="potionResult"></p>
    </div>
    <div class="game-box">
      <h3>🔍 Hidden Object Game</h3>
      <p>Coming soon! (interactive room with items)</p>
    </div>
  </section>  <section id="calendar" class="calendar">
    <h2>🌕 Spooky Calendar</h2>
    <ul>
      <li>🌝 Full Moon – 21 July 2025</li>
      <li>🔮 Mercury Retrograde – 5 Aug to 28 Aug 2025</li>
      <li>🌑 New Moon – 4 August 2025</li>
      <li>🕯️ Witch's Market – 13 July 2025</li>
<li>💀 Ancestor Night – 31 October 2025</li>
<li>🧛 Blood Moon Eclipse – 8 November 2025</li>
<li>🎃 Samhain Festival – 31 October 2025</li>
<li>📿 Dark Spirit Portal Opening – 21 December 2025</li>
<li>🔔 Hex Hour – Every Friday the 13th</li>
    </ul>
  </section> 
  <section id="horoscope" class="horoscope-section">
  <h2 class="spooky-heading">🧿 Your Spooky Horoscope</h2>
  <label for="sign">Choose your sign:</label>
  <select id="sign">
    <option value="">--Select--</option>
    <option value="aries">♈ Aries</option>
    <option value="taurus">♉ Taurus</option>
    <option value="gemini">♊ Gemini</option>
    <option value="cancer">♋ Cancer</option>
    <option value="leo">♌ Leo</option>
    <option value="virgo">♍ Virgo</option>
    <option value="libra">♎ Libra</option>
    <option value="scorpio">♏ Scorpio</option>
    <option value="sagittarius">♐ Sagittarius</option>
    <option value="capricorn">♑ Capricorn</option>
    <option value="aquarius">♒ Aquarius</option>
    <option value="pisces">♓ Pisces</option>
  </select>
  <button onclick="getSpookyHoroscope()">Reveal My Fate</button>
  <p id="spookyResult" style="margin-top: 20px; color: violet; font-style: italic;"></p>
  </section>
  <section class="spotify">
    <h2>🔮 Some Creepy Vibes</h2>
    <p><em>🧪 This playlist was brewed under a blood moon with ghostly hands and glittering shadows. It’s not just music — it’s a spell. Press play and vanish. 💫👻 
    <iframe style="border-radius:12px" src="https://open.spotify.com/embed/playlist/1Pg4aIDGiFGKhgAfwDa3b3?utm_source=generator" width="100%" height="152" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
  
  <footer class="adios"><footer style="text-align:center; padding: 50px 20px; background: linear-gradient(90deg, #0b0019, #1e0033); color: violet; font-family: 'Creepster', cursive; font-size: 22px; letter-spacing: 2px; text-shadow: 2px 2px 6px purple;">
 <h2>🌙 Adios</h2>
    <p>Thank you for exploring my little spooky world! This was just a witchy beginning — more chaos, more spells, and more stories will brew soon. Stay weird, stay magical. ✨👾💀<br />
    Adios, fellow night crawlers!</p>
  </footer>  <script>
    function getWitchResult() {
      const val = document.querySelector('input[name="q1"]:checked');
      if (!val) return alert("Choose an answer!");
      const type = val.value;
      const types = {
  forest: "🌲 You're a Forest Witch! You draw power from nature and earth spirits.",
  storm: "🌩️ You're a Storm Witch! You thrive in chaos, change, and lightning strikes.",
  shadow: "🌑 You're a Shadow Witch! You're mysterious, deep, and see the unseen.",
  fire: "🔥 You're a Fire Witch! Passionate, fierce, and born to lead.",
  ice: "❄️ You're an Ice Witch! Calm, elegant, and unshakably in control.",
  sea: "🌊 You're a Sea Witch! Emotions, tides, and the unknown call to you.",
  bone: "🦴 You're a Bone Witch! Wise, ancient, connected to the spirit realm.",
  cosmic: "💫 You're a Cosmic Witch! You read stars and dream with galaxies."
};
      document.getElementById("witchResult").innerText = types[type];
    }

    function drawTarot() {
      const cards = ["The Moon", "The Tower", "The Lovers", "Death", "The Star"];
      const meanings = {
        "The Moon": "Confusion, illusion, dreams.",
        "The Tower": "Sudden change, upheaval.",
        "The Lovers": "Connection, choice, harmony.",
        "Death": "Endings, transformation, rebirth.",
        "The Star": "Hope, guidance, inspiration."
      };
      const pick = cards[Math.floor(Math.random() * cards.length)];
      document.getElementById("tarotResult").innerText = `${pick}: ${meanings[pick]}`;
    }

    function generateSpell() {
      const names = ["Binding Whispers", "Night Veil", "Crystal Echo", "Blood Pact"];
      const ingredients = ["raven feather", "moon water", "black salt", "phantom root"];
      const chants = ["Morva elthra senna!", "Zel nocht varun!", "Silven drak osh!"];
      const spell = names[Math.floor(Math.random() * names.length)];
      const ing = ingredients.sort(() => 0.5 - Math.random()).slice(0, 2).join(", ");
      const chant = chants[Math.floor(Math.random() * chants.length)];
      document.getElementById("spellResult").innerText = `${spell}\nIngredients: ${ing}\nIncantation: ${chant}`;
    }

    function makePotion() {
     const results = [
  "Potion of Eternal Confidence",
  "Love Elixir",
  "Invisibility Draught",
  "Truth Serum",
  "Witch's Brew of Misfortune",
  "Serpent's Tongue Serum",
  "Liquid Luck (Felix Felicis)",
  "Memory Mist",
  "Nightmare Nectar",
  "Dragon’s Breath Potion",
  "Potion of Shapeshifting",
  "Ghost Whisper Tonic",
  "Elixir of Time Freeze",
  "Poison of Eternal Sleep",
  "Soul Binding Vial",
  "Potion of Endless Night",
  "Spider Silk Serum",
  "Moonlight Elixir",
  "Goblin Gigglegoo",
  "Cauldron of Curses"
]; 
      document.getElementById("potionResult").innerText = `You brewed: ${results[Math.floor(Math.random() * results.length)]}`;
    }
  </script><script>
  function talkToSpirit() {
    const messages = [
      "You are not alone... the spirits walk with you.",
      "Your future is cloudy, but something stirs in the shadows.",
      "Beware the full moon... it brings more than light.",
      "A forgotten soul is watching. Are you ready to listen?",
      "Your power grows stronger, but so does the danger.",
      "You will soon meet someone... or something.",
      "The mirror sees all — even what you try to hide."
    ];
    const mirror = document.getElementById("mirrorMessage");
    const spirit = messages[Math.floor(Math.random() * messages.length)];
    mirror.innerText = `"${spirit}"`;
  }
</script>
<script>
  function triggerScare() {
    const scare = document.getElementById("scareContainer");
    const blood = document.getElementById("bloodFlash");
    scare.style.display = "flex";
    blood.style.display = "block";

    const scream = new Audio("https://www.myinstants.com/media/sounds/wilhelm-scream.mp3");
    scream.play();

    setTimeout(() => {
      scare.style.display = "none";
      blood.style.display = "none";
    }, 3000);
  }
</script>
<script>
  const horoscopes = {
    aries: [
      "Aries, your flame burns bright tonight... but beware who follows its light.",
      "Your courage may attract spirits. Burn sage at dusk.",
      "A shadow has its eye on you. Be bold, but not careless."
    ],
    taurus: [
      "Taurus, something old is clinging to your aura. Cleanse with earth and salt.",
      "Your stubbornness will summon ancient energy. Are you ready to deal with it?",
      "A creature walks where you once stood. It remembers you."
    ],
    gemini: [
      "Two faces, two paths. One leads to light, the other to screams.",
      "Speak less today. The spirits are listening.",
      "Your reflection may answer before you do. Avoid mirrors."
    ],
    cancer: [
      "The moon is whispering to you. Listen closely, but do not answer.",
      "Your feelings summon more than just memories tonight.",
      "Something watery wants to drag you under — emotionally or otherwise."
    ],
    leo: [
      "You’re glowing... which means dark things are watching.",
      "Pride may attract a challenge. A ghostly one.",
      "Don’t roar too loud. It may wake what sleeps below."
    ],
    virgo: [
      "You notice the patterns... but some were never meant to be seen.",
      "Dust your corners. Something’s hiding behind the perfection.",
      "Your logic won’t help when magic slips through the cracks."
    ],
    libra: [
      "Balance is breaking. Tip too far, and you’ll see the veil tear.",
      "You’ll be haunted by a choice. But which one?",
      "Mirror magic surrounds you — don’t stare too long."
    ],
    scorpio: [
      "Death isn’t the end for you today... it’s a beginning.",
      "A secret you’ve buried is clawing its way out.",
      "Your energy is magnetic — even to the dead."
    ],
    sagittarius: [
      "Wander far, but don’t follow the voices.",
      "You’ll find something lost. It may not want to be found.",
      "A new path opens. But it smells of ash and blood."
    ],
    capricorn: [
      "You're grounded — but something is trying to pull you down further.",
      "Be cautious with time. The past wants you back.",
      "Bones remember footsteps. Walk lighter today."
    ],
    aquarius: [
      "Your visions grow clearer, but they may not be your own.",
      "The air crackles. Something magical is reaching for you.",
      "Dreams will deliver a message tonight. Do not ignore it."
    ],
    pisces: [
      "You see beyond the veil — but something is staring back.",
      "Water remembers. Don’t let it carry away your truth.",
      "Tonight, your dreams become a door. Will you walk through?"
    ]
  };

  function getSpookyHoroscope() {
    const sign = document.getElementById("sign").value;
    const result = document.getElementById("spookyResult");

    if (!sign) {
      result.innerText = "Please choose your zodiac sign, child of the stars...";
      return;
    }

    const options = horoscopes[sign];
    const message = options[Math.floor(Math.random() * options.length)];
    result.innerText = message;
  }
</script>
<script>
  function submitEcho() {
    const story = document.getElementById("userStory").value.trim();
    const userEchos = document.getElementById("userEchos");

    if (story === "") {
      alert("The spirits demand a message...");
      return;
    }

    const entry = document.createElement("div");
    entry.className = "entry";
    entry.innerText = story;
    userEchos.appendChild(entry);

    document.getElementById("userStory").value = "";
  }
</script>
