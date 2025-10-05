<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Form Garansi Produk</title>
  <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-gray-100 min-h-screen flex flex-col items-center justify-center">

  <section id="form-section" class="w-full max-w-md bg-white p-6 rounded-2xl shadow-lg">
    <h1 class="text-2xl font-semibold mb-4 text-center text-gray-700">Form Klaim Garansi</h1>
    <form id="claimForm" class="space-y-3">
      <input type="text" id="nama" placeholder="Nama Lengkap" required class="w-full border rounded-lg p-2" />
      <input type="email" id="email" placeholder="Email" required class="w-full border rounded-lg p-2" />
      <input type="text" id="produk" placeholder="Nama Produk" required class="w-full border rounded-lg p-2" />
      <input type="date" id="tanggal" required class="w-full border rounded-lg p-2" />
      <textarea id="alasan" placeholder="Alasan Klaim" required class="w-full border rounded-lg p-2"></textarea>
      <input type="tel" id="wa" placeholder="Nomor WhatsApp (contoh: 628123456789)" required class="w-full border rounded-lg p-2" />

      <div>
        <label class="block text-gray-600 mb-1">Upload Foto Produk</label>
        <input type="file" id="foto" accept="image/*" class="w-full border rounded-lg p-2" />
        <img id="preview" class="mt-2 w-32 h-32 object-cover rounded-lg hidden" />
      </div>

      <button type="submit" class="w-full bg-blue-600 text-white p-2 rounded-lg hover:bg-blue-700">Kirim Klaim</button>
    </form>

    <p class="text-center text-sm text-gray-500 mt-4">
      Admin? <button id="toLogin" class="text-blue-600 underline">Login di sini</button>
    </p>
  </section>

  <section id="login-section" class="hidden w-full max-w-sm bg-white p-6 rounded-2xl shadow-lg">
    <h2 class="text-2xl font-semibold mb-4 text-center text-gray-700">Login Admin</h2>
    <form id="loginForm" class="space-y-3">
      <input type="text" id="username" placeholder="Username" required class="w-full border rounded-lg p-2" />
      <input type="password" id="password" placeholder="Password" required class="w-full border rounded-lg p-2" />
      <button type="submit" class="w-full bg-green-600 text-white p-2 rounded-lg hover:bg-green-700">Masuk</button>
    </form>
    <p class="text-center text-sm text-gray-500 mt-4">
      Kembali ke form? <button id="toForm" class="text-blue-600 underline">Kembali</button>
    </p>
  </section>

  <section id="dashboard" class="hidden w-full max-w-4xl bg-white p-6 rounded-2xl shadow-lg">
    <div class="flex justify-between
