<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Happy New Year 2026</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

body {
    height: 100vh;
    background: radial-gradient(circle at bottom, #0a0a23, #000);
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: hidden;
    color: white;
}

/* Text */
.container {
    text-align: center;
    z-index: 5;
}

h1 {
    font-size: 4rem;
    animation: glow 2s infinite alternate;
}

h2 {
    font-size: 3rem;
    color: gold;
    animation: bounce 2s infinite;
}

/* Firework container */
.firework {
    position: absolute;
    width: 6px;
    height: 6px;
    background: transparent;
}

/* Firework burst */
.firework::before {
    content: '';
    position: absolute;
    width: 6px;
    height: 6px;
    background: gold;
    border-radius: 50%;
    animation: boom 2.5s infinite;
    box-shadow:
        0 -40px gold,
        0 40px gold,
        40px 0 gold,
        -40px 0 gold,
        28px 28px gold,
        -28px -28px gold,
        -28px 28px gold,
        28px -28px gold;
}

/* Positions */
.fw1 { top: 30%; left: 25%; animation-delay: 0s; }
.fw2 { top: 40%; left: 60%; animation-delay: 1s; }
.fw3 { top: 25%; left: 45%; animation-delay: 2s; }

/* Animations */
@keyframes boom {
    0% {
        transform: scale(0);
        opacity: 1;
    }
    50% {
        transform: scale(1.2);
        opacity: 1;
    }
    100% {
        transform: scale(0);
        opacity: 0;
    }
}

@keyframes glow {
    from {
        text-shadow: 0 0 10px gold;
    }
    to {
        text-shadow: 0 0 30px orange, 0 0 60px gold;
    }
}

@keyframes bounce {
    0%, 100% {
        transform: translateY(0);
    }
    50% {
        transform: translateY(-12px);
    }
}
</style>
</head>

<body>

<div class="container">
    <h1>🎉 Happy New Year 🎉</h1>
    <h2>2026</h2>
</div>

<div class="firework fw1"></div>
<div class="firework fw2"></div>
<div class="firework fw3"></div>

</body>
</html>
