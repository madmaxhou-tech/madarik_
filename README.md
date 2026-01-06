<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <title>مدارك | التفسير الجذري الدلالي</title>
  <style>
    body {
      font-family: "Amiri", serif;
      background: #f7f7f7;
      margin: 0;
      padding: 0;
      line-height: 1.9;
    }
    header {
      background: #1f2937;
      color: #fff;
      padding: 20px;
      text-align: center;
    }
    header h1 { margin: 0; }
    .search-box {
      margin: 20px auto;
      max-width: 500px;
      display: flex;
    }
    .search-box input {
      flex: 1;
      padding: 10px;
      font-size: 16px;
    }
    .container {
      max-width: 900px;
      margin: auto;
      padding: 20px;
      background: #fff;
    }
    .card {
      border-bottom: 1px solid #ddd;
      padding: 15px 0;
    }
    .term { font-weight: bold; font-size: 18px; }
    .root { color: #555; }
    footer {
      text-align: center;
      padding: 15px;
      font-size: 14px;
      color: #666;
    }
  </style>
</head>
<body>

<header>
  <h1>مدارك</h1>
  <p>التفسير الجذري الدلالي للقرآن الكريم<br>على منهج مقاييس اللغة لابن فارس</p>
</header>

<div class="search-box">
  <input type="text" id="search" placeholder="ابحث عن لفظ أو جذر…" onkeyup="searchTerms()" />
</div>

<div class="container" id="results">
  <div class="card">
    <div class="term">الحمد</div>
    <div class="root">الجذر: ح م د</div>
    <div>المقياس: الثناء المقترن بالرضا</div>
    <div>التوجيه: إقرار اختياري بكمال المنعِم</div>
  </div>
  <div class="card">
    <div class="term">اهدنا</div>
    <div class="root">الجذر: ه د ي</div>
    <div>المقياس: الإيصال بلطف</div>
    <div>التوجيه: نقل عملي في السلوك لا مجرد دلالة</div>
  </div>
</div>

<footer>
  مشروع مدارك © تفسير لغوي جذري
</footer>

<script>
function searchTerms() {
  let input = document.getElementById('search').value.toLowerCase();
  let cards = document.getElementsByClassName('card');
  for (let i = 0; i < cards.length; i++) {
    let text = cards[i].innerText.toLowerCase();
    cards[i].style.display = text.includes(input) ? "block" : "none";
  }
}
</script>

</body>
</html>
