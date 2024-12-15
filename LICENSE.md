<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image Scroll Website</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>

    <div>
        <label for="bpm-input"></label><input type="number" id="bpm-input" min="40" max="240" value="120">
        <button id="start-stop"><span class="ggg">Start</span></button>
        <div id="indicator"></div>
    </div>

    <button class="button12">
        <a href="part2/page2.html" style="text-decoration: none; color: inherit;">Go</a>
    </button>


    <div class="container" id="imageContainer">
        <!-- הכנס תמונות PNG מהמחשב -->
        <img src="images/gggg.png" alt="Image 1">
        <img src="images/gggg1.png" alt="Image 2">
        <img src="images/gggg2.png" alt="Image 3">
        <img src="images/gggg3.png" alt="Image 4">
        <img src="images/gggg4.png" alt="Image 5">
    </div>

    <div class="buttons-container">
        <button id="deleteImages">X</button>
        <button id="uploadImages">!</button>
        <input type="file" id="fileInput" accept="image/*" multiple style="display: none;">
    </div>


    <div class="circle-container">
        <label>
            <input class="circle-input" type="number" min="1" max="100" maxlength="3" />
        </label>
        <span class="percent-symbol">%</span>
    </div>

    <div id="welcomeMessage" class="welcome-message">
        ברוך הבא לאתר! תהנה מהשימוש :)
    </div>

    <div id="welcomeMessageInstructions" class="welcome-message1">
        :להלן הוראות שימוש<br><br>
        בעיגול ניתן לקבוע<br> את מהירות הגלילה באחוזים (מ1 עד 999).<br><br>
        Xכפתור ה<br>pdf/מוחק את התמונות<br><br>
        כפתור ה ! מעלה תמונות חדשות<br><br>
        חדש pdf פותח fכפתור ה <br><br>
        לפעלת הגלילה לחצ/י על התמונה והגלילה תתחיל לחיצה נוספת תעצור אותה
    </div>


    <div class="draggable" id="draggable">
        <button id="searchSongButton">🔍</button>
        <label for="searchSongInput"></label><input type="text" id="searchSongInput" placeholder="שיר/מקצב">
        <button id="prevButton">⬅️</button>
        <button id="toggleButton">⏯️</button>
        <button id="nextButton">➡️</button>
    </div>




    <div class="container">
        <canvas id="pdfCanvas"></canvas>
    </div>
    <div class="buttons-container">
        <button id="uploadPdf">F</button>
        <input type="file" id="pdfInput" accept="application/pdf" style="display: none;">
    </div>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/pdf.js/2.16.105/pdf.min.js"></script>

    <script src="script.js"></script>
</body>

</html>