```abap
@AccessControl.authorizationCheck: #NOT_REQUIRED
@EndUserText.label: 'RAP mara root view'
@Metadata.ignorePropagatedAnnotations: true
@Metadata.allowExtensions: true

define root view entity ZVCDS_ROOT_DOCU21 
  as select from zcl1docu21 {
    
    key matnr as Matnr,
    key werks as Werks,
    key lgort as Lgort,

    mtart as Mtart,
    matkl as Matkl,

    @Semantics.quantity.unitOfMeasure: 'Meins'
    menge as Menge,

    meins as Meins,

    @Semantics.amount.currencyCode: 'Waers'
    wrbtr as Wrbtr,

    waers as Waers,
    lvorm as Lvorm

  }
