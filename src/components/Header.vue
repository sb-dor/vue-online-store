<template>
  <header class="flex justify-between border-b border-state-300 p-8">
    <div class="flex items-center gap-2">
      <img src="/logo.png" alt="Logo" class="w-10" />
      <div>
        <h2 class="text-xl font-bold uppercase">Vue Sneakers</h2>
        <p class="text-slate-400">Магазин лучших кроссовок</p>
      </div>
    </div>

    <ul class="flex items-center gap-7">
      <li class="flex items-center gap-3 text-gray-500 hover:text-black cursor-pointer">
        <img src="/cart.svg" alt="Cart" />
        <b>1200р</b>
      </li>

      <li class="flex items-center gap-3 text-gray-500 hover:text-black cursor-pointer">
        <img src="/heart.svg" alt="Cart" />
        <b>Закладки</b>
      </li>

      <li class="flex items-center gap-3 text-gray-500 hover:text-black cursor-pointer">
        <img src="/profile.svg" alt="Cart" />
        <b>Профиль</b>
      </li>
    </ul>
  </header>
</template>
