# Architecture which can be implemented using serverless

1. Request-Response architecture
2. Event-drive architcture :
3. Microservice architecture
4. Batch processing archicture

Following are

client -> API -> Message Queue -> Processing -> Store
client -> File Store -> Processing -> Store

5. Stream processing architecture

Following are

client -> API -> Message Queue -> Processing -> Store
client -> File Store -> Trigger -> Store 6. Hybrid archticture

❌

| Architecture        | Server | serverless |
| :------------------ | :----: | :--------: |
| Request-Response    |   ✅   |     ✅     |
| Event-drive         |   ✅   |     ✅     |
| Microservice        |   ✅   |     ✅     |
| Batch processing    |   ✅   |     ❌     |
| Stream processing   |   ✅   |     ❌     |
| hybrid architecture |   ✅   |     ❌     |
