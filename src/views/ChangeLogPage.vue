<template>
  <div class="about">
    <h1>Change log</h1>
    <div class="container">
      <at-timeline pending>
        <at-timeline-item color="red">
          <i slot="dot" class="icon icon-package"></i>
          <p>Install framework</p>
          <small>17.07.18</small>
        </at-timeline-item>
        <at-timeline-item color="green">
          <i slot="dot" class="icon icon-settings"></i>
          <p>Vue init</p>
          <small>17.07.18</small>
        </at-timeline-item>
      </at-timeline>
    </div>
  </div>
</template>

<style lang="scss">
  .at-timeline {
    .at-timeline__content {
      top: -3px;
      padding: 0 0 20px 24px;
    }
  }
</style>