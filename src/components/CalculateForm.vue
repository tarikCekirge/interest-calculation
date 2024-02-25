<script setup></script>

<template>
  <div class="calculate-form">
    <form class="space-y-3">
      <h1 class="text-2xl font-bold text-center dark:text-gray-50">Interest Calculation</h1>
      <div class="row">
        <h2 class="row-title">Present Value:</h2>
        <input type="text" class="value-input" />
      </div>
      <div class="row">
        <h2 class="row-title">Interest Rate:</h2>
        <input type="text" class="col-span-2" />
        <select name="" id="">
          <option value="">1</option>
          <option value="">2</option>
          <option value="">3</option>
        </select>
      </div>
      <div class="row">
        <h2 class="row-title">Term:</h2>
        <input type="text" class="col-span-2" />
        <select name="" id="">
          <option value="">1</option>
          <option value="">2</option>
          <option value="">3</option>
        </select>
      </div>
      <button>Calculate</button>
    </form>
  </div>
</template>

<style scoped>
.calculate-form {
  @apply w-full max-w-2xl bg-slate-300 dark:bg-gray-700 rounded-md p-4 shadow-xl text-gray-800 dark:text-gray-50;
}

.calculate-form .row {
  @apply grid grid-cols-4 gap-3 place-items-stretch;
}
.calculate-form .row .row-title {
  @apply self-center font-semibold;
}
.calculate-form .row input,
.calculate-form .row select {
  @apply p-2 block w-full rounded-md bg-gray-100 dark:bg-slate-600 border border-transparent outline-0  focus:border-slate-400 dark:focus:border-slate-400 focus:bg-white dark:focus:bg-slate-500 outline-none focus:ring-0 focus:ring-offset-0;
}
.calculate-form .row .value-input {
  @apply col-span-3;
}

.calculate-form button {
  @apply p-2 flex mx-auto justify-center text-slate-100 font-bold w-full max-w-32 rounded-md bg-slate-600 dark:bg-gray-100 dark:text-gray-700;
}
</style>
