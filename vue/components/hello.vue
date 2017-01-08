Vue.component('hello', {
  props: ['message'],
  template: '\
    <div>\
      <h1>Hello, {{ showMessage }}</h1>\
    </div>\
  ',
  computed: {
    showMessage: function() {
      return this.message === undefined ? '___' : this.message
    }
  }
})
