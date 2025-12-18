// LOGIN PALSU (tanpa keamanan)
function login() {
  const user = document.getElementById("username").value;
  const pass = document.getElementById("password").value;
  const error = document.getElementById("error");

  if (user === "admin" && pass === "12345") {
    window.location.href = "dashboard.html";
  } else {
    error.innerText = "Username atau password salah!";
  }
}

// UPLOAD GAMBAR (hanya preview)
function uploadGambar() {
  const file = document.getElementById("gambar").files[0];
  const hasil = document.getElementById("hasil");

  if (!file) {
    alert("Pilih gambar dulu!");
    return;
  }

  const reader = new FileReader();
  reader.onload = function(e) {
    hasil.innerHTML = `
      <p>Gambar berhasil diunggah:</p>
      <img src="${e.target.result}" width="200">
    `;
  };
  reader.readAsDataURL(file);
}
