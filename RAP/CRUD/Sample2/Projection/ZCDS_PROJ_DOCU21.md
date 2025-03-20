```abap
@AccessControl.authorizationCheck: #NOT_REQUIRED
@EndUserText.label: 'RAP DOCU projection view'
@Metadata.ignorePropagatedAnnotations: true
@Metadata.allowExtensions: true

define root view entity ZCDS_PROJ_DOCU21 
  as projection on ZVCDS_ROOT_DOCU21 {

    key Matnr,
    key Werks,
    key Lgort,

    Mtart,
    Matkl,

    Menge,
    Meins,

    Wrbtr,
    Waers,
    Lvorm

  }
