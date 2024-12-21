<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Механика</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f8ff;
            color: #333;
        }

        header {
            background-color: #4682b4;
            color: white;
            padding: 20px;
            text-align: center;
        }

        main {
            padding: 20px;
            text-align: center;
        }

        .buttons {
            margin-bottom: 20px;
        }

        button {
            background-color: #87cefa;
            border: none;
            border-radius: 5px;
            padding: 10px 20px;
            margin: 5px;
            cursor: pointer;
            font-size: 16px;
        }

        button:hover {
            background-color: #4682b4;
            color: white;
        }

        #content {
            margin-top: 20px;
            padding: 20px;
            border: 1px solid #ddd;
            border-radius: 5px;
            background-color: #ffffff;
        }
    </style>
</head>
<body>
    <header>
        <h1>Механика: Физикаға Қош Келдіңіз!</h1>
    </header>
    <main>
        <div class="buttons">
            <button onclick="showContent('theory')">Теория</button>
            <button onclick="showContent('formulas')">Формула</button>
            <button onclick="showContent('examples')">Мысал</button>
            <button onclick="showContent('problems')">Есеп</button>
        </div>
        <section id="content">
            <p>Қажетті бөлімді таңдап басыңыз.</p>
        </section>
    </main>
    <script>
        function showContent(section) {
            const content = {
                theory: `<h2>Теория</h2><p>Механика — денелердің қозғалысын және өзара әрекеттесуін зерттейтін физиканың бір бөлімі.</p>`,
                formulas: `<h2>Формула</h2><p>Негізгі формулалар: <br> 1. v = s / t (Жылдамдық) <br> 2. a = Δv / t (Үдеу) <br> 3. F = m * a (Ньютонның екінші заңы).</p>`,
                examples: `<h2>Мысал</h2><p>Егер дене 10 м/с жылдамдықпен 5 секунд қозғалған болса, оның жүрген жолы: s = v * t = 10 * 5 = 50 м.</p>`,
                problems: `<h2>Есеп</h2><p><strong>Есеп:</strong> Массасы 5 кг денеге 10 Н күш әсер етеді. Үдеуді табыңыз.<br><strong>Шешімі:</strong> a = F / m = 10 / 5 = 2 м/с².</p>`
            };

            document.getElementById("content").innerHTML = content[section] || "<p>Мәлімет табылмады.</p>";
        }
    </script>
</body>
</html>
