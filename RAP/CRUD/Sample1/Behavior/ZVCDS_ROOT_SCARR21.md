```abap
managed; // Implementation in class zbp_vcds_root_scarr21
unique;

define behavior for ZVCDS_ROOT_SCARR21 
// alias <alias_name> 
persistent table zcl1scarr21
lock master {

    create;
    update;
    delete;

    // Field mapping
    mapping for zcl1scarr21 corresponding {
        Carrid   = carrid;
        Carrname = carrname;
        Currcode = currcode;
        Url      = url;
    }

}
