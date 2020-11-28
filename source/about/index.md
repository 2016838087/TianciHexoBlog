---
title: 关于
photos: https://cdn.jsdelivr.net/gh/2016838087/SakuraHexoFile@master/themes/images/background/lonely.png
comment: false
---
{% raw %}
<!-- 因为vue和botui更新导至bug,现将对话移至js下的botui中配置 -->
<div class="entry-content">
  <div class="moe-mashiro" style="text-align:center; font-size: 50px; margin-bottom: 20px;">关于博🐷
  </div>
  <div id="hello-mashiro" class="popcontainer" style="min-height: 300px; padding: 2px 6px 4px; background-color: rgba(242, 242, 242, 0.5); border-radius: 10px;">
    <center>
    <p>
    </p>
    <h4>
    与Tianci对话中...
    </h4>
    <p>
    </p>
    </center>
    <bot-ui></botui>
  </div>
</div>
<!-- <script src="../js/about.js"></script> -->
<script src="https://cdn.jsdelivr.net/gh/2016838087/SakuraHexoFile@master/themes/js/botui.js"></script>
<script>
bot_ui_ini()
</script>
{% endraw %}