<template>
<div class="flex-container-vertical window panels-container" v-bind:class="{big: IsBig}">
<div class="flex-container-horizontal panel-item">
    <div class="icon icon-health"></div>
    <div class="loading-bar f-grow"><div class="loading-bar-line health">
        <div>{{Health}}%</div>
        <div :style="'width:' + Health + '%'">{{Health}}%</div>
    </div></div>
</div>
<div class="flex-container-horizontal panel-item">
    <div class="icon icon-armor"></div>
    <div class="loading-bar f-grow"><div class="loading-bar-line armor">
        <div>{{Armor}}%</div>
        <div :style="'width:' + Armor + '%'">{{Armor}}%</div>
    </div></div>
</div>
</div>
</template>

<script>
module.exports = {
  data: function() {
    return {
      Health: 100,
      Armor: 5,
      IsBig: true
    };
  }
};
</script>

<style lang="css" src="UI/Resources/css/main.css">
</style>