<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>مركز فجر الإسلام للموبايل</title>
  <link href="https://fonts.googleapis.com/css2?family=Cairo&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Cairo', sans-serif;
      margin: 0;
      background-color: #f2f2f2;
    }
    header {
      background-color: #007acc;
      color: white;
      padding: 20px;
      text-align: center;
      font-size: 24px;
      font-weight: bold;
    }
    .logo {
      font-size: 28px;
      margin-bottom: 10px;
      font-weight: bold;
      color: #fff;
    }
    .banner {
      width: 100%;
      max-height: 250px;
      object-fit: cover;
    }
    .content {
      max-width: 800px;
      margin: auto;
      padding: 20px;
      background: white;
      border-radius: 12px;
      margin-top: -30px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }
    h2 {
      color: #007acc;
    }
    ul {
      text-align: right;
      padding-right: 20px;
    }
    .whatsapp-btn {
      display: inline-block;
      margin-top: 20px;
      background-color: #25d366;
      color: white;
      padding: 12px 20px;
      border-radius: 8px;
      text-decoration: none;
      font-size: 18px;
    }
    form {
      text-align: right;
      margin-top: 20px;
    }
    input, textarea {
      width: 100%;
      padding: 10px;
      margin-top: 10px;
      border: 1px solid #ccc;
      border-radius: 6px;
      font-family: 'Cairo', sans-serif;
    }
    .submit-btn {
      background-color: #007acc;
      color: white;
      border: none;
      padding: 10px 20px;
      border-radius: 8px;
      margin-top: 10px;
      font-size: 16px;
      cursor: pointer;
    }
    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
      gap: 10px;
      margin-top: 20px;
    }
    .gallery img {
      width: 100%;
      border-radius: 10px;
      height: 120px;
      object-fit: cover;
    }
    footer {
      margin-top: 30px;
      text-align: center;
      font-size: 14px;
      color: gray;
    }
  </style>
</head>
<body>

  <header>
    <div class="logo">مركز فجر الإسلام للموبايل</div>
  </header>

  <!-- بانر -->
  <img src="https://images.unsplash.com/photo-1510557880182-3c5aee37a6d6?auto=format&fit=crop&w=800&q=80" class="banner" alt="Mobile Repair">

  <div class="content">
    <h2>خدماتنا</h2>
    <ul>
      <li>تغيير شاشات وبطاريات</li>
      <li>صيانة أعطال السوفت وير</li>
      <li>استرجاع بيانات</li>
      <li>بيع قطع غيار أصلية</li>
    </ul>

    <h2>مواعيد العمل</h2>
    <p>يومياً من 11 ظهراً إلى 12 منتصف الليل</p>

    <h2>تواصل معنا</h2>
    <p>📞 01100070768</p>
    <a class="whatsapp-btn" href="https://wa.me/201100070768" target="_blank">راسلنا على واتساب</a>

    <h2>احجز صيانة الآن</h2>
    <form onsubmit="sendWhatsApp(); return false;">
      <input type="text" id="name" placeholder="الاسم" required>
      <input type="tel" id="phone" placeholder="رقم الهاتف" required>
      <textarea id="problem" placeholder="ما هي مشكلتك؟" rows="4" required></textarea>
      <button type="submit" class="submit-btn">إرسال</button>
    </form>

    <h2>صور من خدماتنا</h2>
    <div class="gallery">
      <img src="https://images.unsplash.com/photo-1581090700227-1e37b190418e?auto=format&fit=crop&w=400&q=80" alt="خدمة">
      <img src="https://images.unsplash.com/photo-1603791440384-56cd371ee9a7?auto=format&fit=crop&w=400&q=80" alt="صيانة">
      <img src="https://images.unsplash.com/photo-1580910051073-eebd5ae5e43f?auto=format&fit=crop&w=400&q=80" alt="موبايل">
    </div>

  </div>

  <footer>
    &copy; 2025 مركز فجر الإسلام للموبايل
  </footer>

  <script>
    function sendWhatsApp() {
      const name = document.getElementById('name').value;
      const phone = document.getElementById('phone').value;
      const problem = document.getElementById('problem').value;
      const msg = `الاسم: ${name}%0Aرقم الهاتف: ${phone}%0Aالمشكلة: ${problem}`;
      window.open(`https://wa.me/201100070768?text=${msg}`, '_blank');
    }
  </script>

</body>
</html>
