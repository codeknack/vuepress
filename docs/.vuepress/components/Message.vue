<template>
  <article class="message is-info" :class="{hidden: dismiss}">
    <div class="message-header">
      <p>Welcome to Our Blog</p>
      <button @click="hide" class="delete"></button>
    </div>
    <div class="message-body">
      Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque risus mi, tempus quis placerat ut, porta nec nulla. Vestibulum rhoncus ac ex sit amet fringilla. Nullam gravida purus diam, et dictum felis venenatis efficitur. Aenean aceleifend lacus, in mollis lectus. Donec sodales, arcu et sollicitudin porttitor, tortor urna tempor ligula, id porttitor mi magna a neque. Donec dui urna, vehicula et sem eget, facilisis sodales sem.
    </div>
  </article>
</template>

<script>
  export default {
    data: function() {
      return {
        dismiss: false
      };
    },
    methods: {
      hide() {
        this.dismiss = true;
      }
    }
  };
</script>

<style>
  .hidden {
    display: none;
  }
</style>

