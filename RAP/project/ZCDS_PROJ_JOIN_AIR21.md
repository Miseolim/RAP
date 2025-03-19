```abap
@AccessControl.authorizationCheck: #NOT_REQUIRED
@EndUserText.label: 'RAP JOIN_AIR projection view'
@Metadata.ignorePropagatedAnnotations: true

define root view entity ZCDS_PROJ_JOIN_AIR21  
  as projection on ZVCDS_ROOT_JOIN_AIR21 {  

    key Carrid,  
    key Connid,  

    Carrname,  
    Currcode,  
    Url,  

    Countryfr,  
    Cityfrom,  
    Airpfrom,  

    Countryto,  
    Cityto,  
    Airpto  

};
