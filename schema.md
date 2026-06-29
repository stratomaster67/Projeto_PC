Estrutura de Dados e Contratos de Dados

1. Objeto Componente (`Component`)
Representa uma peça inserida no setup do usuário e salva no `localStorage` sob a chave `setup_manager_data`.

```json
{
  "id": "String (UUID v4)",
  "name": "String",
  "category": "String (GPU | CPU | PSU | MOBO | RAM | STORAGE | COOLER)",
  "watts": "Number",
  "price": "Number",
  "createdAt": "Number (Timestamp)"
}