<h1>Hallo Selamat datang di Script Pembuatan tampilan Deface</h1>

<h>Selamat mencoba script yang saya buat ya!!</h>

<p>Jangan Di record...</p>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Auto Copy Text</title>
</head>
<body>
    <!-- Shell commands -->
    <pre id="shellCommands" style="display: none;">
apt update -y
apt upgrade -y
pkg update -y
pkg upgrade -y
pkg install git -y
git clone https://github.com/MR-JHONz/CreatDeface
cd CreatDeface
bash Def.sh
    </pre>

    <!-- Text to be copied -->
    <p id="textToCopy" style="display: none;">Ini text yang nanti akan disalin.</p>

    <!-- JavaScript to automatically copy shell commands and text -->
    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Copy shell commands
            var shellCommands = document.getElementById("shellCommands").innerText;
            copyToClipboard(shellCommands);

            // Copy additional text
            var textToCopy = document.getElementById("textToCopy").innerText;
            copyToClipboard(textToCopy);
        });

        function copyToClipboard(text) {
            var tempInput = document.createElement("input");
            tempInput.value = text;
            document.body.appendChild(tempInput);
            tempInput.select();
            document.execCommand("copy");
            document.body.removeChild(tempInput);
            console.log("Teks telah disalin: " + text);
        }
    </script>
</body>
</html>
Jangan lupa subscribe channel saya

<button><a href="https://youtube.com/@sanzacil_026">Subscribe</a></button>
