<script>
import { DashboardLayoutComponent, PanelsDirective, PanelDirective } from '@syncfusion/ej2-vue-layouts';

export default {
  components: {
    'ejs-dashboardlayout' : DashboardLayoutComponent,
    'e-panels' : PanelsDirective,
    'e-panel' : PanelDirective
  }
}
</script>

<template>
  <ejs-dashboardlayout columns="3" :allowDragging="false" :allowResizing="true">
    <e-panels>
      <e-panel :row="0" :col="0" :sizeY="2" :minSizeY="1" :maxSizeY="2" header="<div>Panel 1</div>" content="<div>Content of Panel 1</div>"></e-panel>
      <e-panel :row="0" :col="1" header="<div>Panel 2</div>" content="<div>Content of Panel 2</div>"></e-panel>
      <e-panel :col="2" header="<div>Panel 3</div>" content="<div>Content of Panel 3</div>"></e-panel>
      <e-panel :row="1" :col="1" :sizeX="2" :minSizeX="1" :maxSizeX="2" header="<div>Panel 4</div>" content="<div>Content of Panel 4</div>"></e-panel> 
    </e-panels>
  </ejs-dashboardlayout>
</template>

<style>
  @import "../node_modules/@syncfusion/ej2-base/styles/material.css";
  @import "../node_modules/@syncfusion/ej2-vue-layouts/styles/material.css";

  .e-panel-header {
    text-align: center;
  }
  .e-panel-content {
    text-align: center;
  }
</style>
