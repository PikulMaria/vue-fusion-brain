<script>

</script>

<template>
  <div class="container">
    <div class="settings">
      <label for="width">Ширина:</label>
      <input type="number" id="width" name="width" min="100" value="1024">

      <label for="height">Высота:</label>
      <input type="number" id="height" name="height" min="100" value="1024">

      <label for="negativePrompt">Негативный промпт:</label>
      <input type="text" id="negativePrompt" name="negativePrompt" placeholder="Яркие цвета, кислотность, высокая контрастность">

      <label for="style">Стиль:</label>
      <select id="style" name="style">
        <option value="string">Свой стиль (впишите ниже)</option>
        <option value="style1">Стиль 1</option>
        <option value="style2">Стиль 2</option>
        <option value="style3">Стиль 3</option>
      </select>

      <textarea id="customStyle" name="customStyle" placeholder="Ваш стиль..."></textarea>

      <button onclick="">Генерация</button>
    </div>

    <div class="image-container">
      <label for="imageName">Название картинки:</label>
      <input type="text" id="imageName" name="imageName" placeholder="Введите название">

      <img id="generatedImage" src="#" alt="Generated Image">
    </div>
  </div>
</template>



<style>
#app {
  body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
  }

  .container {
    display: flex;
    justify-content: space-around;
    align-items: center;
    height: 100vh;
  }

  .settings {
    width: 300px;
  }

  .settings label,
  .settings select,
  .settings input,
  .settings textarea {
    display: block;
    margin-bottom: 10px;
  }

  .image-container {
    text-align: center;
  }

  #generatedImage {
    max-width: 100%;
    max-height: 400px;
    border: 2px solid #333;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
  }
}
</style>
