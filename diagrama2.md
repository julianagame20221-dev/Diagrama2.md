``` mermaid
flowchart LR
    REP[Persona que reporta]
    TEC[Tecnico]
    UI[Interfaz web]
    MR[Modulo de reportes]
    ME[Modulo de equipos]
    MA[Modulo de atencion tecnica]
    BD[(Base de datos)]

    REP-->|registra dano| UI
    TEC-->|consulta pendientes| UI
    UI-->MR
    UI-->ME
    UI-->MA
    MR-->BD
    ME-->BD
    MA-->BD
```
