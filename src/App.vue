<template>
  <h1>hello</h1>
</template>

<script>
new Vue({
  el: 'body',
  data: {
    currentComponent: null,
    componentsArray: ['foo', 'bar']
  },
  components: {
    'foo': {
      template: '<h1>Foo component</h1>'
    },
    'bar': {
      template: '<h1>Bar component</h1>'
    }
  },
  methods: {
    swapComponent: function (component) {
      this.currentComponent = component;
    }
  }
})
</script>