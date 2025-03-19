```abap
@AccessControl.authorizationCheck: #NOT_REQUIRED
@EndUserText.label: 'RAP Airline join root view'
@Metadata.ignorePropagatedAnnotations: true

define root view entity ZVCDS_ROOT_JOIN_AIR21  
  as select from scarr as a  
  inner join spfli as b  
    on a.carrid = b.carrid  
  {  
    key a.carrid   as Carrid,  
    key b.connid   as Connid,  

        a.carrname  as Carrname,  
        a.currcode  as Currcode,  
        a.url       as Url,  

        b.countryfr as Countryfr,  
        b.cityfrom  as Cityfrom,  
        b.airpfrom  as Airpfrom,  

        b.countryto as Countryto,  
        b.cityto    as Cityto,  
        b.airpto    as Airpto  
  };
