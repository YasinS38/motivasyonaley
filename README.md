<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Senin İçin</title>
  <style>
    body {
      font-family: 'Georgia', serif;
      background: #fff8f0;
      color: #4b3e2b;
      margin: 0;
      padding: 0;
    }

    header {
      background-color: #ffd6d6;
      padding: 2rem;
      text-align: center;
    }

    header h1 {
      font-size: 2.5rem;
      margin: 0;
    }

    section {
      max-width: 800px;
      margin: auto;
      padding: 2rem;
      line-height: 1.8;
    }

    .mektup {
      background-color: #fff0f5;
      border-left: 5px solid #f7a1c4;
      padding: 1.5rem;
      margin-top: 2rem;
      border-radius: 8px;
    }

    .sayac {
      text-align: center;
      margin-top: 3rem;
      font-size: 1.2rem;
      background: #ffe4e1;
      padding: 1rem;
      border-radius: 10px;
    }

    .gallery {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 15px;
      margin-top: 3rem;
    }

    .gallery img {
      width: 200px;
      height: auto;
      border-radius: 10px;
      box-shadow: 0 4px 6px rgba(0,0,0,0.1);
      transition: transform 0.3s ease;
    }

    .gallery img:hover {
      transform: scale(1.05);
    }

    h2 {
      text-align: center;
      margin-top: 3rem;
    }
  </style>
</head>
<body>

<header>
  <h1>Senin İçin, Sadece Senin İçin</h1>
</header>

<section>
  <p>
    Biliyorum... Son zamanlarda her şey üst üste geldi. İçinde fırtınalar koparken, dışarıdan güçlü görünmeye çalışıyorsun.
    Bu yük bazen fazla geliyor. Sınavlar, regl döneminin verdiği gerginlik, hayattaki baskılar… Hepsi bir anda yükleniyor omuzlarına. 
    Ama bir bilsen, seni ne kadar güçlü ve hayranlık uyandırıcı buluyorum…
  </p>

  <p>
    Senin iç dünyan çok değerli. Ne kadar yorulsan da, ne kadar karışık hissetsen de, bu seni eksik yapmaz. 
    Aksine, bu seni insan yapar. Seni sen yapan her şey, iyi ve kötü anlar dâhil olmak üzere, seni sevmeme neden.
  </p>

  <div class="mektup">
    <h2>📝 Sana Birkaç Satır</h2>
    <p>
      Sevgilim, seni ilk gördüğüm an ne kadar güzelsen, zamanla tanıdıkça bir o kadar güzel olduğunu fark ettim. 
      Gücünü, duygularını, kararlılığını… Hepsine hayran kaldım. Zor günler geçiriyorsun, ama inan bana bu sadece geçici. 
      Bu fırtına dinecek ve güneş seni yine en güzel haliyle aydınlatacak. 
      Sen bu sınavdan, bu yorgunluktan, bu stresli dönemden dimdik çıkacaksın. 
      Çünkü senin içinde, çoğu insanın içinde olmayan özel bir güç var.
    </p>
    <p>
      Yanındayım. Her zaman. Ağlamak istersen omzum burada, susmak istersen sessizliğim seninle. 
      Gülmek istersen, beraber kahkahalar atalım. Yorgunsan, birlikte dinlenelim. 
      Ama hiçbir zaman yalnız olmadığını unutma.
    </p>
    <p>
      Bu site belki küçük bir şey. Ama kalbimin büyük bir parçası burada. Her kelime, senin içini biraz olsun ısıtsın diye yazıldı. 
      Seni seviyorum… Her halinle.
    </p>
  </div>

  <div class="sayac">
    <h3>📚 Sınavına Kalan Gün:</h3>
    <p id="examCountdown"></p>
  </div>

  <h2>📸 Anılarımız</h2>
  <div class="gallery">
    <img src="foto1.jpg" alt="Anı 1">
    <img src="foto2.jpg" alt="Anı 2">
    <img src="foto3.jpg" alt="Anı 3">
  </div>
</section>

<script>
  // Güncel sınav tarihi: 2025-06-20
  const examDate = new Date("2025-06-20");
  const today = new Date();
  const diffTime = examDate - today;
  const diffDays = Math.ceil(diffTime / (1000 * 60 * 60 * 24));
  document.getElementById("examCountdown").textContent = 
    diffDays > 0 
    ? `${diffDays} gün kaldı. Ama sen hazırsın 💪` 
    : "Sınav günün geldi! Başarılar ❤️";
</script>

</body>
</html>
