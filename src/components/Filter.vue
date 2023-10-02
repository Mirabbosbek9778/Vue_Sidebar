<script setup></script>
<template>
  <div>
    <h1 class="text-white">Фильмы</h1>
    <div class="flex gap-[10px] pt-8">
      <div>
        <select>
          <option>Комедия</option>
          <option>Комедия1</option>
          <option>Комедия2</option>
          <option>Комедия3</option>
        </select>
      </div>
      <div>
        <select>
          <option>2020 – 2023</option>
          <option>2021 – 2023</option>
          <option>2022 – 2023</option>
          <option>2023 – 2023</option>
        </select>
      </div>
      <div>
        <select>
          <option>Disney</option>
          <option>Disney1</option>
          <option>Disney2</option>
          <option>Disney3</option>
        </select>
      </div>
      <div>
        <select>
          <option>По умолчанию</option>
          <option>По умолчанию1</option>
          <option>По умолчанию2</option>
          <option>По умолчанию3</option>
        </select>
      </div>
    </div>
  </div>
</template>
<style lang="scss" scoped>
h1 {
  color: #fff;
  font-family: SF Pro Display, sans-serif;
  font-size: 40px;
  font-style: normal;
  font-weight: 600;
  line-height: 100%;
  padding-top: 55px;
}
select {
  color: #808080;
  width: 340px;
  height: 64px;
  border-radius: 200px;
  background: rgba(255, 255, 255, 0.1);
  padding: 0px 32px;
  option {
    font-family: SF Pro Display, sans-serif;
    font-size: 24px;
    font-style: normal;
    font-weight: 500;
    line-height: 100%;
  }
}
</style>
