# App Comparison

| URL Shortener                          | Your Project
| -----------------------------------    | ------------------------------------
| **Backend**                            | **Backend**
| - Django                               | - Django
| - Django Rest                          | - Django Rest
| - React                                | - React
|                                        |
| **Models**                             | **Model**
| - Users (built in)                     | - Users (built in)
| - URLs (user submitted data)           | - Posts/Shows/Parts/Cigars (user submitted data)
|                                        |
| **View**                               | **View**
| - Tokens                               | - Tokens
| - Logout                               | - Logout
| - Viewset for User Submitted Data      | - Viewset for User Submitted Data
|                                        |
| **Serializers (returns JSON)**         | **Serializers (returns JSON)**
| - Token                                | - Token
| - URLs                                 | - Posts/Shows/Parts/Cigars
|                                        |
| **URLs (aka "routes")**                | **URLs**
| - `/token` (login)                     | - `/token` (login)
| - `/logout` (logout)                   | - `/logout` (logout)
| - `/urls` (show all posts)             | - `/[user data]/[id of single item]` (show all items or single item)
| - `/snd/[variable]` (trigger shortener)|
|                                        |
| **Frontend**                           | **Frontend**
|                                        |
| `<form method=POST>`                   | `<form method=POST>`
| - Submit request to API                | - Submit request to API
| - Send To -> API Route                 | - Send To -> API Route
| - `POST` triggers call to Model        | -`POST` triggers call to Model
| - Model updates DB, new entry made     | - Model updates DB, new entry made
