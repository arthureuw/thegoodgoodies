> Entité : Restaurant

| Champ | Type | Commentaires |
|---|---|---|
| id | integer | Clé primaire |
| name | string | |
| created | date | Date de création de l'enregistrement, renseignée automatiquement à la création de l'enregistrement |
| rate | integer | Note sur 5 |
| menus | **Relation** | menus dans le restaurant |
| plats | **Relation** | plats dans le restaurant |

> Entité : Menu

| Champ | Type | Commentaires |
|---|---|---|
| id | integer | Clé primaire |
| name | string | |
| price | integer | Prix du Menu |
| plats | **Relation** | Listes des plats dans le menu |
| restaurant | **Relation** | Restaurant contenant le menu |

> Entité : Plat

| Champ | Type | Commentaires |
|---|---|---|
| id | integer | Clé primaire |
| name | string | |
| price | integer | Prix du plat | 
| restaurant | **Relation** | restaurant du plat |

> User : User

- Id
- Email
- LastName
- Firstname
- Password
- Created date
- Last Connection
