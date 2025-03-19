```abap
@AccessControl.authorizationCheck: #NOT_REQUIRED
@EndUserText.label: 'RAP sflight_sbook_join root view'
@Metadata.ignorePropagatedAnnotations: true

define root view entity ZVCDS_ROOT_SFLSBO_JOIN_AIR21  
  as select from sflight as a  
  inner join sbook as b  
    on a.carrid = b.carrid  
   and a.connid = b.connid  
   and a.fldate = b.fldate  
  {  
    key b.carrid     as Carrid,  
    key b.connid     as Connid,  
    key b.fldate     as Fldate,  
    key b.bookid     as Bookid,  

    b.customid       as Customid,  
    b.custtype       as Custtype,  
    b.smoker         as Smoker,  
    b.invoice        as Invoice,  
    b.order_date     as OrderDate,  
    b.counter        as Counter,  
    b.agencynum      as Agencynum,  
    b.cancelled      as Cancelled,  
    b.reserved       as Reserved,  

    b.passname       as Passname,  
    b.passform       as Passform,  
    b.passbirth      as Passbirth  
  };
