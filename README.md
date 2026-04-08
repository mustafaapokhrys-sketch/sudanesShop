<!DOCTYPE html>
<html lang="ar">
<head>
<meta charset="UTF-8">
<title>موقع مصطفى</title>
<style>
    body {
        margin: 0;
        padding: 0;
        font-family: "Cairo", sans-serif;
        background: linear-gradient(135deg, #0d47a1, #1976d2);
        color: white;
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
        text-align: center;
    }

    .container {
        max-width: 600px;
        padding: 20px;
        background: rgba(255, 255, 255, 0.1);
        border-radius: 20px;
        backdrop-filter: blur(10px);
        box-shadow: 0 0 20px rgba(0,0,0,0.3);
    }

    h1 {
        font-size: 40px;
        margin-bottom: 10px;
    }

    p {
        font-size: 20px;
        opacity: 0.9;
    }

    .loader {
        margin: 30px auto 0;
        width: 60px;
        height: 60px;
        border: 6px solid rgba(255,255,255,0.3);
        border-top-color: white;
        border-radius: 50%;
        animation: spin 1s linear infinite;
    }

    @keyframes spin {
        to { transform: rotate(360deg); }
    }
</style>
</head>
<body>

<div class="container">
    <h1>موقع مصطفى</h1>
    <p>الموقع قيد العمل حالياً… ترقبوا الإطلاق قريباً</p>
    <div class="loader"></div>
</div>

</body>
</html>
