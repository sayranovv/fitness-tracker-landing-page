<script>

</script>

<template>
    <label class="custom-checkbox">
      <input type="checkbox" id="checkbox1">
      <span class="checkmark"></span>
    </label>
</template>

<style scoped>
.custom-checkbox input[type="checkbox"] {
  display: none;
}

/* Стиль для метки */
.custom-checkbox {
  position: relative;
  padding-left: 30px;
  cursor: pointer;
  user-select: none;
  color: #474A57;
}

/* Создание кастомной чекбокс-метки */
.checkmark {
  position: absolute;
  top: 0;
  left: 0;
  height: 32px; /* Высота чекбокса */
  width: 32px; /* Ширина чекбокса */
  background-color: #FA6648; /* Цвет фона по умолчанию */
  border: 2px solid #1C1C1D;
  border-radius: 5px; /* Скругление углов */
}

.custom-checkbox:hover .checkmark {
  background-color: #fff;
}

/* Стиль для чекбокса, когда он отмечен */
.custom-checkbox input:checked + .checkmark {
  background-color: #FFBD12; /* Цвет при отметке */
}

/* Создание галочки */
.checkmark:after {
  content: "";
  position: absolute;
  display: none;
}

/* Показ галочки, когда чекбокс отмечен */
.custom-checkbox input:checked + .checkmark:after {
  display: block;
}

/* Галочка */
.checkmark:after {
  left: 8px; /* Положение галочки */
  top: 3px; /* Положение галочки */
  width: 7px; /* Ширина галочки */
  height: 13px; /* Высота галочки */
  border: solid #1C1C1D; /* Цвет галочки */
  border-width: 0 3px 3px 0; /* Размеры галочки */
  transform: rotate(45deg); /* Поворот для создания галочки */
}
</style>