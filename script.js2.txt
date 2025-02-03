function showMessage() {
    document.getElementById("message-title").style.display = "block";
    document.getElementById("message-content").style.display = "block";
    document.getElementById("fireworks").style.display = "block";
    document.getElementById("love-rain").style.display = "block";
    createFireworks();
    createLoveRain();
}

function createFireworks() {
    const fireworksContainer = document.getElementById("fireworks");
    for (let i = 0; i < 20; i++) {
        const firework = document.createElement("div");
        firework.style.top = Math.random() * 100 + "%";
        firework.style.left = Math.random() * 100 + "%";
        fireworksContainer.appendChild(firework);
    }
}

function createLoveRain() {
    const loveRainContainer = document.getElementById("love-rain");
    for (let i = 0; i < 30; i++) {
        const heart = document.createElement("div");
        heart.style.left = Math.random() * 100 + "%";
        heart.style.animationDelay = Math.random() * 2 + "s";
        loveRainContainer.appendChild(heart);
    }
}
