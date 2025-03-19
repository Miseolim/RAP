```abap
@AccessControl.authorizationCheck: #NOT_REQUIRED
@EndUserText.label: 'RAP SBOOK root view'
@Metadata.ignorePropagatedAnnotations: true

define root view entity ZVCDS_ROOT_SBOOK21  
  as select from sbook {  

    key carrid   as Carrid,  
    key connid   as Connid,  
    key fldate   as Fldate,  
    key bookid   as Bookid,  

        customid  as Customid,  
        custtype  as Custtype,  
        smoker    as Smoker  

  };
