<template>
    <main class="flex flex-col items-center justify-center h-screen bg-gradient-to-b from-rose-200 to-rose-400 p-6">
      <div class="bg-white shadow-lg rounded-xl p-6 w-72 text-center">
        <img src="https://via.placeholder.com/100" alt="Profile Picture" class="w-24 h-24 mx-auto rounded-full mb-4" />
        <h1 class="text-xl font-bold text-gray-800">Timur Ivanov</h1>
        <p class="text-gray-600">Frontend Developer</p>
        <p class="text-gray-500 text-sm mt-2">"Creating interactive and modern web experiences."</p>
        <div class="mt-4 space-y-2">
          <p class="text-gray-700"><strong>📍 Location:</strong> Almaty, Kazakhstan</p>
          <p class="text-gray-700"><strong>📞 Phone:</strong> +7 777 123 4567</p>
          <p class="text-gray-700 flex justify-center items-center gap-2">
            <strong>📧 Email:</strong> timur@example.com
            <button @click="copyEmail" class="text-blue-500 hover:underline">📋</button>
          </p>
        </div>
      </div>
    </main>
  </template>
  
  <script setup lang="ts">
  const copyEmail = () => {
    navigator.clipboard.writeText("timur@example.com");
    alert("Email copied to clipboard!");
  };
  </script>
  