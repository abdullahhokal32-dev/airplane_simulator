# airplane_simulator
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document.body.style.backgroundColor<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<title>تحليل الجولات</title>
<link rel="stylesheet" href="css/style.css">
</head>
<body>
<div class="container">
<h1>تحليل الجولات</h1>
<label>ادخل نتائج الجولات (رقم واحد لكل جولة)</label>
<input type="text" id="roundsInput" placeholder="مثال: 2,5,3">
<button id="analyzeBtn">تحليل</button>
<div id="results"></div>
</div>
<script src="js/analyzer.js"></script>
</body>
</html><!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<title>الإعدادات</title>
<link rel="stylesheet" href="css/style.css">
</head>
<body>
<div class="container">
<h1>الإعدادات</h1>
<label>تغيير لون الواجهة</label>
<input type="color" id="themeColor">
<label>سرعة المحاكاة</label>
<input type="range" id="speedRange" min="1" max="10" value="5">
<label>تشغيل/إيقاف الصوت</label>
<input type="checkbox" id="soundToggle" checked>
</div>
<script>
const theme = document.getElementById("themeColor");
theme.addEventListener("input", () => {
  document.body.style.backgroundColor = theme.value;
});
</script>
</body>
</html><!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<title>تسجيل الدخول</title>
<link rel="stylesheet" href="css/style.css">
</head>
<body>
<div class="container">
  <h1>تسجيل الدخول</h1>
  <form id="loginForm">
    <label>المعرف</label>
    <input type="text" id="userId" required>
    <label>كلمة المرور</label>
    <input type="password" id="password" required>
    <button type="submit">دخول</button>
    <p id="errorMsg"></p>
  </form>
</div>
<script>
document.getElementById("loginForm").addEventListener("submit", function(e){
  e.preventDefault();
  const pw = document.getElementById("password").value;
  if(pw === "hoklagmaing"){
    window.location.href = "dashboard.html";
  } else {
    document.getElementById("errorMsg").innerText = "كلمة المرور خاطئة";
  }
});
</script>
</body>
</html><!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<title>لوحة التحكم</title>
<link rel="stylesheet" href="css/style.css">
</head>
<body>
<div class="container">
  <h1>محاكاة الطائرة</h1>
  <button id="startSim">بدء المحاكاة</button>
  <canvas id="simCanvas" width="400" height="200"></canvas>
</div>
<script src="js/app.js"></script>
</body>
</html><!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<title>الإعدادات</title>
<link rel="stylesheet" href="css/style.css">
</head>
<body>
<div class="container">
<h1>الإعدادات</h1>
<label>تغيير لون الواجهة</label>
<input type="color" id="themeColor">
<label>سرعة المحاكاة</label>
<input type="range" id="speedRange" min="1" max="10" value="5">
<label>تشغيل/إيقاف الصوت</label>
<input type="checkbox" id="soundToggle" checked>
</div>
<script>
const theme = document.getElementById("themeColor");
theme.addEventListener("input", () => {
  document.body.style.backgroundColor = theme.value;
});
</script>
</body>
</html><!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<title>تحليل الجولات</title>
<link rel="stylesheet" href="css/style.css">
</head>
<body>
<div class="container">
<h1>تحليل 
  الجولات</h1>
<label>ادخل نتائج الجولات (رقم واحد لكل جولة)</label>
<input type="text" id="roundsInput" placeholder="مثال: 2,5,3">
<button id="analyzeBtn">تحليل</button>
<div id="results"></div>
</div>
<script src="js/analyzer.js"></script>
</body>
</html>
