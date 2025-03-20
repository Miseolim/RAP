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
    menge as Menge, //수량

    meins as Meins, //(단위)

    @Semantics.amount.currencyCode: 'Waers' //통화 코드
    wrbtr as Wrbtr, //금액

    waers as Waers, 
    lvorm as Lvorm

  }
