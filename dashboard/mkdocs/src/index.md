### Card: default

<div class="row">
        <div style='display: inline-block;'>
            <div id='ipc-card'></div>
        </div>
        <div style='display: inline-block;'>
            <div id='exportaciones-card'> </div>
        </div>
        <div style='display: inline-block;'>
            <div id='superavit-card'></div>
        </div>
        <div style='display: inline-block;'>
            <div id='desempleo-card'></div>
        </div>
</div>

### Card: menos links

<div class="row">
        <div id='ipc-card-links2' class="col-xs-12 col-sm-6 col-md-3"></div>
        <div id='exportaciones-card-links2' class="col-xs-12 col-sm-6 col-md-3"></div>
        <div id='superavit-card-links2' class="col-xs-12 col-sm-6 col-md-3"></div>
        <div id='desempleo-card-links2' class="col-xs-12 col-sm-6 col-md-3"></div>
</div>

### Card: sin links

<div class="row">
        <div id='ipc-card-med' class="col-xs-12 col-sm-6 col-md-3"></div>
        <div id='exportaciones-card-med' class="col-xs-12 col-sm-6 col-md-3"></div>
        <div id='superavit-card-med' class="col-xs-12 col-sm-6 col-md-3"></div>
        <div id='desempleo-card-med' class="col-xs-12 col-sm-6 col-md-3"></div>
</div>

### Card: mínima

<div class="row">
        <div id='ipc-card-min' class="col-xs-12 col-sm-6 col-md-3"></div>
        <div id='exportaciones-card-min' class="col-xs-12 col-sm-6 col-md-3"></div>
        <div id='superavit-card-min' class="col-xs-12 col-sm-6 col-md-3"></div>
        <div id='desempleo-card-min' class="col-xs-12 col-sm-6 col-md-3"></div>
</div>

### Card: mínima (eliminando elementos)

<div class="row">
        <div id='ipc-card-min-xtreme' class="col-xs-12 col-sm-6 col-md-3"></div>
        <div id='exportaciones-card-min-xtreme' class="col-xs-12 col-sm-6 col-md-3"></div>
        <div id='superavit-card-min-xtreme' class="col-xs-12 col-sm-6 col-md-3"></div>
        <div id='desempleo-card-min-xtreme' class="col-xs-12 col-sm-6 col-md-3"></div>
</div>

### Graphic: full

<div class="row row-graphic">
        <div id='tcrm-graphic'></div>
</div>

### Graphic: sin filtros de tiempo

<div class="row row-graphic">
        <div id='emae-graphic-without-filters' class="col-xs-12 col-sm-6 col-md-6"></div>
        <div id='ica-graphic-without-filters' class="col-xs-12 col-sm-6 col-md-6"></div>
</div>

### Graphic: mínimo

<div class="row row-graphic-min">
        <div id='ipc-graphic-min' class="col-xs-12 col-sm-6 col-md-4"></div>
        <div id='rem-graphic-min' class="col-xs-12 col-sm-6 col-md-4"></div>
        <div id='tcbna-graphic-min' class="col-xs-12 col-sm-6 col-md-4"></div>
</div>

<script>
    window.onload = function() {
        // componentes de series de tiempo

        TSComponents.Card.render('ipc-card', {
            serieId: '148.3_INIVELNAL_DICI_M_26:percent_change',
            color: '#F9A822',
            hasChart: 'small',
            title: "Indice de Precios al Consumidor Nacional"
        })

        TSComponents.Card.render('exportaciones-card', {
            serieId: '74.3_IET_0_M_16:percent_change_a_year_ago',
            explicitSign: true,
            hasChart: 'small',
            title: "Exportaciones"
        })

        TSComponents.Card.render('superavit-card', {
            serieId: '372.6_SUPERAVIT_017__23_67',
            hasChart: 'small',
            title: "Resultado Primario del Sector Público No Fin."
        })

        TSComponents.Card.render('desempleo-card', {
            serieId: '42.3_EPH_PUNTUATAL_0_M_30',
            color: '#EC407A',
            hasChart: 'small',
            title: "Desocupación"
        })

        TSComponents.Card.render('ipc-card-links2', {
            serieId: '148.3_INIVELNAL_DICI_M_26:percent_change',
            color: '#F9A822',
            hasChart: 'small',
            links: "small",
            title: "Indice de Precios al Consumidor Nacional"
        })

        TSComponents.Card.render('exportaciones-card-links2', {
            serieId: '74.3_IET_0_M_16:percent_change_a_year_ago',
            explicitSign: true,
            hasChart: 'small',
            links: "small",
            title: "Exportaciones"
        })

        TSComponents.Card.render('superavit-card-links2', {
            serieId: '372.6_SUPERAVIT_017__23_67',
            hasChart: 'small',
            links: "small",
            title: "Resultado Primario del Sector Público No Fin."
        })

        TSComponents.Card.render('desempleo-card-links2', {
            serieId: '42.3_EPH_PUNTUATAL_0_M_30',
            color: '#EC407A',
            hasChart: 'small',
            links: "small",
            title: "Desocupación"
        })

        TSComponents.Card.render('ipc-card-med', {
            serieId: '148.3_INIVELNAL_DICI_M_26:percent_change',
            color: '#F9A822',
            hasChart: 'small',
            links: "none",
            title: "Indice de Precios al Consumidor Nacional"
        })

        TSComponents.Card.render('exportaciones-card-med', {
            serieId: '74.3_IET_0_M_16:percent_change_a_year_ago',
            explicitSign: true,
            hasChart: 'small',
            links: "none",
            title: "Exportaciones"
        })

        TSComponents.Card.render('superavit-card-med', {
            serieId: '372.6_SUPERAVIT_017__23_67',
            hasChart: 'small',
            links: "none",
            title: "Resultado Primario del Sector Público No Fin."
        })

        TSComponents.Card.render('desempleo-card-med', {
            serieId: '42.3_EPH_PUNTUATAL_0_M_30',
            color: '#EC407A',
            hasChart: 'small',
            links: "none",
            title: "Desocupación"
        })

        TSComponents.Card.render('ipc-card-min', {
            serieId: '148.3_INIVELNAL_DICI_M_26:percent_change',
            color: '#F9A822',
            links: 'none',
            hasChart: "none",
            title: "Indice de Precios al Consumidor Nacional"
        })

        TSComponents.Card.render('exportaciones-card-min', {
            serieId: '74.3_IET_0_M_16:percent_change_a_year_ago',
            explicitSign: true,
            links: 'none',
            hasChart: "none",
            title: "Exportaciones"
        })

        TSComponents.Card.render('superavit-card-min', {
            serieId: '372.6_SUPERAVIT_017__23_67',
            links: 'none',
            hasChart: "none",
            title: "Resultado Primario del Sector Público No Fin."
        })

        TSComponents.Card.render('desempleo-card-min', {
            serieId: '42.3_EPH_PUNTUATAL_0_M_30',
            color: '#EC407A',
            links: 'none',
            hasChart: "none",
            title: "Desocupación"
        })

        TSComponents.Card.render('ipc-card-min-xtreme', {
            serieId: '148.3_INIVELNAL_DICI_M_26:percent_change',
            links: 'none',
            hasChart: "none",
            title: "",
            units: "",
            source: ""
        })

        TSComponents.Card.render('exportaciones-card-min-xtreme', {
            serieId: '74.3_IET_0_M_16:percent_change_a_year_ago',
            explicitSign: true,
            links: 'none',
            hasChart: "none",
            title: "",
            units: "",
            source: ""
        })

        TSComponents.Card.render('superavit-card-min-xtreme', {
            serieId: '372.6_SUPERAVIT_017__23_67',
            links: 'none',
            hasChart: "none",
            title: "",
            units: "",
            source: ""
        })

        TSComponents.Card.render('desempleo-card-min-xtreme', {
            serieId: '42.3_EPH_PUNTUATAL_0_M_30',
            color: '#EC407A',
            links: 'none',
            hasChart: "none",
            title: "",
            units: "",
            source: ""
        })

        TSComponents.Graphic.render('tcrm-graphic', {
            graphicUrl: 'https://apis.datos.gob.ar/series/api/series/?metadata=full&ids=143.3_NO_PR_2004_A_21:percent_change_a_year_ago,116.4_TCRZE_2015_D_36_4&limit=1000&start=0',
            title: "Nivel de actividad y tipo de cambio real",
            source: "Fuente: Instituto Nacional de Estadística y Censos (INDEC)",
            chartTypes: { '143.3_NO_PR_2004_A_21': 'column' },
            navigator: true
        })

        TSComponents.Graphic.render('emae-graphic-without-filters', {
            graphicUrl: 'https://apis.datos.gob.ar/series/api/series/?metadata=full&ids=11.3_VMATC_2004_M_12:percent_change_a_year_ago,143.3_NO_PR_2004_A_21:percent_change_a_year_ago&limit=1000&start=0&format=json',
            chartOptions: { // Override highstock configs. See https://api.highcharts.com/highstock/
            },
            source: "Fuente: Instituto Nacional de Estadística y Censos (INDEC)",
            datePickerEnabled: false,
            navigator: false,
            title: "Estimador Mensual de Actividad Económica (EMAE)",
            chartTypes: { '11.3_VMATC_2004_M_12': 'area', '143.3_NO_PR_2004_A_21': 'area' },
            legendLabel: { '11.3_VMATC_2004_M_12': "Construcción", '143.3_NO_PR_2004_A_21': "Nivel general" }
        })

        TSComponents.Graphic.render('ica-graphic-without-filters', {
            graphicUrl: 'https://apis.datos.gob.ar/series/api/series/?ids=74.3_IET_0_M_16,74.3_IIT_0_M_25,74.3_ISC_0_M_19&collapse=year&collapse_aggregation=sum',
            chartTypes: { '74.3_IET_0_M_16': 'line', '74.3_IIT_0_M_25': 'line', '74.3_ISC_0_M_19': 'column' },
            title: "Intercambio Comercial Argentino (ICA)",
            navigator: false,
            datePickerEnabled: false,
            source: "Fuente: Instituto Nacional de Estadística y Censos (INDEC)",
        })

        TSComponents.Graphic.render('ipc-graphic-min', {
            graphicUrl: 'https://apis.datos.gob.ar/series/api/series/?ids=148.3_INIVELNAL_DICI_M_26:percent_change_a_year_ago',
            navigator: false,
            datePickerEnabled: false,
            title: "Inflación interanual (nivel general)"
        })

        TSComponents.Graphic.render('rem-graphic-min', {
            graphicUrl: 'https://apis.datos.gob.ar/series/api/series/?ids=430.1_MEDIANA_IP_12_M_0_0_27_96',
            navigator: false,
            datePickerEnabled: false,
            title: "REM mediana de expectativas de inflación a 12 meses"
        })

        TSComponents.Graphic.render('tcbna-graphic-min', {
            graphicUrl: 'https://apis.datos.gob.ar/series/api/series/?ids=168.1_T_CAMBIOR_D_0_0_26',
            navigator: false,
            datePickerEnabled: false,
            title: "Tipo de Cambio Vendedor (BNA)"
        })


    }
</script>
