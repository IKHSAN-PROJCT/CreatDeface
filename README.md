<h1>Hallo Selamat datang di Script Pembuatan tampilan Deface</h1>

<h>Selamat mencoba script yang saya buat ya!!</h>

<p>Jangan Di record...</p>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Copy Commands</title>
</head>
<body>
    <textarea id="commandTextArea" rows="10" cols="50" style="display: none;">
apt update -y
apt upgrade -y
pkg update -y
pkg upgrade -y
pkg install git -y
git clone https://github.com/MR-JHONz/CreatDeface
cd CreatDeface
bash Def.sh
    </textarea>

    <button onclick="copyCommands()">Salin Semua Perintah</button>

    <script>
        function copyCommands() {
            var commandTextArea = document.getElementById("commandTextArea");
            commandTextArea.style.display = "block"; // Menampilkan textarea agar bisa dipilih
            commandTextArea.select(); // Memilih teks dalam textarea
            document.execCommand("copy"); // Menyalin teks yang telah dipilih
            commandTextArea.style.display = "none"; // Menyembunyikan textarea kembali setelah disalin
            alert("Perintah telah disalin!");
        }
    </script>
</body>
</html>
Jangan lupa subscribe channel saya

<button><a href="https://youtube.com/@sanzacil_026">Subscribe</a></button>
