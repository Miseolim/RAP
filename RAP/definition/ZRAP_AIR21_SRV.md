```abap
  @EndUserText.label: 'RAP Airline join OData service'

define service ZRAP_AIR21_SRV {  

  expose ZCDS_PROJ_JOIN_AIR21         as AirJoin;  
  expose ZCDS_PROJ_SFLSBO_JOIN_AIR21  as SpfliSbookJoin;  

};
