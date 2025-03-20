```abap
@Metadata.layer: #CORE
@UI: {    
    headerInfo: {    
        typeName: 'AirlineInfo',    
        typeNamePlural: 'Airline master',    
        title: { value: 'AirlineData' },    
        description: { value: 'AirlineMaster' }    
    }    
}  

annotate view ZVCDS_PROJ_SCARR21 with {    

    @UI.facet: [    
        {    
            id: 'AirlineInfo',    
            purpose: #STANDARD,    
            type: #IDENTIFICATION_REFERENCE,    
            label: 'AirlineInfo',    
            position: 10    
        }    
    ]    

    // Airline Code    
    @UI: {    
        lineItem: [ { position: 10, label: 'Airline Code', importance: #HIGH } ],    
        identification: [ { position: 10, label: '항공사코드', importance: #HIGH } ]    
    }    
    Carrid;    

    // Airline Name    
    @UI: {    
        lineItem: [ { position: 10, label: 'Airline Name', importance: #HIGH } ],    
        identification: [ { position: 10, label: '항공사이름', importance: #HIGH } ]    
    }    
    Carrname;    

    // Airline Currency    
    @UI: {    
        lineItem: [ { position: 10, label: 'Airline Currency', importance: #HIGH } ],    
        identification: [ { position: 10, label: '항공사 통화키', importance: #HIGH } ]    
    }    
    Currcode;    

    // Airline URL    
    @UI: {    
        lineItem: [ { position: 10, label: 'Airline URL', importance: #HIGH } ],    
        identification: [ { position: 10, label: 'Homepage URL', importance: #HIGH } ]    
    }    
    Url;    

}
