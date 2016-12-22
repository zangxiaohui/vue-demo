<template>
  <main>
    <mt-button type="primary" @click.native="hello">primary</mt-button>
    <hello></hello>
  </main>
</template>

<script>
  import { Button, Toast } from 'mint-ui'

  import Hello from 'components/Hello'

  export default {
    components: {
      MtButton: Button,
      Hello
    },
    methods: {
      hello () {
        Toast({
          message: 'Hello Vue',
          iconClass: 'icon icon-success'
        })
      }
    }
  }
</script>