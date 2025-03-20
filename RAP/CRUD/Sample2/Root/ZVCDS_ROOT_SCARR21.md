```abap
@AccessControl.authorizationCheck: #NOT_REQUIRED
@EndUserText.label: 'RAP Airline master root view'
@Metadata.ignorePropagatedAnnotations: true
@Metadata.allowExtensions: true 

define root view entity ZVCDS_ROOT_SCARR21 
  as select from zcl1scarr21 {
  
    key carrid   as Carrid,
        carrname as Carrname,
        currcode as Currcode,
        url      as Url

}

