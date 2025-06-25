<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Game Tebak Kata - Tebak Kata Lengkap dengan Gambar</title>
<style>
  /* CSS code goes here */
</style>
</head>
<body>
<h1>Game Tebak Kata - Tebak Kata Lengkap dengan Gambar</h1>

<div id="nameInputArea" aria-label="Masukkan nama pemain dan mulai game">
  <label for="playerNameInput">namain dulu ngab</label>
  <input type="text" id="playerNameInput" maxlength="20" autocomplete="off" aria-describedby="message" aria-label="Masukkan nama pemain" />
  <button id="startBtn" aria-label="Mulai permainan">Mulai</button>
</div>

<div id="categorySelection" role="group" aria-label="Pilih kategori" style="display:none;">
  <button class="categoryBtn" data-category="Negara">Negara</button>
  <button class="categoryBtn" data-category="Newan">Hewan</button>
  <button class="categoryBtn" data-category="Pengetahuan">Pengetahuan Umum</button>
</div>

<div id="gameContainer" role="main" aria-label="Game Tebak Kata" style="display:none;">
  <div id="playerInfo" aria-live="polite" aria-atomic="true"></div>
  <div id="scoreDisplay" aria-live="polite" aria-atomic="true"></div>
  <div id="selectedCategory" aria-live="polite" style="margin-bottom:12px; font-weight:bold; font-size:18px"></div>
  <div id="wordDisplay" aria-live="polite" aria-atomic="true" aria-label="Kata yang harus ditebak"></div>
  <div id="clueDisplay" aria-live="polite" aria-atomic="true" aria-label="Petunjuk kata"></div>
  <div id="message" role="alert" aria-live="assertive"></div>
  <div id="inputArea">
    <label for="wordInput" class="visually-hidden">Masukkan tebakan kata lengkap</label>
    <input type="text" id="wordInput" autocomplete="off" aria-describedby="message" aria-label="Input tebakan kata lengkap" disabled />
    <button id="guessBtn" aria-label="Tebak kata" disabled>Tebak</button>
    <button id="skipBtn" aria-label="Lewati kata" disabled>Lewati</button>
  </div>
  <div id="wrongLetters" aria-live="polite" aria-atomic="true"></div>
  <button id="restartBtn" aria-label="Mulai ulang permainan">Main Lagi</button>
  <img id="imageDisplay" alt="Gambar tebakan" />
</div>

<script>
  // JavaScript code goes here
</script>
</body>
</html>
