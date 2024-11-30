<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wedding Invitation</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
            background-color: #f9f1f0;
        }
        .container {
            padding: 20px;
        }
        .card {
            background: #fff;
            margin: 20px auto;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            max-width: 500px;
        }
        h1 {
            color: #d87d7d;
        }
        p {
            font-size: 18px;
            color: #555;
        }
        .footer {
            margin-top: 20px;
            font-size: 14px;
            color: #aaa;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="card">
            <h1>Thiệp Cưới</h1>
            <p>Chào <span id="to"></span>,</p>
            <p>Chúng tôi hân hạnh mời bạn đến dự lễ cưới của <span id="me"></span>.</p>
            <p>Thời gian: 16h30, ngày 12/10/2024</p>
            <p>Địa điểm: Nhà trai - Thôn Như Phượng Thượng, xã Long Hưng, Văn Giang, Hưng Yên.</p>
        </div>
        <div class="footer">
            <p>&copy; 2024 by Đức Thắng & Huyền Trang</p>
        </div>
    </div>

    <script>
        const urlParams = new URLSearchParams(window.location.search);
        const to = urlParams.get('to') || 'bạn';
        const me = urlParams.get('me') || 'chúng tôi';

        document.getElementById('to').textContent = decodeURIComponent(to.replace(/\+/g, ' '));
        document.getElementById('me').textContent = decodeURIComponent(me.replace(/\+/g, ' '));
    </script>
</body>
</html>