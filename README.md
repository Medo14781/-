<!DOCTYPE html><html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ادفع الآن - Pay Now</title>
    <style>
        body {
            background: #f8f8f8;
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 50px;
        }
        .card {
            background: white;
            padding: 20px;
            margin: auto;
            width: 90%;
            max-width: 400px;
            box-shadow: 0 0 15px rgba(0,0,0,0.1);
            border-radius: 12px;
        }
        h1 {
            color: #333;
        }
        .pay-info {
            margin: 20px 0;
            font-size: 18px;
            background: #eee;
            padding: 10px;
            border-radius: 8px;
        }
        button {
            background: #007bff;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 8px;
            cursor: pointer;
            margin: 10px 0;
        }
        button:hover {
            background: #0056b3;
        }
        .qr-code {
            margin-top: 20px;
        }
        img {
            width: 150px;
            border-radius: 8px;
        }
    </style>
</head>
<body>
    <div class="card">
        <h1>ادفع الآن</h1>
        <p>يرجى تحويل المبلغ على:</p><div class="pay-info">
        فودافون كاش: <strong>01012345678</strong>
    </div>
    <button onclick="copyToClipboard('01012345678')">نسخ رقم فودافون كاش</button>

    <div class="pay-info">
        Instapay: <strong>name@instapay</strong>
    </div>
    <button onclick="copyToClipboard('name@instapay')">نسخ Instapay</button>

    <div class="qr-code">
        <p>امسح QR للدفع:</p>
        <img src="YOUR_QR_CODE_IMAGE_URL" alt="QR Code">
    </div>

    <p style="margin-top:20px; color:gray;">شكراً لدعمك! تأكد من تحويل المبلغ الصحيح.</p>
</div>

<script>
    function copyToClipboard(text) {
        navigator.clipboard.writeText(text);
        alert("تم نسخ: " + text);
    }
</script>

</body>
</html># -
