```abap
@EndUserText.label: 'RAP Material OData service'

define service ZRAP_MATERIAL_SRV {
    expose ZCDS_PROJ_DOCU21 as Material;
}
