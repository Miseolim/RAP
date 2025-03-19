```abap
@AccessControl.authorizationCheck: #NOT_REQUIRED
@EndUserText.label: 'RAP SFLSBOJOIN_AIR projection view'
@Metadata.ignorePropagatedAnnotations: true

define root view entity ZCDS_PROJ_SFLSBO_JOIN_AIR21  
  as projection on ZVCDS_ROOT_SFLSBO_JOIN_AIR21 {  

    key Carrid,  
    key Connid,  
    key Fldate,  
    key Bookid,  

    Customid,  
    Custtype,  
    Smoker,  
    Invoice,  
    OrderDate,  
    Counter,  
    Agencynum,  
    Cancelled,  
    Reserved,  

    Passname,  
    Passform,  
    Passbirth  

};
