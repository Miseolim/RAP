```abap
@EndUserText.label: 'RAP Airline master OData service'

define service ZRAP_SCARR21_SRV {
    expose ZVCDS_PROJ_SCARR21 as Airline;
    expose ZCDS_PROJ_SPFLI21 as Schedule;
}
