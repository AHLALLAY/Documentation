# 🌐 Codes de statut HTTP et leur implémentation en PHP

## ✅ 2xx - Codes de succès

| Code HTTP🔍 | Rôle💻 | Exemple de code PHP |
|-------------|--------|---------------------|
| 200 ⭐       | OK - Requête traitée avec succès | `http_response_code(200);` |
| 201 ➕       | Created - Ressource créée avec succès | `http_response_code(201);` |
| 202 ⏳       | Accepted - Requête acceptée pour traitement | `http_response_code(202);` |
| 204 📭       | No Content - Requête traitée mais pas de contenu à renvoyer | `http_response_code(204);` |

## 🔄 3xx - Codes de redirection

| Code HTTP🔍 | Rôle💻 | Exemple de code PHP |
|-------------|--------|---------------------|
| 301 🏃       | Moved Permanently - Redirection permanente | `header("Location: http://example.com", true, 301);` |
| 302 🔀       | Found - Redirection temporaire | `header("Location: http://example.com", true, 302);` |
| 304 📋       | Not Modified - Contenu non modifié depuis la dernière requête | `http_response_code(304);` |
| 307 ↪️       | Temporary Redirect - Redirection temporaire (préserve la méthode HTTP) | `header("Location: http://example.com", true, 307);` |

## ⚠️ 4xx - Erreurs client

| Code HTTP🔍 | Rôle💻 | Exemple de code PHP |
|-------------|--------|---------------------|
| 400 ❌       | Bad Request - Requête mal formée | `http_response_code(400);` |
| 401 🔒       | Unauthorized - Authentification nécessaire | `http_response_code(401);` |
| 403 🚫       | Forbidden - Accès interdit | `http_response_code(403);` |
| 404 🔍       | Not Found - Ressource non trouvée | `http_response_code(404);` |
| 429 🚦       | Too Many Requests - Trop de requêtes | `http_response_code(429);` |

## 🛑 5xx - Erreurs serveur

| Code HTTP🔍 | Rôle💻 | Exemple de code PHP |
|-------------|--------|---------------------|
| 500 💥       | Internal Server Error - Erreur interne du serveur | `http_response_code(500);` |
| 502 🌐       | Bad Gateway - Erreur de la passerelle | `http_response_code(502);` |
| 503 🔧       | Service Unavailable - Service temporairement indisponible | `http_response_code(503);` |
| 504 ⏰       | Gateway Timeout - Délai d'attente dépassé | `http_response_code(504);` |