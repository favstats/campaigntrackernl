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
<div id="htmlwidget-107cbd9663283337d9c6" style="width:100%;height:160px;" class="apexcharter html-widget"></div>
<script type="application/json" data-for="htmlwidget-107cbd9663283337d9c6">{"x":{"ax_opts":{"chart":{"type":"area","sparkline":{"enabled":true}},"series":[{"name":"n","type":"area","data":[[1758067200000,810],[1758153600000,794],[1758240000000,685],[1758326400000,645],[1758412800000,525],[1758499200000,712],[1758585600000,799],[1758672000000,764],[1758758400000,846]]}],"dataLabels":{"enabled":false},"stroke":{"curve":"straight","width":2},"yaxis":{"decimalsInFloat":2,"labels":{"style":{"colors":"#848484"}},"show":false},"xaxis":{"type":"datetime","labels":{"style":{"colors":"#848484"}}},"colors":["#2E93fA"],"title":{"text":6580,"style":{"fontSize":"24px"}},"subtitle":{"text":"Totaal aantal gevolgde berichten","style":{"fontSize":"14px"}}},"auto_update":{"series_animate":true,"update_options":true,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":{"color":"#2E93fA","background":"#FFF"},"xaxis":{"min":"2025-09-17T00:00:00Z","max":"2025-09-25T00:00:00Z"},"type":"area"},"evals":[],"jsHooks":[]}</script>
</div>
<div style="flex: 1; min-width: 300px;">
<div id="htmlwidget-9e8563966b8dfc03f430" style="width:100%;height:160px;" class="apexcharter html-widget"></div>
<script type="application/json" data-for="htmlwidget-9e8563966b8dfc03f430">{"x":{"ax_opts":{"chart":{"type":"area","sparkline":{"enabled":true}},"series":[{"name":"n","type":"area","data":[[1758067200000,7],[1758153600000,22],[1758240000000,21],[1758326400000,23],[1758412800000,18],[1758499200000,19],[1758585600000,20],[1758672000000,14],[1758758400000,22]]}],"dataLabels":{"enabled":false},"stroke":{"curve":"straight","width":2},"yaxis":{"decimalsInFloat":2,"labels":{"style":{"colors":"#848484"}},"show":false},"xaxis":{"type":"datetime","labels":{"style":{"colors":"#848484"}}},"colors":["#FFF"],"title":{"text":166,"style":{"fontSize":"22px","color":"#FFF"}},"subtitle":{"text":"Totaal aantal geïdentificeerde AI-berichten","style":{"fontSize":"14px","color":"#FFF"}}},"auto_update":{"series_animate":true,"update_options":true,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":{"color":"#FFF","background":"#1E90FF"},"xaxis":{"min":"2025-09-17T00:00:00Z","max":"2025-09-25T00:00:00Z"},"type":"area"},"evals":[],"jsHooks":[]}</script>
</div>
</div>
```
:::
:::

::: {.cell}

:::


<br>

#  Overzicht van Inhoud

Hier laten we zien hoeveel AI-inhoud we hebben gevonden, onderverdeeld in **platform**, **actortype** en **politieke voorkeur**.

We onderscheiden **partijen en politici** van **andere actoren**, zoals commentatoren, influencers, fanpagina's en meme-pagina's.

::: {.panel-tabset}


## Per Partij / Actor {#ki-content-by-party2}


::: {.cell}

:::




::: {.panel-tabset}

### All


::: {.cell}
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
<div id="htmlwidget-26750cce3625da17a294" style="width:100%;height:400px;" class="apexcharter html-widget"></div>
<script type="application/json" data-for="htmlwidget-26750cce3625da17a294">{"x":{"ax_opts":{"chart":{"type":"treemap","toolbar":{"show":false}},"series":[{"name":"y","data":[{"x":"PVV","y":46},{"x":"Pro-Right","y":30},{"x":"Satire","y":18},{"x":"Pro-PVV","y":16},{"x":"VVD","y":11},{"x":"Pro-FvD","y":7},{"x":"GL-PvdA","y":6},{"x":"BBB","y":5},{"x":"50PLUS","y":3},{"x":"De Linie","y":3},{"x":"FvD","y":3},{"x":"NCPN","y":3},{"x":"SP","y":3},{"x":"DENK","y":2},{"x":"SGP","y":2},{"x":"Unspecified/Other","y":2},{"x":"BVNL","y":1},{"x":"CU","y":1},{"x":"D66","y":1},{"x":"JA21","y":1},{"x":"LP","y":1},{"x":"Vrede voor Dieren","y":1}]}],"yaxis":{"labels":{"style":{"colors":"#848484"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}}},"title":{"text":"Per Partij / Actor","align":"center","style":{"fontSize":"16px"}},"legend":{"show":false},"colors":["#003082","#8C6D1F","#6A5ACD","#B22222","#FF7900","#7E2342","#C00040","#009639","#7F2481","#AA3377","#7B1E26","#CC0000","#BE1E2D","#00A7B3","#E57200","#CCCCCC","#132141","#00A1DE","#009E60","#0C2E6E","#003399","#5496c6"],"plotOptions":{"treemap":{"distributed":true,"enableShades":false,"dataLabels":{"enabled":true,"style":{"fontSize":"12px"}}}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"50PLUS","max":"VVD"},"type":"treemap"},"evals":[],"jsHooks":[]}</script>
</div>
```
:::
:::


### Parties


::: {.cell}
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
<div id="htmlwidget-2760d2fe0bee81352f3a" style="width:100%;height:400px;" class="apexcharter html-widget"></div>
<script type="application/json" data-for="htmlwidget-2760d2fe0bee81352f3a">{"x":{"ax_opts":{"chart":{"type":"treemap","toolbar":{"show":false}},"series":[{"name":"y","data":[{"x":"PVV","y":46},{"x":"VVD","y":11},{"x":"GL-PvdA","y":6},{"x":"BBB","y":5},{"x":"50PLUS","y":3},{"x":"De Linie","y":3},{"x":"FvD","y":3},{"x":"NCPN","y":3},{"x":"SP","y":3},{"x":"DENK","y":2},{"x":"SGP","y":2},{"x":"BVNL","y":1},{"x":"CU","y":1},{"x":"D66","y":1},{"x":"JA21","y":1},{"x":"LP","y":1},{"x":"Vrede voor Dieren","y":1}]}],"yaxis":{"labels":{"style":{"colors":"#848484"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}}},"title":{"text":"Per Partij / Actor","align":"center","style":{"fontSize":"16px"}},"legend":{"show":false},"colors":["#003082","#FF7900","#C00040","#009639","#7F2481","#AA3377","#7B1E26","#CC0000","#BE1E2D","#00A7B3","#E57200","#132141","#00A1DE","#009E60","#0C2E6E","#003399","#5496c6"],"plotOptions":{"treemap":{"distributed":true,"enableShades":false,"dataLabels":{"enabled":true,"style":{"fontSize":"12px"}}}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"50PLUS","max":"VVD"},"type":"treemap"},"evals":[],"jsHooks":[]}</script>
</div>
```
:::
:::


### Other Actors


::: {.cell}
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
<div id="htmlwidget-aab47212c6c4bd9637ff" style="width:100%;height:400px;" class="apexcharter html-widget"></div>
<script type="application/json" data-for="htmlwidget-aab47212c6c4bd9637ff">{"x":{"ax_opts":{"chart":{"type":"treemap","toolbar":{"show":false}},"series":[{"name":"y","data":[{"x":"Pro-Right","y":30},{"x":"Satire","y":18},{"x":"Pro-PVV","y":16},{"x":"Pro-FvD","y":7},{"x":"Unspecified/Other","y":2}]}],"yaxis":{"labels":{"style":{"colors":"#848484"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}}},"title":{"text":"Per Partij / Actor","align":"center","style":{"fontSize":"16px"}},"legend":{"show":false},"colors":["#8C6D1F","#6A5ACD","#B22222","#7E2342","#CCCCCC"],"plotOptions":{"treemap":{"distributed":true,"enableShades":false,"dataLabels":{"enabled":true,"style":{"fontSize":"12px"}}}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"Pro-FvD","max":"Unspecified/Other"},"type":"treemap"},"evals":[],"jsHooks":[]}</script>
</div>
```
:::
:::


:::


> Deze visualisatie laat zien hoeveel AI-gegenereerde inhoud elke partij, politicus of andere actor heeft gepubliceerd. De veldgrootte komt overeen met het aantal geïdentificeerde berichten. Grotere velden duiden op een hoger gebruik van AI door de betreffende partij/actor.



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
<div id="htmlwidget-d130b5bb9079ba870a79" style="width:100%;height:400px;" class="apexcharter html-widget"></div>
<script type="application/json" data-for="htmlwidget-d130b5bb9079ba870a79">{"x":{"ax_opts":{"chart":{"type":"treemap","toolbar":{"show":false}},"series":[{"name":"y","data":[{"x":"Facebook","y":74},{"x":"Instagram","y":48},{"x":"TikTok","y":44}]}],"yaxis":{"labels":{"style":{"colors":"#848484"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}}},"title":{"text":"Per Platform","align":"center","style":{"fontSize":"16px"}},"legend":{"show":false},"colors":["#1877F2","#E4405F","#69C9D0"],"plotOptions":{"treemap":{"distributed":true,"enableShades":false,"dataLabels":{"enabled":true,"style":{"fontSize":"12px"}}}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"Facebook","max":"TikTok"},"type":"treemap"},"evals":[],"jsHooks":[]}</script>
</div>
```
:::
:::



> Deze visualisatie laat zien hoeveel AI-gegenereerde inhoud we per platform hebben gevonden. De veldgrootte komt overeen met het aantal geïdentificeerde berichten. Grotere velden duiden op meer AI-gegenereerde berichten op dat platform.

## Per Actortype {#ki-content-by-party2}




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
<div id="htmlwidget-3936565c5cad26d9b03f" style="width:100%;height:400px;" class="apexcharter html-widget"></div>
<script type="application/json" data-for="htmlwidget-3936565c5cad26d9b03f">{"x":{"ax_opts":{"chart":{"type":"treemap","toolbar":{"show":false}},"series":[{"name":"y","data":[{"x":"Partijen","y":87},{"x":"Overige Actoren","y":73},{"x":"Politici","y":6}]}],"yaxis":{"labels":{"style":{"colors":"#848484"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}}},"title":{"text":"Per Actortype","align":"center","style":{"fontSize":"16px"}},"legend":{"show":false},"colors":["#D55E00","#009E73","#0072B2"],"plotOptions":{"treemap":{"distributed":true,"enableShades":false,"dataLabels":{"enabled":true,"style":{"fontSize":"12px"}}}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"Overige Actoren","max":"Politici"},"type":"treemap"},"evals":[],"jsHooks":[]}</script>
</div>
```
:::


> 
Deze visualisatie laat zien hoeveel AI-gegenereerde inhoud we hebben gevonden per actortype (bijv. partijen, politici, overige actoren). De veldgrootte komt overeen met het aantal geïdentificeerde berichten. Grotere velden duiden op meer AI-gegenereerde berichten van dat actortype.


::: 


## Aandeel berichten met en zonder AI {#ki-content-by-party2}

Deze grafiek toont het *relatieve* aandeel AI-gegenereerde inhoud per partij. De partijen zijn gesorteerd naar het hoogste aandeel AI-inhoud.


<!-- ::: {.panel-tabset} -->


::: {.cell}

:::



<!-- ### Partijen & Politici -->


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
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-e70222b995b9c9e4b18e" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-e70222b995b9c9e4b18e">{"x":{"ax_opts":{"chart":{"type":"bar","animations":{"enabled":false},"background":"transparent","foreColor":"#000","toolbar":{"show":false},"height":648,"redrawOnWindowResize":true,"redrawOnParentResize":true},"series":[{"name":"Berichten met AI","data":[{"x":"De Linie","y":60,"n":3,"total":5},{"x":"Pro-PVV","y":33,"n":16,"total":48},{"x":"Satire","y":32,"n":18,"total":56},{"x":"50PLUS","y":27,"n":3,"total":11},{"x":"NCPN","y":23,"n":3,"total":13},{"x":"PVV","y":10,"n":46,"total":441},{"x":"Vrede voor Dieren","y":9,"n":1,"total":11},{"x":"Pro-Right","y":5,"n":30,"total":648},{"x":"LP","y":4,"n":1,"total":24},{"x":"Pro-FvD","y":4,"n":7,"total":169},{"x":"VVD","y":3,"n":11,"total":439},{"x":"BVNL","y":2,"n":1,"total":42},{"x":"BBB","y":2,"n":5,"total":226},{"x":"DENK","y":2,"n":2,"total":106},{"x":"CU","y":2,"n":1,"total":59},{"x":"GL-PvdA","y":1,"n":6,"total":482},{"x":"FvD","y":1,"n":3,"total":245},{"x":"SGP","y":1,"n":2,"total":177},{"x":"SP","y":1,"n":3,"total":385},{"x":"JA21","y":1,"n":1,"total":161},{"x":"D66","y":0.308641975308642,"n":1,"total":324},{"x":"Unspecified/Other","y":0.1657000828500414,"n":2,"total":1207}]}],"plotOptions":{"bar":{"horizontal":true,"barHeight":"55%","borderRadius":6,"distributed":true,"dataLabels":{"position":"center"}}},"colors":["#AA3377","#B22222","#6A5ACD","#7F2481","#CC0000","#003082","#5496c6","#8C6D1F","#003399","#7E2342","#FF7900","#132141","#009639","#00A7B3","#00A1DE","#C00040","#7B1E26","#E57200","#BE1E2D","#0C2E6E","#009E60","#17a2b8"],"dataLabels":{"enabled":true,"style":{"fontSize":"12px","fontWeight":"bold","colors":["#ffffff"]},"formatter":"function(v){ return (v < 2 ? '' : (Math.round(v*10)/10) + '%'); }"},"tooltip":{"shared":false,"y":{"formatter":"function(val, opts){ \n           var d  = opts.w.config.series[opts.seriesIndex].data[opts.dataPointIndex];\n           var nf = new Intl.NumberFormat();\n           return (Math.round(val*10)/10) + '% (' + d.n + ' / ' + nf.format(d.total) + ')';\n         }"}},"xaxis":{"labels":{"formatter":"v => v + \"%\""},"tickAmount":4,"max":80,"title":{"text":[]}},"yaxis":{"labels":{"style":{"fontSize":"13px","fontWeight":"600"}}},"grid":{"xaxis":{"lines":{"show":true}},"yaxis":{"lines":{"show":false}}},"legend":{"show":false},"title":{"text":"Aandeel berichten met AI","align":"center","style":{"fontSize":"18px","fontWeight":"bold"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false},"evals":["ax_opts.dataLabels.formatter","ax_opts.tooltip.y.formatter","ax_opts.xaxis.labels.formatter"],"jsHooks":[]}</script>
</div>
```
:::
:::



<!-- ### Overige Actoren -->

<!-- ```{r} -->

<!-- # ai_pct: % with AI per party (only parties with AI) -->
<!-- ai_pct <- full_data %>% -->
<!--   filter(!(list_source %in% c("Politicians","Parties"))) %>% -->
<!--   count(party, name = "total") %>% -->
<!--   left_join(full_data %>% filter(!(list_source %in% c("Politicians","Parties")), ai == 1) %>% -->
<!--               count(party, name = "n_ai"), -->
<!--             by = "party") %>% -->
<!--   mutate(n_ai = coalesce(n_ai, 0L), -->
<!--          pct  = ifelse(total > 0, 100 * n_ai / total, 0)) %>% -->
<!--   filter(n_ai > 0) %>% -->
<!--   arrange(desc(pct)) -->

<!-- if (nrow(ai_pct) == 0) { -->
<!--   apexchart() %>% ax_noData(text = "Geen AI-berichten gevonden") -->
<!-- } else { -->
<!--   # points carry counts for the tooltip -->
<!--   pts <- pmap( -->
<!--     list(x = ai_pct$party, -->
<!--          y = round(ai_pct$pct, 1), -->
<!--          n = ai_pct$n_ai, -->
<!--          total = ai_pct$total), -->
<!--     ~ list(x = ..1, y = ..2, n = ..3, total = ..4) -->
<!--   ) -->

<!--   cols <- unname(party_colors[ai_pct$party]); cols[is.na(cols)] <- "#17a2b8" -->
<!--   H <- max(240, 24 * nrow(ai_pct) + 120) -->

<!--  ooo <- apexchart() %>% -->
<!--     ax_chart( -->
<!--       type = "bar", -->
<!--       height = H, -->
<!--       background = "transparent", -->
<!--       foreColor  = "#000", -->
<!--       animations = list(enabled = FALSE), -->
<!--       redrawOnWindowResize = TRUE, -->
<!--       redrawOnParentResize = TRUE, -->
<!--       toolbar = list(show = FALSE) -->
<!--     ) %>% -->
<!--     ax_series(list(name = get_text("posts_with_ai", lang), data = pts)) %>% -->
<!--     ax_plotOptions( -->
<!--       bar = list( -->
<!--         horizontal   = TRUE, -->
<!--         barHeight    = "55%", -->
<!--         borderRadius = 6, -->
<!--         distributed  = TRUE, -->
<!--         dataLabels   = list(position = "center")   # <-- center text inside bar -->
<!--       ) -->
<!--     ) %>% -->
<!--     ax_colors(cols) %>% -->
<!--     ax_dataLabels( -->
<!--       enabled = TRUE, -->
<!--       style   = list(fontSize = "12px", fontWeight = "bold", colors = list("#ffffff")), -->
<!--       formatter = JS( -->
<!--         # show centered %; hide on very tiny bars so it doesn't overlap -->
<!--         "function(v){ return (v < 1 ? '' : (Math.round(v*10)/10) + '%'); }" -->
<!--       ) -->
<!--     ) %>% -->
<!--     ax_tooltip( -->
<!--       shared = FALSE, -->
<!--       y = list(formatter = JS( -->
<!--         # 23.1% (X out of 1,343 posts) -->
<!--         "function(val, opts){  -->
<!--            var d  = opts.w.config.series[opts.seriesIndex].data[opts.dataPointIndex]; -->
<!--            var nf = new Intl.NumberFormat(); -->
<!--            return (Math.round(val*10)/10) + '% (' + d.n + ' / ' + nf.format(d.total) + ')'; -->
<!--          }" -->
<!--       )) -->
<!--     ) %>% -->
<!--     ax_xaxis( -->
<!--       max = 80, tickAmount = 4, -->
<!--       labels = list(formatter = JS('v => v + "%"')), -->
<!--       title  = list(text = get_text("percent", lang)) -->
<!--     ) %>% -->
<!--     ax_yaxis( -->
<!--       labels = list(style = list(fontSize = "13px", fontWeight = "600"))  # party names only -->
<!--     ) %>% -->
<!--     ax_grid(xaxis = list(lines = list(show = TRUE)), -->
<!--             yaxis = list(lines = list(show = FALSE))) %>% -->
<!--     ax_legend(show = FALSE) %>% -->
<!--     ax_title(text = get_text("posts_with_ai", lang), -->
<!--              align = "center", -->
<!--              style = list(fontSize = "18px", fontWeight = "bold")) -->
<!-- } -->
<!-- # Embedding Chart into Responsive Container -->
<!-- htmltools::tagList( -->
<!--   custom_css, -->
<!--   tags$div( -->
<!--     class = "apex-container", -->
<!--     ooo -->
<!--   ) -->
<!-- ) -->



<!-- ``` -->





<!-- ::: -->


> Let op: bij actoren met minder totale berichten (inclusief kleinere partijen) kan zelfs beperkt AI-gebruik leiden tot hoge relatieve percentages.

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
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-e52706428c977f0960d9" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-e52706428c977f0960d9">{"x":{"ax_opts":{"chart":{"type":"radialBar","sparkline":{"enabled":true},"height":420,"animations":{"enabled":false},"background":"transparent","foreColor":"#000","redrawOnWindowResize":true,"redrawOnParentResize":true},"series":[68],"labels":["AI ZONDER disclaimer"],"yaxis":{"labels":{"style":{"colors":"#848484"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}}},"colors":["#FF4500"],"plotOptions":{"radialBar":{"hollow":{"size":"58%","margin":4},"track":{"margin":2},"dataLabels":{"name":{"show":true,"style":{"color":"#000","fontSize":"14px","fontWeight":"bold"}},"value":{"show":true,"formatter":"function(val){ return Math.round(val) + '%'; }","style":{"color":"#000","fontSize":"20px","fontWeight":"bold"}}}}},"stroke":{"show":true,"lineCap":"round"},"title":{"text":"Was de AI-inhoud (niet) voorzien van een disclaimer?","align":"center","style":{"fontSize":"18px","color":"#000"}},"theme":{"mode":"light"}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"AI ZONDER disclaimer","max":"AI ZONDER disclaimer"},"type":"radialBar"},"evals":["ax_opts.plotOptions.radialBar.dataLabels.value.formatter"],"jsHooks":[]}</script>
</div>
<div style="flex: 1; min-width: 300px;">
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-e4e471cf92e39470d0a7" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-e4e471cf92e39470d0a7">{"x":{"ax_opts":{"chart":{"type":"radialBar","sparkline":{"enabled":true},"height":420,"animations":{"enabled":false},"background":"transparent","foreColor":"#000","redrawOnWindowResize":true,"redrawOnParentResize":true},"series":[3.3,0,96.7],"labels":["In Beeld","In Tekst","Door Platform"],"yaxis":{"labels":{"style":{"colors":"#848484"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}}},"colors":["#FF6347","#4682B4","#32CD32"],"plotOptions":{"radialBar":{"hollow":{"size":"48%","margin":4},"track":{"margin":3},"dataLabels":{"name":{"show":true,"style":{"color":"#000","fontSize":"12px","fontWeight":"bold"}},"value":{"show":true,"formatter":"v => Math.round(v) + '%'","style":{"color":"#000","fontSize":"16px"}},"total":{"show":true,"label":"Door Platform","formatter":"\n            function(w){\n              var t = w.globals.seriesTotals;\n              var m = Math.max.apply(null, t);\n              return Math.round(m) + '%';\n            }\n          "}}}},"legend":{"show":false},"stroke":{"show":true,"lineCap":"round"},"title":{"text":"Hoe werd het gebruik van AI kenbaar gemaakt?","align":"center","style":{"fontSize":"18px","color":"#000"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"Door Platform","max":"In Tekst"},"type":"radialBar"},"evals":["ax_opts.plotOptions.radialBar.dataLabels.value.formatter","ax_opts.plotOptions.radialBar.dataLabels.total.formatter"],"jsHooks":[]}</script>
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
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-aa442b446b8af21552d6" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-aa442b446b8af21552d6">{"x":{"ax_opts":{"chart":{"type":"radialBar","sparkline":{"enabled":true},"height":420,"animations":{"enabled":false},"background":"transparent","foreColor":"#000","redrawOnWindowResize":true,"redrawOnParentResize":true},"series":[58],"labels":["AI ZONDER disclaimer"],"yaxis":{"labels":{"style":{"colors":"#848484"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}}},"colors":["#FF4500"],"plotOptions":{"radialBar":{"hollow":{"size":"58%","margin":4},"track":{"margin":2},"dataLabels":{"name":{"show":true,"style":{"color":"#000","fontSize":"14px","fontWeight":"bold"}},"value":{"show":true,"formatter":"function(val){ return Math.round(val) + '%'; }","style":{"color":"#000","fontSize":"20px","fontWeight":"bold"}}}}},"stroke":{"show":true,"lineCap":"round"},"title":{"text":"Was de AI-inhoud (niet) voorzien van een disclaimer?","align":"center","style":{"fontSize":"18px","color":"#000"}},"theme":{"mode":"light"}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"AI ZONDER disclaimer","max":"AI ZONDER disclaimer"},"type":"radialBar"},"evals":["ax_opts.plotOptions.radialBar.dataLabels.value.formatter"],"jsHooks":[]}</script>
</div>
<div style="flex: 1; min-width: 300px;">
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-94098d0df5c1ff91aa3e" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-94098d0df5c1ff91aa3e">{"x":{"ax_opts":{"chart":{"type":"radialBar","sparkline":{"enabled":true},"height":420,"animations":{"enabled":false},"background":"transparent","foreColor":"#000","redrawOnWindowResize":true,"redrawOnParentResize":true},"series":[0,9.699999999999999,100],"labels":["In Beeld","In Tekst","Door Platform"],"yaxis":{"labels":{"style":{"colors":"#848484"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}}},"colors":["#FF6347","#4682B4","#32CD32"],"plotOptions":{"radialBar":{"hollow":{"size":"48%","margin":4},"track":{"margin":3},"dataLabels":{"name":{"show":true,"style":{"color":"#000","fontSize":"12px","fontWeight":"bold"}},"value":{"show":true,"formatter":"v => Math.round(v) + '%'","style":{"color":"#000","fontSize":"16px"}},"total":{"show":true,"label":"Door Platform","formatter":"\n            function(w){\n              var t = w.globals.seriesTotals;\n              var m = Math.max.apply(null, t);\n              return Math.round(m) + '%';\n            }\n          "}}}},"legend":{"show":false},"stroke":{"show":true,"lineCap":"round"},"title":{"text":"Hoe werd het gebruik van AI kenbaar gemaakt?","align":"center","style":{"fontSize":"18px","color":"#000"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"Door Platform","max":"In Tekst"},"type":"radialBar"},"evals":["ax_opts.plotOptions.radialBar.dataLabels.value.formatter","ax_opts.plotOptions.radialBar.dataLabels.total.formatter"],"jsHooks":[]}</script>
</div>
</div>
</div>
```
:::
:::


<!-- ::: -->



> Het kenbaar maken van AI-inhoud via disclaimers of platformlabels is cruciaal voor transparantie. Deze visualisatie laat zien hoe vaak AI-gegenereerde content mét of zonder vermelding is gepubliceerd, en of het label is aangebracht door de actor (in tekst of beeld) of door het platform. 

<br>




## AI-mediavormen {#medienformatte}


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
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-f26c27cce1fe7306c008" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-f26c27cce1fe7306c008">{"x":{"ax_opts":{"chart":{"type":"bar","animations":{"enabled":false},"background":"transparent","foreColor":"#000","toolbar":{"show":false},"height":200,"redrawOnWindowResize":true,"redrawOnParentResize":true},"series":[{"name":"round(pct, 1)","data":[{"x":"Afbeelding(en) (n=79)","y":84.90000000000001},{"x":"Video(’s) (n=14)","y":15.1}]}],"dataLabels":{"enabled":true,"formatter":"function(v){ return (Math.round(v*10)/10) + '%'; }"},"plotOptions":{"bar":{"horizontal":true,"isDumbbell":false,"barHeight":"60%","borderRadius":6,"distributed":true}},"tooltip":{"shared":true,"intersect":false,"followCursor":true},"grid":{"yaxis":{"lines":{"show":false}},"xaxis":{"lines":{"show":true}}},"yaxis":{"labels":{"style":{"colors":"#848484","fontSize":"14px","fontWeight":"bold"}}},"xaxis":{"labels":{"style":{"colors":"#848484"},"formatter":"function(v){ return v + '%'; }"},"max":100,"title":{"text":[]}},"colors":["#FF6347","#4682B4"],"legend":{"show":false},"title":{"text":"AI Beeld of Video?","align":"center","style":{"fontSize":"18px","fontWeight":"bold"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"Afbeelding(en) (n=79)","max":"Video(’s) (n=14)"},"type":"bar"},"evals":["ax_opts.dataLabels.formatter","ax_opts.xaxis.labels.formatter"],"jsHooks":[]}</script>
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
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-1ec5edf65060dd16cf48" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-1ec5edf65060dd16cf48">{"x":{"ax_opts":{"chart":{"type":"bar","animations":{"enabled":false},"background":"transparent","foreColor":"#000","toolbar":{"show":false},"height":200,"redrawOnWindowResize":true,"redrawOnParentResize":true},"series":[{"name":"round(pct, 1)","data":[{"x":"Video(’s) (n=52)","y":71.2},{"x":"Afbeelding(en) (n=21)","y":28.8}]}],"dataLabels":{"enabled":true,"formatter":"function(v){ return (Math.round(v*10)/10) + '%'; }"},"plotOptions":{"bar":{"horizontal":true,"isDumbbell":false,"barHeight":"60%","borderRadius":6,"distributed":true}},"tooltip":{"shared":true,"intersect":false,"followCursor":true},"grid":{"yaxis":{"lines":{"show":false}},"xaxis":{"lines":{"show":true}}},"yaxis":{"labels":{"style":{"colors":"#848484","fontSize":"14px","fontWeight":"bold"}}},"xaxis":{"labels":{"style":{"colors":"#848484"},"formatter":"function(v){ return v + '%'; }"},"max":100,"title":{"text":[]}},"colors":["#FF6347","#4682B4"],"legend":{"show":false},"title":{"text":"AI Beeld of Video?","align":"center","style":{"fontSize":"18px","fontWeight":"bold"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"Afbeelding(en) (n=21)","max":"Video(’s) (n=52)"},"type":"bar"},"evals":["ax_opts.dataLabels.formatter","ax_opts.xaxis.labels.formatter"],"jsHooks":[]}</script>
</div>
```
:::
:::



:::

> Deze grafiek toont het aandeel afbeeldingen en video’s in AI-gegenereerde berichten, en of ze er echt uitzien (camera-achtig of deepfakes) of tekeningen/grafisch zijn.


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
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-200361807d5d3ca59811" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-200361807d5d3ca59811">{"x":{"ax_opts":{"chart":{"type":"bar","animations":{"enabled":false},"background":"transparent","foreColor":"#000","toolbar":{"show":false},"height":200,"redrawOnWindowResize":true,"redrawOnParentResize":true},"series":[{"name":"round(pct, 1)","data":[{"x":"Lijkt echt (deepfake) (n=72)","y":77.40000000000001},{"x":"Lijkt niet echt (grafisch/tekening) (n=21)","y":22.6}]}],"dataLabels":{"enabled":true,"formatter":"function(v){ return (Math.round(v*10)/10) + '%'; }"},"plotOptions":{"bar":{"horizontal":true,"isDumbbell":false,"barHeight":"60%","borderRadius":6,"distributed":true}},"tooltip":{"shared":true,"intersect":false,"followCursor":true},"grid":{"yaxis":{"lines":{"show":false}},"xaxis":{"lines":{"show":true}}},"yaxis":{"labels":{"style":{"colors":"#848484","fontSize":"14px","fontWeight":"bold"}}},"xaxis":{"labels":{"style":{"colors":"#848484"},"formatter":"function(v){ return v + '%'; }"},"max":100,"title":{"text":[]}},"colors":["#1F5A96","#AC0999"],"legend":{"show":false},"title":{"text":"Is de AI-inhoud realistisch?","align":"center","style":{"fontSize":"18px","fontWeight":"bold"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"Lijkt echt (deepfake) (n=72)","max":"Lijkt niet echt (grafisch/tekening) (n=21)"},"type":"bar"},"evals":["ax_opts.dataLabels.formatter","ax_opts.xaxis.labels.formatter"],"jsHooks":[]}</script>
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
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-41fcb61284772b0e8aad" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-41fcb61284772b0e8aad">{"x":{"ax_opts":{"chart":{"type":"bar","animations":{"enabled":false},"background":"transparent","foreColor":"#000","toolbar":{"show":false},"height":200,"redrawOnWindowResize":true,"redrawOnParentResize":true},"series":[{"name":"round(pct, 1)","data":[{"x":"Lijkt echt (deepfake) (n=64)","y":88.90000000000001},{"x":"Lijkt niet echt (grafisch/tekening) (n=8)","y":11.1}]}],"dataLabels":{"enabled":true,"formatter":"function(v){ return (Math.round(v*10)/10) + '%'; }"},"plotOptions":{"bar":{"horizontal":true,"isDumbbell":false,"barHeight":"60%","borderRadius":6,"distributed":true}},"tooltip":{"shared":true,"intersect":false,"followCursor":true},"grid":{"yaxis":{"lines":{"show":false}},"xaxis":{"lines":{"show":true}}},"yaxis":{"labels":{"style":{"colors":"#848484","fontSize":"14px","fontWeight":"bold"}}},"xaxis":{"labels":{"style":{"colors":"#848484"},"formatter":"function(v){ return v + '%'; }"},"max":100,"title":{"text":[]}},"colors":["#1F5A96","#AC0999"],"legend":{"show":false},"title":{"text":"Is de AI-inhoud realistisch?","align":"center","style":{"fontSize":"18px","fontWeight":"bold"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"Lijkt echt (deepfake) (n=64)","max":"Lijkt niet echt (grafisch/tekening) (n=8)"},"type":"bar"},"evals":["ax_opts.dataLabels.formatter","ax_opts.xaxis.labels.formatter"],"jsHooks":[]}</script>
</div>
```
:::
:::




:::



> Deze grafiek toont het aandeel afbeeldingen en video’s in AI-gegenereerde berichten, en of ze er echt uitzien (camera-achtig of deepfakes) of tekeningen/grafisch zijn.



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
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-6ff0bcc804aecb8297c1" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-6ff0bcc804aecb8297c1">{"x":{"ax_opts":{"chart":{"type":"bar"},"series":[{"name":"n","data":[{"x":"Positief","y":84},{"x":"Negatief","y":47}]}],"dataLabels":{"enabled":true,"formatter":"function(val) { return val + ' Berichten'; }"},"plotOptions":{"bar":{"horizontal":true,"isDumbbell":false,"barHeight":"60%","borderRadius":5,"distributed":true}},"tooltip":{"shared":true,"intersect":false,"followCursor":true,"y":{"formatter":"function(val) { return val + ' Berichten'; }"}},"grid":{"yaxis":{"lines":{"show":false}},"xaxis":{"lines":{"show":true}}},"yaxis":{"labels":{"style":{"colors":"#848484","fontSize":"14px","fontWeight":"bold"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}},"title":{"text":"Aantal berichten"}},"colors":["#4CAF50","#F44336","#9E9E9E"],"title":{"text":"Verdeling van toon in AI-gegenereerde inhoud","align":"center","style":{"fontSize":"18px","fontWeight":"bold"}},"legend":{"position":"bottom","labels":{"colors":"#000"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"Negatief","max":"Positief"},"type":"bar"},"evals":["ax_opts.dataLabels.formatter","ax_opts.tooltip.y.formatter"],"jsHooks":[]}</script>
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
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-f465537c8636b54b76b8" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-f465537c8636b54b76b8">{"x":{"ax_opts":{"chart":{"type":"bar"},"series":[{"name":"n","data":[{"x":"Negatief","y":59},{"x":"Positief","y":36}]}],"dataLabels":{"enabled":true,"formatter":"function(val) { return val + ' Berichten'; }"},"plotOptions":{"bar":{"horizontal":true,"isDumbbell":false,"barHeight":"60%","borderRadius":5,"distributed":true}},"tooltip":{"shared":true,"intersect":false,"followCursor":true,"y":{"formatter":"function(val) { return val + ' Berichten'; }"}},"grid":{"yaxis":{"lines":{"show":false}},"xaxis":{"lines":{"show":true}}},"yaxis":{"labels":{"style":{"colors":"#848484","fontSize":"14px","fontWeight":"bold"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}},"title":{"text":"Aantal berichten"}},"colors":["#4CAF50","#F44336","#9E9E9E"],"title":{"text":"Verdeling van toon in AI-gegenereerde inhoud","align":"center","style":{"fontSize":"18px","fontWeight":"bold"}},"legend":{"position":"bottom","labels":{"colors":"#000"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"Negatief","max":"Positief"},"type":"bar"},"evals":["ax_opts.dataLabels.formatter","ax_opts.tooltip.y.formatter"],"jsHooks":[]}</script>
</div>
```
:::
:::



:::



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
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-1c2b77776eecba885628" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-1c2b77776eecba885628">{"x":{"ax_opts":{"chart":{"type":"bar","stacked":false,"height":800,"horizontal":true},"series":[{"name":"n","data":[{"x":"Politieke partijen & politici","y":49},{"x":"Stemappèl","y":43},{"x":"Binnenlands & Migratiebeleid","y":34},{"x":"Verkiezingen (algemeen)","y":21},{"x":"Arbeid & Sociale Zaken","y":18},{"x":"Economie & Financiën","y":16},{"x":"Wooncrisis","y":13},{"x":"Defensiebeleid","y":9},{"x":"Digitaal & Infrastructuur","y":9},{"x":"Energiebeleid","y":9},{"x":"Onderwijs & Cultuur","y":8},{"x":"Grondrechten","y":4},{"x":"Overige politieke thema’s","y":2},{"x":"Europa","y":1}]}],"dataLabels":{"enabled":true,"formatter":"function(val) { return val + ' Berichten'; }"},"plotOptions":{"bar":{"horizontal":true,"isDumbbell":false,"barHeight":"60%","borderRadius":5}},"tooltip":{"shared":true,"intersect":false,"followCursor":true,"y":{"formatter":"function(val) { return val + ' Berichten'; }"}},"grid":{"yaxis":{"lines":{"show":false}},"xaxis":{"lines":{"show":true}}},"yaxis":{"labels":{"style":{"colors":"#848484","fontSize":"14px","fontWeight":"bold"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}},"title":{"text":"Aantal berichten"}},"title":{"text":"Verdeling van thema’s in AI-gegenereerde inhoud","align":"center","style":{"fontSize":"18px","fontWeight":"bold"}},"legend":{"position":"bottom","labels":{"colors":"#000"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"type":"bar"},"evals":["ax_opts.dataLabels.formatter","ax_opts.tooltip.y.formatter"],"jsHooks":[]}</script>
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
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-2f89d7faf8a1e79f1186" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-2f89d7faf8a1e79f1186">{"x":{"ax_opts":{"chart":{"type":"bar","stacked":false,"height":800,"horizontal":true},"series":[{"name":"n","data":[{"x":"Binnenlands & Migratiebeleid","y":39},{"x":"Politieke partijen & politici","y":26},{"x":"Wooncrisis","y":17},{"x":"Stemappèl","y":15},{"x":"Europa","y":10},{"x":"Overige politieke thema’s","y":10},{"x":"Economie & Financiën","y":7},{"x":"Defensiebeleid","y":6},{"x":"Grondrechten","y":6},{"x":"Energiebeleid","y":5},{"x":"Onderwijs & Cultuur","y":5},{"x":"Arbeid & Sociale Zaken","y":4},{"x":"topic_constitution_system","y":4},{"x":"Verkiezingen (algemeen)","y":2},{"x":"Digitaal & Infrastructuur","y":1}]}],"dataLabels":{"enabled":true,"formatter":"function(val) { return val + ' Berichten'; }"},"plotOptions":{"bar":{"horizontal":true,"isDumbbell":false,"barHeight":"60%","borderRadius":5}},"tooltip":{"shared":true,"intersect":false,"followCursor":true,"y":{"formatter":"function(val) { return val + ' Berichten'; }"}},"grid":{"yaxis":{"lines":{"show":false}},"xaxis":{"lines":{"show":true}}},"yaxis":{"labels":{"style":{"colors":"#848484","fontSize":"14px","fontWeight":"bold"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}},"title":{"text":"Aantal berichten"}},"title":{"text":"Verdeling van thema’s in AI-gegenereerde inhoud","align":"center","style":{"fontSize":"18px","fontWeight":"bold"}},"legend":{"position":"bottom","labels":{"colors":"#000"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"type":"bar"},"evals":["ax_opts.dataLabels.formatter","ax_opts.tooltip.y.formatter"],"jsHooks":[]}</script>
</div>
```
:::
:::





:::



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
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-03af74c7e3404748d855" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-03af74c7e3404748d855">{"x":{"ax_opts":{"chart":{"type":"bar","stacked":false,"height":800,"horizontal":true},"series":[{"name":"n","data":[{"x":"Positieve beeldvorming / lof","y":63},{"x":"Symbolische afbeelding (frontaal afgebeelde mensen)","y":61},{"x":"Negatieve beeldvorming / campagnes","y":32},{"x":"Evenementaankondiging / verkiezingsappèl / kandidatenintroductie","y":26},{"x":"Humor / Satire","y":9},{"x":"Campagne-evenementen","y":6},{"x":"Dagelijkse politiek","y":6},{"x":"Mediaverkeer (incl. tv-debatten)","y":5},{"x":"Nostalgisch / Historisch","y":5},{"x":"Overige beeldinhoud","y":1}]}],"dataLabels":{"enabled":true,"formatter":"function(val) { return val + ' Berichten'; }"},"plotOptions":{"bar":{"horizontal":true,"isDumbbell":false,"barHeight":"60%","borderRadius":5}},"tooltip":{"shared":true,"intersect":false,"followCursor":true,"y":{"formatter":"function(val) { return val + ' Berichten'; }"}},"grid":{"yaxis":{"lines":{"show":false}},"xaxis":{"lines":{"show":true}}},"yaxis":{"labels":{"style":{"colors":"#848484","fontSize":"14px","fontWeight":"bold"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}},"title":{"text":"Aantal berichten"}},"title":{"text":"Verdeling van beeld-/video-inhoud in AI-gegenereerde inhoud","align":"center","style":{"fontSize":"18px","fontWeight":"bold"}},"legend":{"position":"bottom","labels":{"colors":"#000"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"type":"bar"},"evals":["ax_opts.dataLabels.formatter","ax_opts.tooltip.y.formatter"],"jsHooks":[]}</script>
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
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-4d94a6621e56ed7b7fc5" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-4d94a6621e56ed7b7fc5">{"x":{"ax_opts":{"chart":{"type":"bar","stacked":false,"height":800,"horizontal":true},"series":[{"name":"n","data":[{"x":"Symbolische afbeelding (frontaal afgebeelde mensen)","y":52},{"x":"Negatieve beeldvorming / campagnes","y":43},{"x":"Humor / Satire","y":23},{"x":"Positieve beeldvorming / lof","y":22},{"x":"Evenementaankondiging / verkiezingsappèl / kandidatenintroductie","y":13},{"x":"Nostalgisch / Historisch","y":6},{"x":"Mediaverkeer (incl. tv-debatten)","y":5},{"x":"Dagelijkse politiek","y":1},{"x":"Overige beeldinhoud","y":1},{"x":"Utopia or Dystopia","y":1}]}],"dataLabels":{"enabled":true,"formatter":"function(val) { return val + ' Berichten'; }"},"plotOptions":{"bar":{"horizontal":true,"isDumbbell":false,"barHeight":"60%","borderRadius":5}},"tooltip":{"shared":true,"intersect":false,"followCursor":true,"y":{"formatter":"function(val) { return val + ' Berichten'; }"}},"grid":{"yaxis":{"lines":{"show":false}},"xaxis":{"lines":{"show":true}}},"yaxis":{"labels":{"style":{"colors":"#848484","fontSize":"14px","fontWeight":"bold"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}},"title":{"text":"Aantal berichten"}},"title":{"text":"Verdeling van beeld-/video-inhoud in AI-gegenereerde inhoud","align":"center","style":{"fontSize":"18px","fontWeight":"bold"}},"legend":{"position":"bottom","labels":{"colors":"#000"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"type":"bar"},"evals":["ax_opts.dataLabels.formatter","ax_opts.tooltip.y.formatter"],"jsHooks":[]}</script>
</div>
```
:::
:::



:::


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
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-94e72b221fe15f4d6df4" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-94e72b221fe15f4d6df4">{"x":{"ax_opts":{"chart":{"type":"treemap"},"series":[{"name":[],"data":[{"x":"Vertegenwoordigers van sociale bewegingen","y":1},{"x":"GL-PvdA: Frans Timmermans","y":3},{"x":"Niet-politieke vertegenwoordigers van instituties","y":6},{"x":"Illegale/criminelen/extremisten","y":9},{"x":"PVV: Geert Wilders","y":10},{"x":"Minderheden","y":16},{"x":"Gewone mensen","y":59}]}],"yaxis":{"labels":{"style":{"colors":"#848484","fontSize":"14px","fontWeight":"bold"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}},"title":{"text":"Aantal berichten"}},"colors":["#547D01"],"dataLabels":{"style":{"colors":["#000000"]}},"title":{"text":"Verdeling van personen in AI-gegenereerde inhoud","align":"center","style":{"fontSize":"18px","fontWeight":"bold"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"Gewone mensen","max":"Vertegenwoordigers van sociale bewegingen"},"type":"treemap"},"evals":[],"jsHooks":[]}</script>
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
<div class="apexcharter html-widget html-fill-item" id="htmlwidget-f2c2e27ee675fe4fe2f9" style="width:100%;height:100%;"></div>
<script type="application/json" data-for="htmlwidget-f2c2e27ee675fe4fe2f9">{"x":{"ax_opts":{"chart":{"type":"treemap"},"series":[{"name":[],"data":[{"x":"Buitenlandse politici (niet-EU, VN, NAVO)","y":1},{"x":"GL-PvdA: Jesse Klaver","y":1},{"x":"Andere personen","y":2},{"x":"JA21: Joost Eerdmans","y":2},{"x":"Andere partijen","y":3},{"x":"CDA: Henri Bontenbal","y":3},{"x":"Denk: Stephan van Baarle","y":3},{"x":"Niet-politieke vertegenwoordigers van instituties","y":3},{"x":"Overige politici","y":3},{"x":"Vertegenwoordigers van sociale bewegingen","y":3},{"x":"VVD: Dilan Yeşilgöz","y":3},{"x":"BBB: Caroline van der Plas","y":4},{"x":"D66: Rob Jetten","y":4},{"x":"GL-PvdA: Frans Timmermans","y":5},{"x":"PvdD: Esther Ouwehand","y":5},{"x":"PVV: Geert Wilders","y":5},{"x":"Illegale/criminelen/extremisten","y":6},{"x":"Journalisten / nieuwsmedia","y":7},{"x":"Beroemdheden / opiniemakers","y":9},{"x":"Minderheden","y":10},{"x":"Buitenlandse politici (EU, VN, NAVO)","y":16},{"x":"Gewone mensen","y":46}]}],"yaxis":{"labels":{"style":{"colors":"#848484","fontSize":"14px","fontWeight":"bold"}}},"xaxis":{"labels":{"style":{"colors":"#848484"}},"title":{"text":"Aantal berichten"}},"colors":["#547D01"],"dataLabels":{"style":{"colors":["#000000"]}},"title":{"text":"Verdeling van personen in AI-gegenereerde inhoud","align":"center","style":{"fontSize":"18px","fontWeight":"bold"}}},"auto_update":{"series_animate":true,"update_options":false,"options_animate":true,"options_redrawPaths":true,"update_synced_charts":false},"sparkbox":false,"xaxis":{"min":"Andere partijen","max":"VVD: Dilan Yeşilgöz"},"type":"treemap"},"evals":[],"jsHooks":[]}</script>
</div>
```
:::
:::




:::

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
<div class="highchart html-widget html-fill-item" id="htmlwidget-4e93d29bb13aa7bb903f" style="width:100%;height:500px;"></div>
<script type="application/json" data-for="htmlwidget-4e93d29bb13aa7bb903f">{"x":{"hc_opts":{"chart":{"reflow":true,"type":"line"},"title":{"text":"AI-berichten door de tijd heen"},"yAxis":{"title":{"text":"Aantal berichten"}},"credits":{"enabled":false},"exporting":{"enabled":false},"boost":{"enabled":false},"plotOptions":{"series":{"label":{"enabled":false},"turboThreshold":0},"treemap":{"layoutAlgorithm":"squarified"}},"xAxis":{"categories":["2025-09-17","2025-09-18","2025-09-19","2025-09-20","2025-09-21","2025-09-22","2025-09-23","2025-09-24","2025-09-25"]},"series":[{"data":[7,22,21,23,18,19,20,14,22],"name":"Berichten met AI","color":"#FF6F61"},{"data":[803,772,664,622,507,693,779,750,824],"name":"Berichten zonder AI","color":"#6B5B95"}],"tooltip":{"pointFormat":"<b>{series.name}<\/b>: {point.y}"}},"theme":{"chart":{"backgroundColor":"transparent"},"colors":["#7cb5ec","#434348","#90ed7d","#f7a35c","#8085e9","#f15c80","#e4d354","#2b908f","#f45b5b","#91e8e1"]},"conf_opts":{"global":{"Date":null,"VMLRadialGradientURL":"http =//code.highcharts.com/list(version)/gfx/vml-radial-gradient.png","canvasToolsURL":"http =//code.highcharts.com/list(version)/modules/canvas-tools.js","getTimezoneOffset":null,"timezoneOffset":0,"useUTC":true},"lang":{"contextButtonTitle":"Chart context menu","decimalPoint":".","downloadCSV":"Download CSV","downloadJPEG":"Download JPEG image","downloadPDF":"Download PDF document","downloadPNG":"Download PNG image","downloadSVG":"Download SVG vector image","downloadXLS":"Download XLS","drillUpText":"◁ Back to {series.name}","exitFullscreen":"Exit from full screen","exportData":{"annotationHeader":"Annotations","categoryDatetimeHeader":"DateTime","categoryHeader":"Category"},"hideData":"Hide data table","invalidDate":null,"loading":"Loading...","months":["January","February","March","April","May","June","July","August","September","October","November","December"],"noData":"No data to display","numericSymbolMagnitude":1000,"numericSymbols":["k","M","G","T","P","E"],"printChart":"Print chart","resetZoom":"Reset zoom","resetZoomTitle":"Reset zoom level 1:1","shortMonths":["Jan","Feb","Mar","Apr","May","Jun","Jul","Aug","Sep","Oct","Nov","Dec"],"shortWeekdays":["Sat","Sun","Mon","Tue","Wed","Thu","Fri"],"thousandsSep":" ","viewData":"View data table","viewFullscreen":"View in full screen","weekdays":["Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday"]}},"type":"chart","fonts":[],"debug":false},"evals":[],"jsHooks":[]}</script>
</div>
```
:::
:::


<br>

> Deze grafiek toont het gebruik van AI versus niet-AI-inhoud door de tijd heen.

<br>

<br>
<center>
  <a href="https://favstats.github.io/campaigntrackernl">
    <img src="logobelow.png" width="50%">
  </a>
</center>


