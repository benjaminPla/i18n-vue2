<template>
  <div>
    <h1>i18n</h1>
    <h2>{{ $t('message.hello') }}</h2>
    <select v-model='$i18n.locale'>
      <option v-for='(lang, index) in langs' :key='index'>{{ lang }}</option>
    </select>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
  },
  data() {
    return { langs: ['en', 'ja'] };
  },
};
</script>
