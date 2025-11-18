<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Kuis Pengetahuan Umum</title>

<style>
    body {
        font-family: "Poppins", sans-serif;
        background: linear-gradient(135deg, #ffecd2, #fcb69f);
        margin: 0;
        padding: 0;
        color: #333;
    }

    header {
        text-align: center;
        padding: 20px;
        background: rgba(255, 255, 255, 0.3);
        backdrop-filter: blur(8px);
        border-bottom: 3px solid rgba(255, 255, 255, 0.5);
    }

    .container {
        max-width: 800px;
        margin: 40px auto;
        background: white;
        border-radius: 15px;
        padding: 30px;
        box-shadow: 0 5px 18px rgba(0, 0, 0, 0.2);
        position: relative;
        overflow: hidden;
    }

    /* Ornamen */
    .ornamen1, .ornamen2 {
        position: absolute;
        width: 120px;
        height: 120px;
        background: rgba(255, 174, 0, 0.25);
        border-radius: 50%;
        z-index: 0;
    }

    .ornamen1 {
        top: -40px;
        right: -40px;
    }

    .ornamen2 {
        bottom: -40px;
        left: -40px;
    }

    h2 {
        z-index: 2;
        position: relative;
    }

    .question {
        margin-bottom: 20px;
        font-weight: 600;
    }

    .options label {
        display: block;
        padding: 10px;
        margin: 5px 0;
        background: #ffe8cc;
        border-radius: 10px;
        cursor: pointer;
        transition: 0.2s;
        z-index: 2;
        position: relative;
    }

    .options label:hover {
        background: #ffce99;
    }

    button {
        background: #ff9900;
        color: white;
        padding: 12px 20px;
        border: none;
        font-size: 16px;
        cursor: pointer;
        border-radius: 10px;
        margin-top: 20px;
        transition: 0.2s;
    }

    button:hover {
        background: #e68a00;
    }

    #result {
        margin-top: 25px;
        padding: 20px;
        background: #fff3cd;
        border-radius: 10px;
        font-weight: 600;
        display: none;
    }
</style>
</head>

<body>

<header>
    <h1>Kuis Pengetahuan Umum</h1>
    <p>Jawab 10 soal dengan pilihan ganda A–E</p>
</header>

<div class="container">
    <div class="ornamen1"></div>
    <div class="ornamen2"></div>

    <form id="quizForm">

        <!-- Soal 1 -->
        <div class="question">1. Negara mana yang pertama kali mencapai permukaan bulan?</div>
        <div class="options">
            <label><input type="radio" name="q1" value="A"> A. Rusia</label>
            <label><input type="radio" name="q1" value="B"> B. Amerika Serikat ✔</label>
            <label><input type="radio" name="q1" value="C"> C. China</label>
            <label><input type="radio" name="q1" value="D"> D. Jepang</label>
            <label><input type="radio" name="q1" value="E"> E. India</label>
        </div>

        <!-- Soal 2 -->
        <div class="question">2. Siapakah penulis karya “The Origin of Species”?</div>
        <div class="options">
            <label><input type="radio" name="q2" value="A"> A. Albert Einstein</label>
            <label><input type="radio" name="q2" value="B"> B. Isaac Newton</label>
            <label><input type="radio" name="q2" value="C"> C. Charles Darwin ✔</label>
            <label><input type="radio" name="q2" value="D"> D. Nikola Tesla</label>
            <label><input type="radio" name="q2" value="E"> E. Galileo Galilei</label>
        </div>

        <!-- Soal 3 -->
        <div class="question">3. Unsur kimia dengan nomor atom 79 adalah?</div>
        <div class="options">
            <label><input type="radio" name="q3" value="A"> A. Platinum</label>
            <label><input type="radio" name="q3" value="B"> B. Perak</label>
            <label><input type="radio" name="q3" value="C"> C. Tembaga</label>
            <label><input type="radio" name="q3" value="D"> D. Emas ✔</label>
            <label><input type="radio" name="q3" value="E"> E. Uranium</label>
        </div>

        <!-- Soal 4 -->
        <div class="question">4. Sungai terpanjang di dunia saat ini adalah?</div>
        <div class="options">
            <label><input type="radio" name="q4" value="A"> A. Mississippi</label>
            <label><input type="radio" name="q4" value="B"> B. Nil ✔</label>
            <label><input type="radio" name="q4" value="C"> C. Amazon</label>
            <label><input type="radio" name="q4" value="D"> D. Yangtze</label>
            <label><input type="radio" name="q4" value="E"> E. Danube</label>
        </div>

        <!-- Soal 5 -->
        <div class="question">5. Tahun berapakah Perang Dunia II berakhir?</div>
        <div class="options">
            <label><input type="radio" name="q5" value="A"> A. 1939</label>
            <label><input type="radio" name="q5" value="B"> B. 1942</label>
            <label><input type="radio" name="q5" value="C"> C. 1945 ✔</label>
            <label><input type="radio" name="q5" value="D"> D. 1948</label>
            <label><input type="radio" name="q5" value="E"> E. 1950</label>
        </div>

        <!-- Soal 6 -->
        <div class="question">6. Siapakah pelukis terkenal dari karya “Starry Night”?</div>
        <div class="options">
            <label><input type="radio" name="q6" value="A"> A. Michelangelo</label>
            <label><input type="radio" name="q6" value="B"> B. Pablo Picasso</label>
            <label><input type="radio" name="q6" value="C"> C. Vincent van Gogh ✔</label>
            <label><input type="radio" name="q6" value="D"> D. Leonardo da Vinci</label>
            <label><input type="radio" name="q6" value="E"> E. Rembrandt</label>
        </div>

        <!-- Soal 7 -->
        <div class="question">7. Teori relativitas dikembangkan oleh siapa?</div>
        <div class="options">
            <label><input type="radio" name="q7" value="A"> A. Marie Curie</label>
            <label><input type="radio" name="q7" value="B"> B. Albert Einstein ✔</label>
            <label><input type="radio" name="q7" value="C"> C. Enrico Fermi</label>
            <label><input type="radio" name="q7" value="D"> D. Stephen Hawking</label>
            <label><input type="radio" name="q7" value="E"> E. James Clerk Maxwell</label>
        </div>

        <!-- Soal 8 -->
        <div class="question">8. Negara dengan populasi terbesar kedua di dunia adalah?</div>
        <div class="options">
            <label><input type="radio" name="q8" value="A"> A. India ✔</label>
            <label><input type="radio" name="q8" value="B"> B. Brazil</label>
            <label><input type="radio" name="q8" value="C"> C. Rusia</label>
            <label><input type="radio" name="q8" value="D"> D. Indonesia</label>
            <label><input type="radio" name="q8" value="E"> E. Pakistan</label>
        </div>

        <!-- Soal 9 -->
        <div class="question">9. Apa nama galaksi tempat Bima Sakti berada?</div>
        <div class="options">
            <label><input type="radio" name="q9" value="A"> A. Triangulum</label>
            <label><input type="radio" name="q9" value="B"> B. Andromeda</label>
            <label><input type="radio" name="q9" value="C"> C. Messier 87</label>
            <label><input type="radio" name="q9" value="D"> D. Virgo A</label>
            <label><input type="radio" name="q9" value="E"> E. Supercluster Laniakea ✔</label>
        </div>

        <!-- Soal 10 -->
        <div class="question">10. Apa nama partikel penyusun neutron dan proton?</div>
        <div class="options">
            <label><input type="radio" name="q10" value="A"> A. Quark ✔</label>
            <label><input type="radio" name="q10" value="B"> B. Ion</label>
            <label><input type="radio" name="q10" value="C"> C. Positron</label>
            <label><input type="radio" name="q10" value="D"> D. Neutrino</label>
            <label><input type="radio" name="q10" value="E"> E. Gluon</label>
        </div>

        <button type="button" onclick="checkAnswers()">Kumpulkan Jawaban</button>

    </form>

    <div id="result"></div>
</div>

<script>
function checkAnswers() {
    const correct = {
        q1: "B",
        q2: "C",
        q3: "D",
        q4: "B",
        q5: "C",
        q6: "C",
        q7: "B",
        q8: "A",
        q9: "E",
        q10: "A"
    };

    let score = 0;

    for (let key in correct) {
        let answer = document.querySelector(`input[name="${key}"]:checked`);
        if (answer && answer.value === correct[key]) {
            score++;
        }
    }

    const resultBox = document.getElementById("result");
    resultBox.style.display = "block";
    resultBox.innerHTML = `Skor kamu: <strong>${score}/10</strong>`;
}
</script>

</body>
</html>
