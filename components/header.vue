<template>
    <header class="flex flex-row justify-between items-center px-12 py-3 bg-slate-500 text-white">
        <h1>logo</h1>
        <ul class="flex flex-row items-center gap-4">
          <li>
           <NuxtLink to="/">
            Home
           </NuxtLink>
          </li>

          <li>
           <NuxtLink to="/about">
            about
           </NuxtLink>
          </li>

           <li>
           <NuxtLink to="/cart">
            Keranjang kuning
           </NuxtLink>
          </li>

          <li>
           <NuxtLink to="/dashboard">
           dashboard
           </NuxtLink>
          </li>
          <li>
        <NuxtLink to="/profile">
          Profile
        </NuxtLink>
      </li>
      <li>
        <NuxtLink to="/login">
          Login
        </NuxtLink>
      </li>
      <li>
        <NuxtLink to="/dashboard/transaction">
          Transaksi
        </NuxtLink>
      </li>
        </ul>
    </header>
  </template>
  