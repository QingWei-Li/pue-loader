template
  div
    span {{ count }}
    button(@click="count++") +
    button(@click="count--") -

script
  export default {
    name: 'compo'
    data: () ->
      count: 0
  }

style
  span
    color red
