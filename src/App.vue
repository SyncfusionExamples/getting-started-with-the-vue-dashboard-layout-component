<template>
  <ejs-dashboardlayout columns="3" :allowResizing="true" >
    <e-panels>
       <e-panel :row="0" :col="0"  header="<div>Panel 1</div>"   ></e-panel>
       <!-- <e-panel :row="0" :col="1" header="<div>Panel 2</div>" content="<div>content of panel 2</div>" ></e-panel>
       <e-panel :row="0" :col="2" header="<div>Panel 3</div>" content="<div>content of panel 3</div>" ></e-panel> -->
       <e-panel :row="10" :col="0"  header="<div>Panel 2</div>" ></e-panel>
      </e-panels>
  </ejs-dashboardlayout>
</template>

<script setup>
  import { DashboardLayoutComponent as EjsDashboardlayout, PanelDirective as EPanel, PanelsDirective as EPanels } from "@syncfusion/ej2-vue-layouts";
</script>

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