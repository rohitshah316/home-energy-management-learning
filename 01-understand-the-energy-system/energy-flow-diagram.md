
flowchart TD
    SOLAR["☀️ Solar Panels"]
    BATTERY["🔋 Home Battery"]
    HOME["🏠 Home"]
    GRID["⚡ Electricity Grid"]
    HEAT["🌡️ Heat Pump"]
    EV["🚗 EV Charger"]
    EMS["🧠 Energy Management System"]

    SOLAR --> HOME
    SOLAR <--> BATTERY
    SOLAR <--> GRID
    BATTERY <--> HOME
    GRID <--> HOME

    HOME --> HEAT
    HOME --> EV

    EMS -.-> SOLAR
    EMS -.-> BATTERY
    EMS -.-> HEAT
    EMS -.-> EV
    EMS -.-> GRID
