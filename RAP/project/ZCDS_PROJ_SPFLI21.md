```abap
@AccessControl.authorizationCheck: #NOT_REQUIRED
@EndUserText.label: 'RAP Schedule projection view'
@Metadata.ignorePropagatedAnnotations: true

define root view entity ZCDS_PROJ_SPFLI21  
  as projection on ZVCDS_ROOT_SPFLI21 {  

    key Carrid,  
    key Connid,  

    Countryfr,  
    Cityfrom,  
    Airpfrom,  

    Countryto,  
    Cityto,  
    Airpto  

};
