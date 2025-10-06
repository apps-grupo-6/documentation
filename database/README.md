## Relationships / Relaciones: 
### English
- users table with:
    - user_information: **1 -> 1**
    - user_roles: **1 -> N** (as "user_id")
    - user_controls: **1 -> 1**
    - subscriptions: **1 -> 1**
    - otp_tokens: **1 -> N** (if expired or used it deletes by itself, but an user can have differents otp_tokens type )
    - classes: **1 -> N** (as "professor_id")
    - class_participants: **1 -> N** (as "user_id")
    - class_review: **1 -> N** (as "user_id")
    - locations: **1 -> N** (as "owner_id")
    - requests: **1 -> N** (as "user_id")
- subscriptions table with:
    - subscriptions_information: **1 -> N** (as "subscription_id")
- classes table with:
    - class_participants: **1 -> N** (as "class_id")
    - class_review: **1 -> N** (as "class_id")
    - disciplines: **N -> 1** (as "discipline_id")
    - locations: **N -> 1** (as "locations_id")
- roles table with:
    - role_permissions: **1 -> N** (as "role_id")
    - user_roles: **1 -> N** (as "role_id")
  

### Español
- la tabla "users" con:
    - user_information: **1 -> 1**
    - user_roles: **1 -> N** (identificado como "user_id")
    - user_controls: **1 -> 1**
    - subscriptions: **1 -> 1**
    - otp_tokens: **1 -> 1** (si expira o se usa, se elimina automáticamente, pero un usuario puede tener diferentes tipos de otp_tokens)
    - classes: **1 -> N** (identificado como "professor_id")
    - class_participants: **1 -> N** (identificado como "user_id")
    - class_review: **1 -> N** (identificado como "user_id")
    - locations: **1 -> N** (identificado como "owner_id")
    - requests: **1 -> N** (identificado como "user_id")
- la tabla "subscriptions" con:
    - subscriptions_information: **1 -> N** (identificado como "subscription_id")
- la tabla "classes" con:
    - class_participants: **1 -> N** (identificado como "class_id")
    - class_review: **1 -> N** (identificado como "class_id")
    - disciplines: **N -> 1** (identificado como "discipline_id")
    - locations: **N -> 1** (identificado como "locations_id")
- roles table with:
    - role_permissions: **1 -> N** (identificado como "role_id")
    - user_roles: **1 -> N** (identificado como "role_id")
