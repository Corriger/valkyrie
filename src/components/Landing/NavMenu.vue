<template>
      <ul id="nav">
          <menu-item
            v-for='item in navMenu'
            v-bind:option='item'
            v-bind:key='item.id'></menu-item>
      </ul>
</template>

<script>
Vue.component('menu-item', {
        props: ['option'],
        template: '<li>{{ option.text }}</li>'
})

var nav = new Vue({
  el: '#nav',
  data: {
    navMenu: [
      { id: 0, text: 'Rundown' },
      { id: 1, text: 'History' },
      { id: 2, text: 'Lifestyle' },
      { id: 3, text: 'Ability' },
      { id: 4, text: 'Unleashed' }
    ]
  }
})

export default {
  name: 'NavMenu'
}
</script>

<style scoped>
ul {
  list-style: none;
  margin: 15px 0;
  display: flex;
  width: 60%;
  justify-content: space-between;
  align-items: center;
}
</style>
