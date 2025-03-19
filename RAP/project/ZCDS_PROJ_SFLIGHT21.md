```abap
@AccessControl.authorizationCheck: #NOT_REQUIRED
@EndUserText.label: 'RAP SFLIGHT projection view'
@Metadata.ignorePropagatedAnnotations: true

define root view entity ZCDS_PROJ_SFLIGHT21  
  as projection on ZVCDS_ROOT_SFLIGHT21 {  

    key Carrid,  
    Connid,  
    Fldate,  

    @Semantics.amount.currencyCode: 'Currency'  
    Price,  

    Currency  

};
