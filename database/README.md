# Database 
## Online preview / Previsualización online
https://dbdiagram.io/d/APPs-1-gym-68b30569777b52b76c49f0ee

## Offline preview / Previsualización offline
### English
Just take a look at Diagram.pdf, it is the same as the online preview. If needed, you also could check all relationships here. 

### Español
Revisa Diagram.pdf, es lo mismo que la preview online. En caso de ser necesario, acá también podes ver todas las relaciones.

## Relationships / Relaciones: 
### English
- users table with:
    - user_information: **1 -> 1**
    - user_permissions: **1 -> N**
    - subscriptions: **1 -> 1**
    - otp_tokens: **1 -> 1** (if expired or used, it deletes by itself)
    - classes: **1 -> N** (as professor)
    - class_participants: **1 -> N** (as participant)
    - class_review: **1 -> N** (as reviewer)
    - locations: **1 -> N** (as owner)
- subscriptions table with:
    - subscriptions_information: **1 -> N**
- classes table with:
    - class_participants: **1 -> N**
    - class_review: **1 -> N**

### Español
- la tabla "users" con:
    - user_information: **1 -> 1**
    - user_permissions: **1 -> N**
    - subscriptions: **1 -> 1**
    - otp_tokens: **1 -> 1** (si expiró o se usó, se elimina el registro)
    - classes: **1 -> N** (identificado como "professor")
    - class_participants: **1 -> N** (identificado como "participant")
    - class_review: **1 -> N** (identificado como "reviewer")
    - locations: **1 -> N** (identificado como "owner")
- la tabla "subscriptions" con:
    - subscriptions_information: **1 -> N**
- la tabla "classes" con:
    - class_participants: **1 -> N**
    - class_review: **1 -> N**