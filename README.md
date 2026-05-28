# Digital-clock

<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <title>digital clock</title>
</head>
<body>
    <h1 id="clock"></h1>

    <script>
        function updateClock() {
            const now = new Date();
            const options = { 
                hour: '2-digit', 
                minute: '2-digit', 
                second: '2-digit',
                hour12: false 
            };
            document.getElementById('clock').textContent = now.toLocaleTimeString('fa-IR', options);
        }

        setInterval(updateClock, 1000);
        updateClock();
    </script>
</body>
</html>
