# sprinSecurityOAuth2MTPE
springSecurityOAuth2MTPE

Con esta prueba, se demuestra la viabilidad técnica para la generación de tokens (autenticación) y la autorización de acceso a recursos (Servicios API REST) con Spring Security y OAuth2 en un mismo contexto de aplicación.

PROCEDIMIENTO PARA REALIZAR LAS PRUEBAS:
1) OBTENER TOKEN
POST  http://localhost:8080/SpringSecurityOAuth2/oauth/token?grant_type=password&username=bill&password=abc123

EN HEADERS TIPO AUTORIZACION
Authorization Basic bXktdHJ1c3RlZC1jbGllbnQ6c2VjcmV0

2) USAR SERVICIOS API REST CON TOKEN
GET http://localhost:8080/SpringSecurityOAuth2/user/?access_token=<token generado>
