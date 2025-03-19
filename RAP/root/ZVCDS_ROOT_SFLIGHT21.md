```abap
@AccessControl.authorizationCheck: #NOT_REQUIRED
@EndUserText.label: 'RAP SFLIGHT root view'
@Metadata.ignorePropagatedAnnotations: true

define root view entity ZVCDS_ROOT_SFLIGHT21  
  as select from sflight {  

    key carrid   as Carrid,  
        connid   as Connid,  
        fldate   as Fldate,  

    @Semantics.amount.currencyCode: 'Currency'  
        price    as Price,  

        currency as Currency  

  };
