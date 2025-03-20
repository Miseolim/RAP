```abap
@AccessControl.authorizationCheck: #NOT_REQUIRED
@EndUserText.label: 'RAP Airline master projection view'
@Metadata.ignorePropagatedAnnotations: true
@Metadata.allowExtensions: true

define root view entity ZVCDS_PROJ_SCARR21 
  as projection on ZVCDS_ROOT_SCARR21 {

    key Carrid,
        Carrname,
        Currcode,
        Url

}
