<!DOCTYPE html>
<html lang="cs">
<head>
    <meta charset="UTF-8">
    <title>Heslo Kontrola</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background: #f0f2f5;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
        }
        .container {
            background: white;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 0 15px rgba(0,0,0,0.2);
            text-align: center;
            width: 300px;
        }
        input[type="password"] {
            width: 100%;
            padding: 10px;
            font-size: 16px;
            margin-bottom: 20px;
            border-radius: 8px;
            border: 1px solid #ccc;
        }
        .strength-bar {
            position: relative;
            width: 100%;
            height: 10px;
            background: linear-gradient(to right, red 33%, yellow 66%, green 100%);
            border-radius: 5px;
            margin-bottom: 30px;
            overflow: hidden;
        }
        .arrow {
            position: absolute;
            top: -15px;
            width: 0;
            height: 0;
            border-left: 7px solid transparent;
            border-right: 7px solid transparent;
            border-bottom: 15px solid black;
            transition: left 0.3s;
        }
        #confirm-btn {
            padding: 10px 20px;
            font-size: 16px;
            border: none;
            background: #4CAF50;
            color: white;
            border-radius: 8px;
            cursor: pointer;
            transition: 0.3s ease;
            position: relative;
        }
    </style>
</head>
<body>

<div class="container">
    <h2>Zadej heslo</h2>
    <input type="password" id="password" placeholder="Enter your password...">
    <div class="strength-bar">
        <div class="arrow" id="arrow"></div>
    </div>
    <button id="confirm-btn">Potvrdit</button>
</div>

<script>
const passwordInput = document.getElementById('password');
const arrow = document.getElementById('arrow');
const button = document.getElementById('confirm-btn');
const container = document.querySelector('.container');

function calculateStrength(password) {
    let strength = 0;
    if (password.length > 4) strength += 20;
    if (password.length > 8) strength += 30;
    if (/[A-Z]/.test(password)) strength += 20;
    if (/[0-9]/.test(password)) strength += 20;
    if (/[^A-Za-z0-9]/.test(password)) strength += 10;
    return Math.min(strength, 100);
}

passwordInput.addEventListener('input', () => {
    const password = passwordInput.value;
    const strength = calculateStrength(password);
    arrow.style.left = calc(${strength}% - 7px);
});

let isRunningAway = false;

container.addEventListener('mousemove', (e) => {
    const password = passwordInput.value;
    const strength = calculateStrength(password);
    if (strength < 60) {
        const rect = button.getBoundingClientRect();
        const mouseX = e.clientX;
        const mouseY = e.clientY;
        const btnCenterX = rect.left + rect.width / 2;
        const btnCenterY = rect.top + rect.height / 2;
        const dx = mouseX - btnCenterX;
        const dy = mouseY - btnCenterY;
        const dist = Math.sqrt(dx*dx + dy*dy);

        if (dist < 100) {
            const moveX = -(dx) / 10;
            const moveY = -(dy) / 10;
            button.style.transform = translate(${moveX}px, ${moveY}px);
            isRunningAway = true;
        } else if (isRunningAway) {
            button.style.transform = translate(0,0);
            isRunningAway = false;
        }
    } else {
        button.style.transform = translate(0,0);
    }
});
</script>

</body>
</html>
