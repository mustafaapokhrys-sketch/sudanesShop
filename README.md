<!DOCTYPE html>
<html lang="ar">
<head>
<meta charset="UTF-8">
<title>دردشة بسيطة</title>
<style>
    body { font-family: Arial; background:#f2f2f2; }
    #chat-box {
        width: 90%; height: 400px; margin: 20px auto;
        background: white; padding: 10px; overflow-y: auto;
        border-radius: 10px; border: 1px solid #ccc;
    }
    #input-area {
        width: 90%; margin: auto; display: flex; gap: 10px;
    }
    input {
        flex: 1; padding: 10px; border-radius: 8px; border: 1px solid #aaa;
    }
    button {
        padding: 10px 20px; border: none; background: #007bff;
        color: white; border-radius: 8px; cursor: pointer;
    }
</style>
</head>
<body>

<div id="chat-box"></div>

<div id="input-area">
    <input id="msg" placeholder="اكتب رسالتك...">
    <button onclick="sendMsg()">إرسال</button>
</div>

<script>
function sendMsg() {
    let box = document.getElementById("chat-box");
    let msg = document.getElementById("msg").value;

    if (msg.trim() === "") return;

    let p = document.createElement("p");
    p.textContent = "أنت: " + msg;
    box.appendChild(p);

    document.getElementById("msg").value = "";
    box.scrollTop = box.scrollHeight;
}
</script>

</body>
</html>
