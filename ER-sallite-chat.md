```mermaid
erDiagram
USERS ||--o{  MESSAGES:allows
  USERS {
    int id PK
    string name
    string Email UK
    string img
    timestamp created_at
    timestamp deleted_at
  }

  MESSAGES{
    message_id id PK
    string message
    timestamp created_at
    boolian delete_flag
  }


```
