```abap
managed; // Implementation in class zbp_vcds_root_docu21
unique;

define behavior for ZVCDS_ROOT_DOCU21 
// alias <alias_name> 
persistent table zcl1docu21
lock master {

  create;
  update;
  delete;

  // Field mapping
  mapping for zcl1docu21 corresponding {
    Matnr = matnr;
    Werks = werks;
    Lgort = lgort;
    Mtart = mtart;
    Matkl = matkl;
    Menge = menge;
    Meins = meins;
    Wrbtr = wrbtr;
    Waers = waers;
    Lvorm = lvorm;
  }

}
