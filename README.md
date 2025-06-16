

<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Забота+ | Заказы</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 20px;
      background-color: #f3f4f6;
      color: #111827;
    }
    h1 {
      text-align: center;
      color: #2563eb;
    }
    .order {
      background-color: #fff;
      border-radius: 12px;
      padding: 16px;
      margin-bottom: 16px;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    }
    .order h3 {
      margin: 0 0 8px;
    }
    .order p {
      margin: 4px 0;
    }
    .order a {
      display: inline-block;
      margin-top: 12px;
      padding: 10px 16px;
      background-color: #10b981;
      color: white;
      text-decoration: none;
      border-radius: 8px;
    }
  </style>
</head>
<body>
  <h1>Доступные заказы</h1>

  <div class="order">
    <h3>Заказ №1</h3>
    <p><strong>Что:</strong> Продукты</p>
    <p><strong>Откуда:</strong> Магазин «Арай», ул. Мира 12</p>
    <p><strong>Куда:</strong> ул. Жамбыла 45</p>
    <p><strong>Время:</strong> Сегодня в 17:00</p>
    <a id="link1" href="#">Взять заказ</a>
  </div>

  <div class="order">
    <h3>Заказ №2</h3>
    <p><strong>Что:</strong> Лекарства</p>
    <p><strong>Откуда:</strong> Аптека 24, ул. Ленина 5</p>
    <p><strong>Куда:</strong> ул. Абая 21, кв. 10</p>
    <p><strong>Время:</strong> Сегодня в 18:30</p>
    <a id="link2" href="#">Взять заказ</a>
  </div>

  <div class="order">
    <h3>Заказ №3</h3>
    <p><strong>Что:</strong> Документы</p>
    <p><strong>Откуда:</strong> Акимат, ул. Центральная 1</p>
    <p><strong>Куда:</strong> ул. Байтурсынова 8</p>
    <p><strong>Время:</strong> Завтра в 09:00</p>
    <a id="link3" href="#">Взять заказ</a>
  </div>

  <script>
    const urlParams = new URLSearchParams(window.location.search);
    const name = urlParams.get('name') || 'Без имени';
    const number = '+77718748634'; // WhatsApp номер диспетчера

    document.getElementById('link1').href = `https://wa.me/${number}?text=Здравствуйте,%20это%20${name}.%20Беру%20заказ%20№1:%20Продукты,%20ул.%20Мира%2012%20→%20ул.%20Жамбыла%2045,%20сегодня%2017:00`;
    document.getElementById('link2').href = `https://wa.me/${number}?text=Здравствуйте,%20это%20${name}.%20Беру%20заказ%20№2:%20Лекарства,%20ул.%20Ленина%205%20→%20ул.%20Абая%2021,%20сегодня%2018:30`;
    document.getElementById('link3').href = `https://wa.me/${number}?text=Здравствуйте,%20это%20${name}.%20Беру%20заказ%20№3:%20Документы,%20ул.%20Центральная%201%20→%20ул.%20Байтурсынова%208,%20завтра%2009:00`;
  </script>
</body>
</html>

