<style>
div.graphic-panel {
    display: block;
    height: 300px;
    text-align: center;
    margin-bottom: 100px;
}
.graphic-element {
    display: inline-block;
    width: 40%;
}
</style>

<div class="graphic-panel" id="linea-1">
    <div class="graphic-element" id="emae"></div>
    <div class="graphic-element" id="ipi"></div>
    <div class="graphic-element" id="isac"></div>
</div>
<div class="graphic-panel" id="linea-2">
    <div class="graphic-element" id="ipc"></div>
    <div class="graphic-element" id="trabajadores"></div>
    <div class="graphic-element" id="desempleo"></div>
</div>

<script type='text/javascript' src='https://cdn.jsdelivr.net/gh/datosgobar/series-tiempo-ar-explorer@ts_components_2.9.0/dist/js/components.js'></script>

<script>
window.onload = function() {

    TSComponents.Graphic.render('emae', {
        graphicUrl: 'https://apis.datos.gob.ar/series/api/series/?ids=143.3_NO_PR_2004_A_21:percent_change_a_year_ago,143.3_NO_PR_2004_A_31:percent_change&limit=1000&start_date=2017-11',
        chartOptions: { // Override highstock configs. See https://api.highcharts.com/highstock/
        },
        title: 'Estimador Mensual de Actividad Económica (EMAE). Base 2004',
        source: 'Instituto Nacional de Estadística y Censos (INDEC)',
        chartTypes: { "143.3_NO_PR_2004_A_21": "column", "143.3_NO_PR_2004_A_31": "column" }
    })

    TSComponents.Graphic.render('ipi', {
        graphicUrl: 'https://apis.datos.gob.ar/series/api/series/?ids=IPI_UIA_8QBRJ5:percent_change_a_year_ago&limit=1000&start_date=2017-12',
        chartOptions: { // Override highstock configs. See https://api.highcharts.com/highstock/
        },
        title: 'Valor del Índice de Producción Industrial de la UIA',
        source: 'Ministerio de Producción. Secretaría de la Transformación Productiva. Subsecretaría de Desarrollo y Planeamiento Productivo.',
        chartTypes: {"IPI_UIA_8QBRJ5": "column"}
    })

    TSComponents.Graphic.render('isac', {
        graphicUrl: 'https://apis.datos.gob.ar/series/api/series/?ids=33.2_ISAC_SIN_EDAD_0_M_23_56:percent_change_a_year_ago&limit=1000&start_date=2017-12',
        chartOptions: { // Override highstock configs. See https://api.highcharts.com/highstock/
        },
        title: 'Indicador sintético de la actividad de la construcción. Sin Estacionalidad',
        source: 'Instituto Nacional de Estadística y Censos (INDEC)',
        chartTypes: {"33.2_ISAC_SIN_EDAD_0_M_23_56": "column"}
    })

    TSComponents.Graphic.render('ipc', {
        graphicUrl: 'https://apis.datos.gob.ar/series/api/series/?ids=148.3_INIVELNAL_DICI_M_26:percent_change&limit=1000&start_date=2018-01',
        chartOptions: { // Override highstock configs. See https://api.highcharts.com/highstock/
        },
        title: 'Índice de Precios al Consumidor. Nivel General Nacional. Base diciembre 2016. Valores mensuales.',
        source: 'Instituto Nacional de Estadística y Censos (INDEC)',
    })

    TSComponents.Graphic.render('trabajadores', {
        graphicUrl: 'https://apis.datos.gob.ar/series/api/series/?ids=151.1_TL_SIN_TAC_2012_M_15,151.1_TL_ESTADAD_2012_M_20&limit=1000&start_date=2017-11',
        chartOptions: { // Override highstock configs. See https://api.highcharts.com/highstock/
        },
        title: 'Trabajadores registrados según modalidad ocupacional principal. Base 2012',
        source: 'Ministerio de Trabajo, Empleo y Seguridad Social',
    })

    TSComponents.Graphic.render('desempleo', {
        graphicUrl: 'https://apis.datos.gob.ar/series/api/series/?ids=42.3_EPH_PUNTUATAL_0_M_30&limit=1000&start_date=2016',
        chartOptions: { // Override highstock configs. See https://api.highcharts.com/highstock/
        },
        title: 'Tasa de desocupación total. En porcentaje.',
        source: 'Instituto Nacional de Estadística y Censos (INDEC)',
        chartTypes: { "42.3_EPH_PUNTUATAL_0_M_30": "column" }
    })
}
</script>
