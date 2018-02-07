<template>
  <div>
    <div class="editor"></div>
  </div>
</template>

<script>
  import TuiEditor from "tui-editor/dist/tui-editor-Editor-all.min"
  require('tui-editor/dist/tui-editor.min.css')

export default {
  name: 'Main',
  data () {
    return {
    }
  },
  mounted: function () {
    var editor = new TuiEditor({
      el: document.querySelector('.editor'),
      initialEditType: 'wysiwyg',
      previewStyle: 'vertical',
    });
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .editor {
    height: 500px;
  }
</style>
