---
title: ""
format:
  html:
    theme: lumen
    page-layout: full
    self-contained: true
    code-fold: true
    code-overflow: wrap
    html-math-method: mathjax
    include-after-body:
      text: |
        <script>
          document.addEventListener("DOMContentLoaded", function () {
              var toc = document.createElement("div");
              toc.id = "custom-toc";
              toc.style.position = "fixed";
              toc.style.top = "0";
              toc.style.right = "-300px";  // Start hidden
              toc.style.width = "260px";
              toc.style.height = "100%";
              toc.style.background = "white";
              toc.style.padding = "10px";
              toc.style.boxShadow = "0px 2px 5px rgba(0, 0, 0, 0.2)";
              toc.style.transition = "right 0.3s ease-in-out";
              toc.style.overflowY = "auto";
          
              var tocTitle = document.createElement("h3");
              tocTitle.innerText = "Navigation";
              toc.appendChild(tocTitle);
          
              var headers = document.querySelectorAll("h2, h3, h4");
              headers.forEach(function (header, index) {
                  if (!header.id) {
                      header.id = "section-" + index;
                  }
          
                  var link = document.createElement("a");
                  link.innerText = header.innerText;
                  link.href = "#" + header.id;
                  link.style.display = "block";
                  link.style.padding = "5px 0";
                  link.style.color = "#007bff";
                  link.style.textDecoration = "none";
          
                  toc.appendChild(link);
              });
          
              document.body.appendChild(toc);
          
              // Create toggle button (📑 icon)
              var button = document.createElement("button");
              button.id = "toggle-toc";
              button.innerHTML = "📑";
              button.style.position = "fixed";
              button.style.top = "15px";
              button.style.right = "15px";
              button.style.backgroundColor = "white";
              button.style.color = "#333";
              button.style.border = "2px solid #ccc"; // Slightly thicker border
              button.style.padding = "10px 12px"; // Increased padding
              button.style.cursor = "pointer";
              button.style.borderRadius = "8px"; // More rounded
              button.style.fontSize = "22px"; // Larger icon
              button.style.zIndex = "1000";
              button.style.boxShadow = "0px 3px 6px rgba(0, 0, 0, 0.2)";
              button.style.width = "50px"; // Increase button size
              button.style.height = "50px"; // Make it square
          
              document.body.appendChild(button);
          
              // Click event to toggle the ToC
              button.addEventListener("click", function () {
                  if (toc.style.right === "0px") {
                      toc.style.right = "-300px"; // Hide ToC
                  } else {
                      toc.style.right = "0px"; // Show ToC
                  }
              });
          });
          document.addEventListener("DOMContentLoaded", function () {
              document.querySelectorAll("a[href='https://favstats.github.io/de25/']").forEach(function(link) {
                  link.addEventListener("click", function(event) {
                      event.preventDefault(); // Prevent default behavior
                      window.open(link.href, "_blank"); // Open in a new tab/window
                  });
              });
          });
        </script>
    includes:
      in-header: |
        <script src="https://cdn.jsdelivr.net/npm/apexcharts"></script>

---


<style>
  /* Color all Markdown bold text */
  main.content strong,
  main.content b {
    color: #0d6efd !important;  /* nice blue; override theme if needed */
    font-weight: 700;           /* keep it bold */
  }
</style>



> WARNING THIS ONLY SHOWS A MOCK-UP THE DATA IS NOT REAL YET! DO NOTE CITE.





::: {.cell}
<style type="text/css">
/* Modern, Subtle Blockquote Styling */
blockquote {
  background: #f9f9f9;  /* Light gray background for subtlety */
  border-left: 4px solid #6c63ff;  /* Soft purple left border for a modern touch */
  padding: 1rem 1.5rem;  /* Adequate padding for readability */
  margin: 1.5rem 0;  /* Space around blockquote */
  font-style: italic;  /* Classic blockquote style */
  color: #333;  /* Dark text for good contrast */
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05);  /* Light shadow for depth */
  border-radius: 8px;  /* Rounded corners for a modern feel */
  transition: background-color 0.3s ease, border-color 0.3s ease;  /* Smooth hover transition */
}

/* Hover effect for subtle interaction */
blockquote:hover {
  background: #f0f0ff;  /* Very light purple on hover */
  border-left-color: #4e47d6;  /* Slightly darker purple on hover */
}
</style>
:::




In de **CampAIgn Tracker** analyseren we alle *berichten* op *Facebook, Instagram, TikTok en X* van *partijen en kandidaten* en *geselecteerde influencers en commentatoren* voor de **Tweede Kamerverkiezingen van 2025**.  

De **live monitoring** laat zien **hoeveel AI-gegenereerde berichten** door welke partijen worden verspreid. Daarnaast tonen we *of AI-labels* worden gebruikt, welke *actoren* in beeld komen, welke *thema’s aan bod komen* en of de *toon positief of negatief* is.  

Op deze pagina vindt u *analyses van AI-gegenereerde campagnes voor de Tweede Kamerverkiezingen van 2025*. Een doorzoekbaar overzicht van afzonderlijke AI-gegenereerde afbeeldingen en video’s is beschikbaar in de [AI Explorer](https://favstats.github.io/campaigntrackernl/explore).


::: {.cell}

:::

::: {.cell}

:::

::: {.cell}
::: {.cell-output-display}
```{=html}
<div style="&#10;    display: flex; &#10;    justify-content: space-between; &#10;    align-items: flex-start; &#10;    gap: 20px;  /* Adds space between boxes */&#10;    padding: 10px;&#10;  ">
<div style="flex: 1; min-width: 300px;">
<div id="htmlwidget-381ab158105c6c76e5ea" style="width:100%;height:160px;" class="apexcharter html-widget"></div>
<script type="application/json" data-for="htmlwidget-381ab158105c6c76e5ea">{"x":{"ax_opts":{"chart":{"type":"area","sparkline":{"enabled":true}},"series":[{"name":"n","type":"area","data":[[1758067200000,797],[1758153600000,774],[1758240000000,675],[1758326400000,638],[1758412800000,521],[1758499200000,690],[1758585600000,768],[1758672000000,745],[1758758400000,836]]}],"dataLabels":{"enabled":false},"stroke":{"curve":"straight","width":2},"yaxis":{"decimalsInFloat":2,"labels":{"style":{"colors":"#848484"}},"show":false},"xaxis":{"type":"datetime","labels":{"style":{"colors":"#848484"}}},"colors":["#2E93fA"],"title":{"text":6444,"style":{"fontSize":"24px"}},"subtitle":{"text":"Totaal aantal gevolgde berichten","style":{"fontSize":"14px"}}},"auto_update":{"series_animate":true,"update_options":true,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":{"color":"#2E93fA","background":"#FFF"},"xaxis":{"min":"2025-09-17T00:00:00Z","max":"2025-09-25T00:00:00Z"},"type":"area"},"evals":[],"jsHooks":[]}</script>
</div>
<div style="flex: 1; min-width: 300px;">
<div id="htmlwidget-10dc537822a87f863ebd" style="width:100%;height:160px;" class="apexcharter html-widget"></div>
<script type="application/json" data-for="htmlwidget-10dc537822a87f863ebd">{"x":{"ax_opts":{"chart":{"type":"area","sparkline":{"enabled":true}},"series":[{"name":"n","type":"area","data":[[1758067200000,5],[1758153600000,10],[1758240000000,5],[1758326400000,9],[1758412800000,8],[1758499200000,9],[1758585600000,10],[1758672000000,5],[1758758400000,9]]}],"dataLabels":{"enabled":false},"stroke":{"curve":"straight","width":2},"yaxis":{"decimalsInFloat":2,"labels":{"style":{"colors":"#848484"}},"show":false},"xaxis":{"type":"datetime","labels":{"style":{"colors":"#848484"}}},"colors":["#FFF"],"title":{"text":70,"style":{"fontSize":"22px","color":"#FFF"}},"subtitle":{"text":"Totaal aantal geïdentificeerde AI-berichten","style":{"fontSize":"14px","color":"#FFF"}}},"auto_update":{"series_animate":true,"update_options":true,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":{"color":"#FFF","background":"#1E90FF"},"xaxis":{"min":"2025-09-17T00:00:00Z","max":"2025-09-25T00:00:00Z"},"type":"area"},"evals":[],"jsHooks":[]}</script>
</div>
</div>
```
:::
:::

::: {.cell}

:::


<br>

#  Overzicht van Inhoud

Hier laten we zien hoeveel AI-inhoud we hebben gevonden, uitgesplitst naar **platform**, **actortype** en **politieke voorkeur**.

We onderscheiden **partijen en politici** van **andere actoren**, zoals commentatoren, influencers, fanpagina's en meme-pagina's.

::: {.panel-tabset}


## Naar Partij / Actor {#ki-content-by-party2}




::: {.cell-output-display}
```{=html}
<style>
  .apex-container2 {
    max-width: 100%;
    height: auto;
    overflow-x: auto;    /* Horizontal scroll if needed */
    overflow-y: auto;    /* Vertical scroll if needed */
    padding: 20px;
    background-color: #f8f9fa; /* Light background */
    border: 1px solid #ccc;    /* Subtle border */
    border-radius: 10px;       /* Rounded corners */
  }
</style>
<div class="apex-container2">
<div id="htmlwidget-95527aca53da0bb71e28" style="width:100%;height:400px;" class="apexcharter html-widget"></div>
<script type="application/json" data-for="htmlwidget-95527aca53da0bb71e28">{"x":{"ax_opts":{"chart":{"type":"treemap","toolbar":{"show":false}},"series":[{"name":"y","data":[{"x":"PVV","y":17},{"x":"Pro-PVV","y":9},{"x":"VVD","y":9},{"x":"BBB","y":4},{"x":"GL-PvdA","y":4},{"x":"De Linie","y":3},{"x":"50PLUS","y":3},{"x":"NCPN","y":3},{"x":"Protest Accounts","y":3},{"x":"SP","y":3},{"x":"DENK","y":2},{"x":"FvD","y":2},{"x":"Vrede voor Dieren","y":1},{"x":"LP","y":1},{"x":"BVNL","y":1},{"x":"Satire","y":1},{"x":"CU","y":1},{"x":"JA21","y":1},{"x":"SGP","y":1},{"x":"D66","y":1}]}],"yaxis":{"labels":{"style":{"colors":"#848484"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}}},"title":{"text":"Naar Partij / Actor","align":"center","style":{"fontSize":"16px"}},"legend":{"show":false},"colors":["#003082","#B22222","#FF7900","#009639","#C00040","#AA3377","#7F2481","#CC0000","#EE6677","#BE1E2D","#00A7B3","#7B1E26","#5496c6","#003399","#132141","#6A5ACD","#00A1DE","#0C2E6E","#E57200","#009E60"],"plotOptions":{"treemap":{"distributed":true,"enableShades":false,"dataLabels":{"enabled":true,"style":{"fontSize":"12px"}}}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"50PLUS","max":"VVD"},"type":"treemap"},"evals":[],"jsHooks":[]}</script>
</div>
```
:::



Deze visualisatie laat zien hoeveel AI-gegenereerde inhoud elke partij, politicus of andere actor heeft gepubliceerd. De veldgrootte komt overeen met het aantal geïdentificeerde berichten. Grotere velden duiden op een hoger gebruik van AI door de betreffende partij/actor.



## Per Platform {#ki-content-by-party2}


::: {.cell}
::: {.cell-output-display}
```{=html}
<style>
  .apex-container0 {
    max-width: 100%;
    height: auto;
    overflow-x: auto;    /* Horizontal scroll if needed */
    overflow-y: auto;    /* Vertical scroll if needed */
    padding: 20px;
    background-color: #f8f9fa; /* Light background */
    border: 1px solid #ccc;    /* Subtle border */
    border-radius: 10px;       /* Rounded corners */
  }
</style>
<div class="apex-container0">
<div id="htmlwidget-6bdb1a4861c07cd952e3" style="width:100%;height:400px;" class="apexcharter html-widget"></div>
<script type="application/json" data-for="htmlwidget-6bdb1a4861c07cd952e3">{"x":{"ax_opts":{"chart":{"type":"treemap","toolbar":{"show":false}},"series":[{"name":"y","data":[{"x":"Facebook","y":37},{"x":"Instagram","y":27},{"x":"TikTok","y":6}]}],"yaxis":{"labels":{"style":{"colors":"#848484"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}}},"title":{"text":"Per Platform","align":"center","style":{"fontSize":"16px"}},"legend":{"show":false},"colors":["#1877F2","#E4405F","#69C9D0"],"plotOptions":{"treemap":{"distributed":true,"enableShades":false,"dataLabels":{"enabled":true,"style":{"fontSize":"12px"}}}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"Facebook","max":"TikTok"},"type":"treemap"},"evals":[],"jsHooks":[]}</script>
</div>
```
:::
:::




## Naar Actortype {#ki-content-by-party2}




::: {.cell-output-display}
```{=html}
<style>
  .apex-container {
    max-width: 100%;
    height: auto;
    overflow-x: auto;    /* Horizontal scroll if needed */
    overflow-y: auto;    /* Vertical scroll if needed */
    padding: 20px;
    background-color: #f8f9fa; /* Light background */
    border: 1px solid #ccc;    /* Subtle border */
    border-radius: 10px;       /* Rounded corners */
  }
</style>
<div class="apex-container">
<div id="htmlwidget-300068743b46a7d43f49" style="width:100%;height:400px;" class="apexcharter html-widget"></div>
<script type="application/json" data-for="htmlwidget-300068743b46a7d43f49">{"x":{"ax_opts":{"chart":{"type":"treemap","toolbar":{"show":false}},"series":[{"name":"y","data":[{"x":"Parties","y":52},{"x":"Fans","y":13},{"x":"Politicians","y":5}]}],"yaxis":{"labels":{"style":{"colors":"#848484"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}}},"title":{"text":"Naar Actortype","align":"center","style":{"fontSize":"16px"}},"legend":{"show":false},"colors":["#D55E00","#009E73","#0072B2"],"plotOptions":{"treemap":{"distributed":true,"enableShades":false,"dataLabels":{"enabled":true,"style":{"fontSize":"12px"}}}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"Fans","max":"Politicians"},"type":"treemap"},"evals":[],"jsHooks":[]}</script>
</div>
```
:::


::: 


## Aandeel berichten met en zonder AI {#ki-content-by-party2}



::: {.panel-tabset}


::: {.cell}

:::



### Partijen & Politici


::: {.cell}
::: {.cell-output-display}
```{=html}
<style>
  .apex-container {
    max-width: 100%;
    height: auto;
    overflow-x: auto;    /* Horizontal scroll if needed */
    overflow-y: auto;    /* Vertical scroll if needed */
    padding: 20px;
    background-color: #f8f9fa; /* Light background */
    border: 1px solid #ccc;    /* Subtle border */
    border-radius: 10px;       /* Rounded corners */
  }
</style>
<div class="apex-container">
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-874876ae5aa00d90a1b9" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-874876ae5aa00d90a1b9">{"x":{"ax_opts":{"chart":{"type":"bar","stacked":true,"events":{"mounted":"\n        function(chart) {\n          setTimeout(function() {\n            chart.toggleSeries('Berichten zonder AI'); // Hides the non-AI series initially\n          }, 500); // Short delay ensures the chart is fully loaded\n        }\n      "},"height":"5000px"},"plotOptions":{"bar":{"horizontal":true,"barHeight":"70%","columnWidth":"85%"}},"xaxis":{"categories":["De Linie","50PLUS","NCPN","Vrede voor Dieren","LP","PVV","VVD","BVNL","DENK","CU","BBB","GL-PvdA","SP","JA21","FvD","SGP","D66"]},"series":[{"name":"Berichten met AI","data":[60,27.27272727272727,23.07692307692308,9.090909090909092,4.166666666666666,3.917050691244239,3.03030303030303,2.380952380952381,1.904761904761905,1.785714285714286,1.769911504424779,1.201201201201201,1.195219123505976,0.9708737864077669,0.8130081300813009,0.641025641025641,0.398406374501992]}],"colors":["#6c757d","#17a2b8"],"dataLabels":{"enabled":true,"formatter":"function(val) { return val.toFixed(1) + '%'; }"},"legend":{"position":"top","showForSingleSeries":true,"markers":{"fillColors":["#6c757d","#17a2b8"]},"onItemClick":{"toggleDataSeries":true},"onItemHover":{"highlightDataSeries":true}},"tooltip":{"y":{"formatter":"\n        function(val, opts) { \n          return val.toFixed(2) + '%'; \n        }"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false},"evals":["ax_opts.chart.events.mounted","ax_opts.dataLabels.formatter","ax_opts.tooltip.y.formatter"],"jsHooks":[]}</script>
</div>
```
:::
:::



### Overige Actoren


::: {.cell}
::: {.cell-output-display}
```{=html}
<style>
  .apex-container {
    max-width: 100%;
    height: auto;
    overflow-x: auto;    /* Horizontal scroll if needed */
    overflow-y: auto;    /* Vertical scroll if needed */
    padding: 20px;
    background-color: #f8f9fa; /* Light background */
    border: 1px solid #ccc;    /* Subtle border */
    border-radius: 10px;       /* Rounded corners */
  }
</style>
<div class="apex-container">
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-082eb37a1ce04f5a49c1" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-082eb37a1ce04f5a49c1">{"x":{"ax_opts":{"chart":{"type":"bar","stacked":true,"events":{"mounted":"\n        function(chart) {\n          setTimeout(function() {\n            chart.toggleSeries('Berichten zonder AI'); // Hides the non-AI series initially\n          }, 500); // Short delay ensures the chart is fully loaded\n        }\n      "},"height":"5000px"},"plotOptions":{"bar":{"horizontal":true,"barHeight":"70%","columnWidth":"85%"}},"xaxis":{"categories":["Pro-PVV","Protest Accounts","Satire"]},"series":[{"name":"Berichten met AI","data":[18.75,10.71428571428571,1.785714285714286]}],"colors":["#6c757d","#17a2b8"],"dataLabels":{"enabled":true,"formatter":"function(val) { return val.toFixed(1) + '%'; }"},"legend":{"position":"top","showForSingleSeries":true,"markers":{"fillColors":["#6c757d","#17a2b8"]},"onItemClick":{"toggleDataSeries":true},"onItemHover":{"highlightDataSeries":true}},"tooltip":{"y":{"formatter":"\n        function(val, opts) { \n          return val.toFixed(2) + '%'; \n        }"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false},"evals":["ax_opts.chart.events.mounted","ax_opts.dataLabels.formatter","ax_opts.tooltip.y.formatter"],"jsHooks":[]}</script>
</div>
```
:::
:::






:::


<br>

Deze grafiek toont het *relatieve* aandeel AI-gegenereerde inhoud per partij. De partijen zijn gesorteerd naar het hoogste aandeel AI-inhoud.

> Let op: bij partijen met minder totale berichten (inclusief kleinere partijen) kan zelfs beperkt AI-gebruik leiden tot hoge relatieve percentages.

<br>



## AI-transparantie


<!-- ::: {.panel-tabset} -->

### Partijen & Politici


::: {.cell}
::: {.cell-output-display}
```{=html}
<style>
  /* kill any theme/Widget white backgrounds */
  .ac-grid > div,
  .ac-grid .html-widget,
  .ac-grid .apexcharts-canvas,
  .ac-grid .apexcharts-svg,
  .ac-grid .apexcharts-inner {
    background: transparent !important;
  }
  /* keep tooltip readable on light pages */
  .apexcharts-tooltip {
    background: rgba(255,255,255,.96) !important;
    color: #111 !important;
  }
</style>
```
:::
:::

::: {.cell}
::: {.cell-output-display}
```{=html}
<style>
  .apex-container {
    max-width: 100%;
    height: auto;
    overflow-x: auto;    /* Horizontal scroll if needed */
    overflow-y: auto;    /* Vertical scroll if needed */
    padding: 20px;
    background-color: #f8f9fa; /* Light background */
    border: 1px solid #ccc;    /* Subtle border */
    border-radius: 10px;       /* Rounded corners */
  }
</style>
<div class="apex-container">
<div style="&#10;    display: flex; &#10;    justify-content: space-between; &#10;    align-items: flex-start; &#10;    gap: 20px;  /* Adds space between boxes */&#10;    padding: 10px;&#10;  ">
<div style="flex: 1; min-width: 300px;">
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-5997db226fc3d3eb9567" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-5997db226fc3d3eb9567">{"x":{"ax_opts":{"chart":{"type":"radialBar","sparkline":{"enabled":true},"height":420,"animations":{"enabled":false},"background":"transparent","foreColor":"#000","redrawOnWindowResize":true,"redrawOnParentResize":true},"series":[82],"labels":["AI ZONDER disclaimer"],"yaxis":{"labels":{"style":{"colors":"#848484"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}}},"colors":["#FF4500"],"plotOptions":{"radialBar":{"hollow":{"size":"58%","margin":4},"track":{"margin":2},"dataLabels":{"name":{"show":true,"style":{"color":"#000","fontSize":"14px","fontWeight":"bold"}},"value":{"show":true,"formatter":"function(val){ return Math.round(val) + '%'; }","style":{"color":"#000","fontSize":"20px","fontWeight":"bold"}}}}},"stroke":{"show":true,"lineCap":"round"},"title":{"text":"Was de AI-inhoud (niet) voorzien van een disclaimer?","align":"center","style":{"fontSize":"18px","color":"#000"}},"theme":{"mode":"light"}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"AI ZONDER disclaimer","max":"AI ZONDER disclaimer"},"type":"radialBar"},"evals":["ax_opts.plotOptions.radialBar.dataLabels.value.formatter"],"jsHooks":[]}</script>
</div>
<div style="flex: 1; min-width: 300px;">
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-ce1ecddcf6d1f1baa7b8" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-ce1ecddcf6d1f1baa7b8">{"x":{"ax_opts":{"chart":{"type":"radialBar","sparkline":{"enabled":true},"height":420},"series":[0,0,100],"labels":["In Beeld","In Text","Door Platform"],"yaxis":{"labels":{"style":{"colors":"#848484"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}}},"colors":["#FF6347","#4682B4","#32CD32"],"plotOptions":{"radialBar":{"hollow":{"size":"48%","margin":4},"track":{"margin":3},"dataLabels":{"name":{"show":true,"style":{"color":"#000","fontSize":"12px","fontWeight":"bold"}},"value":{"show":true,"formatter":"v => Math.round(v) + '%'","style":{"color":"#000","fontSize":"16px"}},"total":{"show":true,"label":"Door Platform","formatter":"\n            function(w){\n              var t = w.globals.seriesTotals;\n              var m = Math.max.apply(null, t);\n              return Math.round(m) + '%';\n            }\n          "}}}},"legend":{"show":false},"stroke":{"show":true,"lineCap":"round"},"title":{"text":"Hoe werd het gebruik van AI kenbaar gemaakt?","align":"center","style":{"fontSize":"18px","color":"#000"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"Door Platform","max":"In Text"},"type":"radialBar"},"evals":["ax_opts.plotOptions.radialBar.dataLabels.value.formatter","ax_opts.plotOptions.radialBar.dataLabels.total.formatter"],"jsHooks":[]}</script>
</div>
</div>
</div>
```
:::
:::




### Overige Actoren



::: {.cell}
::: {.cell-output-display}
```{=html}
<style>
  /* kill any theme/Widget white backgrounds */
  .ac-grid > div,
  .ac-grid .html-widget,
  .ac-grid .apexcharts-canvas,
  .ac-grid .apexcharts-svg,
  .ac-grid .apexcharts-inner {
    background: transparent !important;
  }
  /* keep tooltip readable on light pages */
  .apexcharts-tooltip {
    background: rgba(255,255,255,.96) !important;
    color: #111 !important;
  }
</style>
```
:::
:::

::: {.cell}
::: {.cell-output-display}
```{=html}
<style>
  .apex-container {
    max-width: 100%;
    height: auto;
    overflow-x: auto;    /* Horizontal scroll if needed */
    overflow-y: auto;    /* Vertical scroll if needed */
    padding: 20px;
    background-color: #f8f9fa; /* Light background */
    border: 1px solid #ccc;    /* Subtle border */
    border-radius: 10px;       /* Rounded corners */
  }
</style>
<div class="apex-container">
<div style="&#10;    display: flex; &#10;    justify-content: space-between; &#10;    align-items: flex-start; &#10;    gap: 20px;  /* Adds space between boxes */&#10;    padding: 10px;&#10;  ">
<div style="flex: 1; min-width: 300px;">
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-63c4af236238dfd28091" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-63c4af236238dfd28091">{"x":{"ax_opts":{"chart":{"type":"radialBar","sparkline":{"enabled":true},"height":420,"animations":{"enabled":false},"background":"transparent","foreColor":"#000","redrawOnWindowResize":true,"redrawOnParentResize":true},"series":[38],"labels":["AI ZONDER disclaimer"],"yaxis":{"labels":{"style":{"colors":"#848484"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}}},"colors":["#FF4500"],"plotOptions":{"radialBar":{"hollow":{"size":"58%","margin":4},"track":{"margin":2},"dataLabels":{"name":{"show":true,"style":{"color":"#000","fontSize":"14px","fontWeight":"bold"}},"value":{"show":true,"formatter":"function(val){ return Math.round(val) + '%'; }","style":{"color":"#000","fontSize":"20px","fontWeight":"bold"}}}}},"stroke":{"show":true,"lineCap":"round"},"title":{"text":"Was de AI-inhoud (niet) voorzien van een disclaimer?","align":"center","style":{"fontSize":"18px","color":"#000"}},"theme":{"mode":"light"}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"AI ZONDER disclaimer","max":"AI ZONDER disclaimer"},"type":"radialBar"},"evals":["ax_opts.plotOptions.radialBar.dataLabels.value.formatter"],"jsHooks":[]}</script>
</div>
<div style="flex: 1; min-width: 300px;">
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-4d1f28c38d75fd34ec80" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-4d1f28c38d75fd34ec80">{"x":{"ax_opts":{"chart":{"type":"radialBar","sparkline":{"enabled":true},"height":420},"series":[0,0,100],"labels":["In Beeld","In Text","Door Platform"],"yaxis":{"labels":{"style":{"colors":"#848484"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}}},"colors":["#FF6347","#4682B4","#32CD32"],"plotOptions":{"radialBar":{"hollow":{"size":"48%","margin":4},"track":{"margin":3},"dataLabels":{"name":{"show":true,"style":{"color":"#000","fontSize":"12px","fontWeight":"bold"}},"value":{"show":true,"formatter":"v => Math.round(v) + '%'","style":{"color":"#000","fontSize":"16px"}},"total":{"show":true,"label":"Door Platform","formatter":"\n            function(w){\n              var t = w.globals.seriesTotals;\n              var m = Math.max.apply(null, t);\n              return Math.round(m) + '%';\n            }\n          "}}}},"legend":{"show":false},"stroke":{"show":true,"lineCap":"round"},"title":{"text":"Hoe werd het gebruik van AI kenbaar gemaakt?","align":"center","style":{"fontSize":"18px","color":"#000"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"Door Platform","max":"In Text"},"type":"radialBar"},"evals":["ax_opts.plotOptions.radialBar.dataLabels.value.formatter","ax_opts.plotOptions.radialBar.dataLabels.total.formatter"],"jsHooks":[]}</script>
</div>
</div>
</div>
```
:::
:::


<!-- ::: -->


<br>


Openbaarmaking van AI-inhoud via disclaimers van partijen of platformlabels is cruciaal voor transparantie. Deze visualisatie toont hoe vaak AI-gegenereerde inhoud werd gepubliceerd met/zonder disclosure en of het label door de partij of door Meta werd toegevoegd. 

<br>




## AI-mediavormen {#medienformatte}

::: {.panel-tabset}

### Partijen & Politici


::: {.cell}

:::

::: {.cell}
::: {.cell-output-display}
```{=html}
<style>
  .apex-container {
    max-width: 100%;
    height: auto;
    overflow-x: auto;    /* Horizontal scroll if needed */
    overflow-y: auto;    /* Vertical scroll if needed */
    padding: 20px;
    background-color: #f8f9fa; /* Light background */
    border: 1px solid #ccc;    /* Subtle border */
    border-radius: 10px;       /* Rounded corners */
  }
</style>
<div class="apex-container">
<div style="&#10;    display: flex; &#10;    justify-content: space-between; &#10;    align-items: flex-start; &#10;    gap: 20px;  /* Adds space between boxes */&#10;    padding: 10px;&#10;  ">
<div style="flex: 1; min-width: 300px;">
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-42783640afa300689474" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-42783640afa300689474">{"x":{"ax_opts":{"chart":{"type":"radialBar","sparkline":{"enabled":true},"height":420,"animations":{"enabled":false},"background":"transparent","foreColor":"#000","redrawOnWindowResize":true,"redrawOnParentResize":true},"series":[38],"labels":["AI ZONDER disclaimer"],"yaxis":{"labels":{"style":{"colors":"#848484"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}}},"colors":["#FF4500"],"plotOptions":{"radialBar":{"hollow":{"size":"58%","margin":4},"track":{"margin":2},"dataLabels":{"name":{"show":true,"style":{"color":"#000","fontSize":"14px","fontWeight":"bold"}},"value":{"show":true,"formatter":"function(val){ return Math.round(val) + '%'; }","style":{"color":"#000","fontSize":"20px","fontWeight":"bold"}}}}},"stroke":{"show":true,"lineCap":"round"},"title":{"text":"Was de AI-inhoud (niet) voorzien van een disclaimer?","align":"center","style":{"fontSize":"18px","color":"#000"}},"theme":{"mode":"light"}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"AI ZONDER disclaimer","max":"AI ZONDER disclaimer"},"type":"radialBar"},"evals":["ax_opts.plotOptions.radialBar.dataLabels.value.formatter"],"jsHooks":[]}</script>
</div>
<div style="flex: 1; min-width: 300px;">
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-c32a1c6299e756133fd8" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-c32a1c6299e756133fd8">{"x":{"ax_opts":{"chart":{"type":"radialBar","sparkline":{"enabled":true},"height":420},"series":[0,0,100],"labels":["In Beeld","In Text","Door Platform"],"yaxis":{"labels":{"style":{"colors":"#848484"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}}},"colors":["#FF6347","#4682B4","#32CD32"],"plotOptions":{"radialBar":{"hollow":{"size":"48%","margin":4},"track":{"margin":3},"dataLabels":{"name":{"show":true,"style":{"color":"#000","fontSize":"12px","fontWeight":"bold"}},"value":{"show":true,"formatter":"v => Math.round(v) + '%'","style":{"color":"#000","fontSize":"16px"}},"total":{"show":true,"label":"Door Platform","formatter":"\n            function(w){\n              var t = w.globals.seriesTotals;\n              var m = Math.max.apply(null, t);\n              return Math.round(m) + '%';\n            }\n          "}}}},"legend":{"show":false},"stroke":{"show":true,"lineCap":"round"},"title":{"text":"Hoe werd het gebruik van AI kenbaar gemaakt?","align":"center","style":{"fontSize":"18px","color":"#000"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"Door Platform","max":"In Text"},"type":"radialBar"},"evals":["ax_opts.plotOptions.radialBar.dataLabels.value.formatter","ax_opts.plotOptions.radialBar.dataLabels.total.formatter"],"jsHooks":[]}</script>
</div>
</div>
</div>
```
:::
:::



### Overige Actoren



::: {.cell}
::: {.cell-output-display}
```{=html}
<style>
  .apex-container {
    max-width: 100%;
    height: auto;
    overflow-x: auto;    /* Horizontal scroll if needed */
    overflow-y: auto;    /* Vertical scroll if needed */
    padding: 20px;
    background-color: #f8f9fa; /* Light background */
    border: 1px solid #ccc;    /* Subtle border */
    border-radius: 10px;       /* Rounded corners */
  }
</style>
<div class="apex-container">
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-a4e96f80ef7612332ff7" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-a4e96f80ef7612332ff7">{"x":{"ax_opts":{"chart":{"type":"donut","height":299},"series":[9,4],"labels":["Afbeelding(en)","Video(’s)"],"yaxis":{"labels":{"style":{"colors":"#848484"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}}},"colors":["#FF6347","#4682B4","#32CD32"],"plotOptions":{"radialBar":{"hollow":{"size":"60%"},"dataLabels":{"name":{"show":true,"style":{"color":"#000","fontSize":"16px","fontWeight":"bold"}},"value":{"show":true,"formatter":"function(val) { return val + '%'; }","style":{"color":"#000","fontSize":"20px","fontWeight":"bold"}}}}},"fill":{"type":"solid"},"stroke":{"show":true,"lineCap":"round"}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"Afbeelding(en)","max":"Video(’s)"},"type":"donut"},"evals":["ax_opts.plotOptions.radialBar.dataLabels.value.formatter"],"jsHooks":[]}</script>
</div>
```
:::
:::




:::


<br>

Deze grafiek toont het percentage afbeeldingen en video’s in berichten die als AI-gegenereerd zijn geïdentificeerd. Dit helpt te laten zien welke mediavormen vaker met AI worden ingezet.

<br>


## AI-inhoudsanalyse

::: {.panel-tabset}

### Partijen & Politici



::: {.cell}
::: {.cell-output-display}
```{=html}
<style>
  .apex-container {
    max-width: 100%;
    height: auto;
    overflow-x: auto;    /* Horizontal scroll if needed */
    overflow-y: auto;    /* Vertical scroll if needed */
    padding: 20px;
    background-color: #f8f9fa; /* Light background */
    border: 1px solid #ccc;    /* Subtle border */
    border-radius: 10px;       /* Rounded corners */
  }
</style>
<div class="apex-container">
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-ca9b8b9146d58ec39a09" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-ca9b8b9146d58ec39a09">{"x":{"ax_opts":{"chart":{"type":"bar"},"series":[{"name":"n","data":[{"x":"Positief","y":51},{"x":"Negatief","y":30}]}],"dataLabels":{"enabled":true,"formatter":"function(val) { return val + ' Berichten'; }"},"plotOptions":{"bar":{"horizontal":true,"isDumbbell":false,"barHeight":"60%","borderRadius":5,"distributed":true}},"tooltip":{"shared":true,"intersect":false,"followCursor":true,"y":{"formatter":"function(val) { return val + ' Berichten'; }"}},"grid":{"yaxis":{"lines":{"show":false}},"xaxis":{"lines":{"show":true}}},"yaxis":{"labels":{"style":{"colors":"#848484","fontSize":"14px","fontWeight":"bold"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}},"title":{"text":"Aantal berichten"}},"colors":["#4CAF50","#F44336","#9E9E9E"],"title":{"text":"Verdeling van toon in AI-gegenereerde inhoud","align":"center","style":{"fontSize":"18px","fontWeight":"bold"}},"legend":{"position":"bottom","labels":{"colors":"#000"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"Negatief","max":"Positief"},"type":"bar"},"evals":["ax_opts.dataLabels.formatter","ax_opts.tooltip.y.formatter"],"jsHooks":[]}</script>
</div>
```
:::
:::



### Overige Actoren



::: {.cell}
::: {.cell-output-display}
```{=html}
<style>
  .apex-container {
    max-width: 100%;
    height: auto;
    overflow-x: auto;    /* Horizontal scroll if needed */
    overflow-y: auto;    /* Vertical scroll if needed */
    padding: 20px;
    background-color: #f8f9fa; /* Light background */
    border: 1px solid #ccc;    /* Subtle border */
    border-radius: 10px;       /* Rounded corners */
  }
</style>
<div class="apex-container">
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-31d6c15d0ee9e4863057" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-31d6c15d0ee9e4863057">{"x":{"ax_opts":{"chart":{"type":"bar"},"series":[{"name":"n","data":[{"x":"Positief","y":11},{"x":"Negatief","y":10}]}],"dataLabels":{"enabled":true,"formatter":"function(val) { return val + ' Berichten'; }"},"plotOptions":{"bar":{"horizontal":true,"isDumbbell":false,"barHeight":"60%","borderRadius":5,"distributed":true}},"tooltip":{"shared":true,"intersect":false,"followCursor":true,"y":{"formatter":"function(val) { return val + ' Berichten'; }"}},"grid":{"yaxis":{"lines":{"show":false}},"xaxis":{"lines":{"show":true}}},"yaxis":{"labels":{"style":{"colors":"#848484","fontSize":"14px","fontWeight":"bold"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}},"title":{"text":"Aantal berichten"}},"colors":["#4CAF50","#F44336","#9E9E9E"],"title":{"text":"Verdeling van toon in AI-gegenereerde inhoud","align":"center","style":{"fontSize":"18px","fontWeight":"bold"}},"legend":{"position":"bottom","labels":{"colors":"#000"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"Negatief","max":"Positief"},"type":"bar"},"evals":["ax_opts.dataLabels.formatter","ax_opts.tooltip.y.formatter"],"jsHooks":[]}</script>
</div>
```
:::
:::



:::


<br>

>  Let op: het is mogelijk dat een bericht zowel negatieve als positieve inhoud bevat.

<br>


::: {.panel-tabset}


### Partijen & Politici


::: {.cell}
::: {.cell-output-display}
```{=html}
<style>
  .apex-container {
    max-width: 100%;
    height: auto;
    overflow-x: auto;    /* Horizontal scroll if needed */
    overflow-y: auto;    /* Vertical scroll if needed */
    padding: 20px;
    background-color: #f8f9fa; /* Light background */
    border: 1px solid #ccc;    /* Subtle border */
    border-radius: 10px;       /* Rounded corners */
  }
</style>
<div class="apex-container">
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-402d758fa7af9b651dc5" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-402d758fa7af9b651dc5">{"x":{"ax_opts":{"chart":{"type":"bar","stacked":false,"height":800,"horizontal":true},"series":[{"name":"n","data":[{"x":"Politieke partijen & politici","y":25},{"x":"Stemappèl","y":23},{"x":"Binnenlands & Migratiebeleid","y":18},{"x":"Verkiezingen (algemeen)","y":14},{"x":"Arbeid & Sociale Zaken","y":12},{"x":"Economie & Financiën","y":11},{"x":"Digitaal & Infrastructuur","y":8},{"x":"Defensiebeleid","y":7},{"x":"Energiebeleid","y":7},{"x":"Wooncrisis","y":6},{"x":"Onderwijs & Cultuur","y":5},{"x":"Grondrechten","y":3},{"x":"Overige politieke thema’s","y":2},{"x":"Europa","y":1}]}],"dataLabels":{"enabled":true,"formatter":"function(val) { return val + ' Berichten'; }"},"plotOptions":{"bar":{"horizontal":true,"isDumbbell":false,"barHeight":"60%","borderRadius":5}},"tooltip":{"shared":true,"intersect":false,"followCursor":true,"y":{"formatter":"function(val) { return val + ' Berichten'; }"}},"grid":{"yaxis":{"lines":{"show":false}},"xaxis":{"lines":{"show":true}}},"yaxis":{"labels":{"style":{"colors":"#848484","fontSize":"14px","fontWeight":"bold"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}},"title":{"text":"Aantal berichten"}},"title":{"text":"Verdeling van thema’s in AI-gegenereerde inhoud","align":"center","style":{"fontSize":"18px","fontWeight":"bold"}},"legend":{"position":"bottom","labels":{"colors":"#000"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"type":"bar"},"evals":["ax_opts.dataLabels.formatter","ax_opts.tooltip.y.formatter"],"jsHooks":[]}</script>
</div>
```
:::
:::



### Overige Actoren





::: {.cell}
::: {.cell-output-display}
```{=html}
<style>
  .apex-container {
    max-width: 100%;
    height: auto;
    overflow-x: auto;    /* Horizontal scroll if needed */
    overflow-y: auto;    /* Vertical scroll if needed */
    padding: 20px;
    background-color: #f8f9fa; /* Light background */
    border: 1px solid #ccc;    /* Subtle border */
    border-radius: 10px;       /* Rounded corners */
  }
</style>
<div class="apex-container">
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-cfe7d56fe8a6cad0e94a" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-cfe7d56fe8a6cad0e94a">{"x":{"ax_opts":{"chart":{"type":"bar","stacked":false,"height":800,"horizontal":true},"series":[{"name":"n","data":[{"x":"Binnenlands & Migratiebeleid","y":11},{"x":"Stemappèl","y":8},{"x":"Politieke partijen & politici","y":4},{"x":"Overige politieke thema’s","y":2},{"x":"Wooncrisis","y":2},{"x":"Arbeid & Sociale Zaken","y":1},{"x":"Economie & Financiën","y":1},{"x":"Energiebeleid","y":1},{"x":"Europa","y":1},{"x":"Grondrechten","y":1}]}],"dataLabels":{"enabled":true,"formatter":"function(val) { return val + ' Berichten'; }"},"plotOptions":{"bar":{"horizontal":true,"isDumbbell":false,"barHeight":"60%","borderRadius":5}},"tooltip":{"shared":true,"intersect":false,"followCursor":true,"y":{"formatter":"function(val) { return val + ' Berichten'; }"}},"grid":{"yaxis":{"lines":{"show":false}},"xaxis":{"lines":{"show":true}}},"yaxis":{"labels":{"style":{"colors":"#848484","fontSize":"14px","fontWeight":"bold"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}},"title":{"text":"Aantal berichten"}},"title":{"text":"Verdeling van thema’s in AI-gegenereerde inhoud","align":"center","style":{"fontSize":"18px","fontWeight":"bold"}},"legend":{"position":"bottom","labels":{"colors":"#000"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"type":"bar"},"evals":["ax_opts.dataLabels.formatter","ax_opts.tooltip.y.formatter"],"jsHooks":[]}</script>
</div>
```
:::
:::





:::



<br>

> Let op: een enkel bericht kan meerdere thema’s behandelen.


<br>


::: {.panel-tabset}


### Partijen & Politici


::: {.cell}
::: {.cell-output-display}
```{=html}
<style>
  .apex-container {
    max-width: 100%;
    height: auto;
    overflow-x: auto;    /* Horizontal scroll if needed */
    overflow-y: auto;    /* Vertical scroll if needed */
    padding: 20px;
    background-color: #f8f9fa; /* Light background */
    border: 1px solid #ccc;    /* Subtle border */
    border-radius: 10px;       /* Rounded corners */
  }
</style>
<div class="apex-container">
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-9cb658bffa07e48dcae4" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-9cb658bffa07e48dcae4">{"x":{"ax_opts":{"chart":{"type":"bar","stacked":false,"height":800,"horizontal":true},"series":[{"name":"n","data":[{"x":"Positieve beeldvorming / lof","y":37},{"x":"Symbolische afbeelding (frontaal afgebeelde mensen)","y":35},{"x":"Politieke positionering","y":34},{"x":"Negatieve beeldvorming / campagnes","y":18},{"x":"Evenementaankondiging / verkiezingsappèl / kandidatenintroductie","y":16},{"x":"Humor / Satire","y":4},{"x":"Dagelijkse politiek","y":2},{"x":"Mediaverkeer (incl. tv-debatten)","y":2},{"x":"Nostalgisch / Historisch","y":2},{"x":"Campagne-evenementen","y":1},{"x":"Overige beeldinhoud","y":1}]}],"dataLabels":{"enabled":true,"formatter":"function(val) { return val + ' Berichten'; }"},"plotOptions":{"bar":{"horizontal":true,"isDumbbell":false,"barHeight":"60%","borderRadius":5}},"tooltip":{"shared":true,"intersect":false,"followCursor":true,"y":{"formatter":"function(val) { return val + ' Berichten'; }"}},"grid":{"yaxis":{"lines":{"show":false}},"xaxis":{"lines":{"show":true}}},"yaxis":{"labels":{"style":{"colors":"#848484","fontSize":"14px","fontWeight":"bold"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}},"title":{"text":"Aantal berichten"}},"title":{"text":"Verdeling van beeld-/video-inhoud in AI-gegenereerde inhoud","align":"center","style":{"fontSize":"18px","fontWeight":"bold"}},"legend":{"position":"bottom","labels":{"colors":"#000"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"type":"bar"},"evals":["ax_opts.dataLabels.formatter","ax_opts.tooltip.y.formatter"],"jsHooks":[]}</script>
</div>
```
:::
:::




### Overige Actoren



::: {.cell}
::: {.cell-output-display}
```{=html}
<style>
  .apex-container {
    max-width: 100%;
    height: auto;
    overflow-x: auto;    /* Horizontal scroll if needed */
    overflow-y: auto;    /* Vertical scroll if needed */
    padding: 20px;
    background-color: #f8f9fa; /* Light background */
    border: 1px solid #ccc;    /* Subtle border */
    border-radius: 10px;       /* Rounded corners */
  }
</style>
<div class="apex-container">
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-f894112403acf14173d5" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-f894112403acf14173d5">{"x":{"ax_opts":{"chart":{"type":"bar","stacked":false,"height":800,"horizontal":true},"series":[{"name":"n","data":[{"x":"Symbolische afbeelding (frontaal afgebeelde mensen)","y":9},{"x":"Positieve beeldvorming / lof","y":8},{"x":"Politieke positionering","y":7},{"x":"Negatieve beeldvorming / campagnes","y":6},{"x":"Evenementaankondiging / verkiezingsappèl / kandidatenintroductie","y":4},{"x":"Humor / Satire","y":1},{"x":"Overige beeldinhoud","y":1},{"x":"Utopia or Dystopia","y":1}]}],"dataLabels":{"enabled":true,"formatter":"function(val) { return val + ' Berichten'; }"},"plotOptions":{"bar":{"horizontal":true,"isDumbbell":false,"barHeight":"60%","borderRadius":5}},"tooltip":{"shared":true,"intersect":false,"followCursor":true,"y":{"formatter":"function(val) { return val + ' Berichten'; }"}},"grid":{"yaxis":{"lines":{"show":false}},"xaxis":{"lines":{"show":true}}},"yaxis":{"labels":{"style":{"colors":"#848484","fontSize":"14px","fontWeight":"bold"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}},"title":{"text":"Aantal berichten"}},"title":{"text":"Verdeling van beeld-/video-inhoud in AI-gegenereerde inhoud","align":"center","style":{"fontSize":"18px","fontWeight":"bold"}},"legend":{"position":"bottom","labels":{"colors":"#000"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"type":"bar"},"evals":["ax_opts.dataLabels.formatter","ax_opts.tooltip.y.formatter"],"jsHooks":[]}</script>
</div>
```
:::
:::



:::

<br>

> Let op: een enkele afbeelding kan meerdere beeld-/videothema’s bevatten.

<br>





## Afgebeelde personen in AI-inhoud {#personen}

::: {.panel-tabset}

### Partijen & Politici


::: {.cell}
::: {.cell-output-display}
```{=html}
<style>
  .apex-container {
    max-width: 100%;
    height: auto;
    overflow-x: auto;    /* Horizontal scroll if needed */
    overflow-y: auto;    /* Vertical scroll if needed */
    padding: 20px;
    background-color: #f8f9fa; /* Light background */
    border: 1px solid #ccc;    /* Subtle border */
    border-radius: 10px;       /* Rounded corners */
  }
</style>
<div class="apex-container">
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-1d2f98cc5c35e9daa43d" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-1d2f98cc5c35e9daa43d">{"x":{"ax_opts":{"chart":{"type":"treemap"},"series":[{"name":[],"data":[{"x":"Vertegenwoordigers van sociale bewegingen","y":1},{"x":"GL-PvdA: Frans Timmermans","y":2},{"x":"Niet-politieke vertegenwoordigers van instituties","y":2},{"x":"PVV: Geert Wilders","y":3},{"x":"Illegale/criminelen/extremisten","y":4},{"x":"Minderheden","y":9},{"x":"Gewone mensen","y":37}]}],"yaxis":{"labels":{"style":{"colors":"#848484","fontSize":"14px","fontWeight":"bold"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}},"title":{"text":"Aantal berichten"}},"colors":["#547D01"],"dataLabels":{"style":{"colors":["#000000"]}},"title":{"text":"Verdeling van personen in AI-gegenereerde inhoud","align":"center","style":{"fontSize":"18px","fontWeight":"bold"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"Gewone mensen","max":"Vertegenwoordigers van sociale bewegingen"},"type":"treemap"},"evals":[],"jsHooks":[]}</script>
</div>
```
:::
:::




### Overige Actoren




::: {.cell}
::: {.cell-output-display}
```{=html}
<style>
  .apex-container {
    max-width: 100%;
    height: auto;
    overflow-x: auto;    /* Horizontal scroll if needed */
    overflow-y: auto;    /* Vertical scroll if needed */
    padding: 20px;
    background-color: #f8f9fa; /* Light background */
    border: 1px solid #ccc;    /* Subtle border */
    border-radius: 10px;       /* Rounded corners */
  }
</style>
<div class="apex-container">
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-5b0573d02fe661ef4636" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-5b0573d02fe661ef4636">{"x":{"ax_opts":{"chart":{"type":"treemap"},"series":[{"name":[],"data":[{"x":"BBB: Caroline van der Plas","y":1},{"x":"CDA: Henri Bontenbal","y":1},{"x":"D66: Rob Jetten","y":1},{"x":"GL-PvdA: Frans Timmermans","y":1},{"x":"GL-PvdA: Jesse Klaver","y":1},{"x":"PVV: Geert Wilders","y":1},{"x":"Vertegenwoordigers van sociale bewegingen","y":1},{"x":"VVD: Dilan Yeşilgöz","y":1},{"x":"Illegale/criminelen/extremisten","y":2},{"x":"Niet-politieke vertegenwoordigers van instituties","y":2},{"x":"Minderheden","y":3},{"x":"Gewone mensen","y":8}]}],"yaxis":{"labels":{"style":{"colors":"#848484","fontSize":"14px","fontWeight":"bold"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}},"title":{"text":"Aantal berichten"}},"colors":["#547D01"],"dataLabels":{"style":{"colors":["#000000"]}},"title":{"text":"Verdeling van personen in AI-gegenereerde inhoud","align":"center","style":{"fontSize":"18px","fontWeight":"bold"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"BBB: Caroline van der Plas","max":"VVD: Dilan Yeşilgöz"},"type":"treemap"},"evals":[],"jsHooks":[]}</script>
</div>
```
:::
:::




:::

<br>

Deze visualisatie toont welke persoon(groepen) in hoeveel van de AI-gegenereerde afbeeldingen/video’s worden afgebeeld.

> Let op: een enkele afbeelding kan meerdere personen bevatten.


<br>



## AI-inhoud door de tijd heen {#ai-over-time}


::: {.cell}
::: {.cell-output-display}
```{=html}
<style>
  .apex-container {
    max-width: 100%;
    height: auto;
    overflow-x: auto;    /* Horizontal scroll if needed */
    overflow-y: auto;    /* Vertical scroll if needed */
    padding: 20px;
    background-color: #f8f9fa; /* Light background */
    border: 1px solid #ccc;    /* Subtle border */
    border-radius: 10px;       /* Rounded corners */
  }
</style>
<div class="apex-container">
<div class="highchart html-widget html-fill-item" id="htmlwidget-625b498fb11299c14fd9" style="width:100%;height:500px;"></div>
<script type="application/json" data-for="htmlwidget-625b498fb11299c14fd9">{"x":{"hc_opts":{"chart":{"reflow":true,"type":"line"},"title":{"text":"AI-berichten door de tijd heen"},"yAxis":{"title":{"text":"Aantal berichten"}},"credits":{"enabled":false},"exporting":{"enabled":false},"boost":{"enabled":false},"plotOptions":{"series":{"label":{"enabled":false},"turboThreshold":0},"treemap":{"layoutAlgorithm":"squarified"}},"xAxis":{"categories":["2025-09-17","2025-09-18","2025-09-19","2025-09-20","2025-09-21","2025-09-22","2025-09-23","2025-09-24","2025-09-25"]},"series":[{"data":[5,10,5,9,8,9,10,5,9],"name":"Berichten met AI","color":"#FF6F61"},{"data":[792,764,670,629,513,681,758,740,827],"name":"Berichten zonder AI","color":"#6B5B95"}],"tooltip":{"pointFormat":"<b>{series.name}<\/b>: {point.y}"}},"theme":{"chart":{"backgroundColor":"transparent"},"colors":["#7cb5ec","#434348","#90ed7d","#f7a35c","#8085e9","#f15c80","#e4d354","#2b908f","#f45b5b","#91e8e1"]},"conf_opts":{"global":{"Date":null,"VMLRadialGradientURL":"http =//code.highcharts.com/list(version)/gfx/vml-radial-gradient.png","canvasToolsURL":"http =//code.highcharts.com/list(version)/modules/canvas-tools.js","getTimezoneOffset":null,"timezoneOffset":0,"useUTC":true},"lang":{"contextButtonTitle":"Chart context menu","decimalPoint":".","downloadCSV":"Download CSV","downloadJPEG":"Download JPEG image","downloadPDF":"Download PDF document","downloadPNG":"Download PNG image","downloadSVG":"Download SVG vector image","downloadXLS":"Download XLS","drillUpText":"◁ Back to {series.name}","exitFullscreen":"Exit from full screen","exportData":{"annotationHeader":"Annotations","categoryDatetimeHeader":"DateTime","categoryHeader":"Category"},"hideData":"Hide data table","invalidDate":null,"loading":"Loading...","months":["January","February","March","April","May","June","July","August","September","October","November","December"],"noData":"No data to display","numericSymbolMagnitude":1000,"numericSymbols":["k","M","G","T","P","E"],"printChart":"Print chart","resetZoom":"Reset zoom","resetZoomTitle":"Reset zoom level 1:1","shortMonths":["Jan","Feb","Mar","Apr","May","Jun","Jul","Aug","Sep","Oct","Nov","Dec"],"shortWeekdays":["Sat","Sun","Mon","Tue","Wed","Thu","Fri"],"thousandsSep":" ","viewData":"View data table","viewFullscreen":"View in full screen","weekdays":["Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday"]}},"type":"chart","fonts":[],"debug":false},"evals":[],"jsHooks":[]}</script>
</div>
```
:::
:::


<br>

Deze grafiek toont het gebruik van AI versus niet-AI-inhoud door de tijd heen.

<br>

<br>
<center>
  <a href="https://favstats.github.io/campaigntrackernl">
    <img src="logobelow.png" width="50%">
  </a>
</center>


