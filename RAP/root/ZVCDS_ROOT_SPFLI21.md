```abap
@AccessControl.authorizationCheck: #NOT_REQUIRED
@EndUserText.label: 'RAP SCHEDULE root view'
@Metadata.ignorePropagatedAnnotations: true

define root view entity ZVCDS_ROOT_SPFLI21  
  as select from spfli {  
      
    key carrid    as Carrid,  
    key connid    as Connid,  
      
    countryfr     as Countryfr,  
    cityfrom      as Cityfrom,  
    airpfrom      as Airpfrom,  
    
    countryto     as Countryto,  
    cityto        as Cityto,  
    airpto        as Airpto  
      
};
