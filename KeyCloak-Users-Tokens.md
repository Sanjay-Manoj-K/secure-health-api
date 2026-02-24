https://slproweb.com/products.html



---



openssl req -x509 -newkey rsa:4096 -keyout certs/server.key -out certs/server.crt -days 365 -nodes -subj "/CN=localhost"



---



curl -X POST http://localhost:8080/realms/health/protocol/openid-connect/token ^

  -H "Content-Type: application/x-www-form-urlencoded" ^

  -d "client\_id=helth-api" ^

  -d "username=Don" ^

  -d "password=don123" ^

  -d "grant\_type=password"



**---------------------------------------------------------------------------------------------------------------------------------**

***Access token for Sanjay***

**---------------------------------------------------------------------------------------------------------------------------------**



**eyJhbGciOiJSUzI1NiIsInR5cCIgOiAiSldUIiwia2lkIiA6ICJ5MC1IQ0RmWUFyalhsd1dxTE9kckRQWFFkUjRTY3NoSF9FbExQaFotZUdnIn0.eyJleHAiOjE3NzA4OTIzMjUsImlhdCI6MTc3MDg5MjAyNSwianRpIjoiYWZiZTU0OGYtYWI2Zi00ZmU4LWJkNDEtMDRmMmQ2OTAwYWJkIiwiaXNzIjoiaHR0cDovL2xvY2FsaG9zdDo4MDgwL3JlYWxtcy9oZWFsdGgiLCJhdWQiOiJhY2NvdW50Iiwic3ViIjoiMDNlZjU2NDEtYjlkMi00MGEyLTkyY2MtMWY0ZjY0ZmU0ZTRiIiwidHlwIjoiQmVhcmVyIiwiYXpwIjoiaGVsdGgtYXBpIiwic2Vzc2lvbl9zdGF0ZSI6ImFlNDlmMGI3LTZjMDctNDZiMi05MDQ0LTA1ZWI0NjZkMWIzZSIsImFjciI6IjEiLCJhbGxvd2VkLW9yaWdpbnMiOlsiaHR0cHM6Ly9sb2NhbGhvc3Q6ODQ0MyJdLCJyZWFsbV9hY2Nlc3MiOnsicm9sZXMiOlsiZWRpdG9yIiwib2ZmbGluZV9hY2Nlc3MiLCJ1bWFfYXV0aG9yaXphdGlvbiIsImRlZmF1bHQtcm9sZXMtaGVhbHRoIl19LCJyZXNvdXJjZV9hY2Nlc3MiOnsiYWNjb3VudCI6eyJyb2xlcyI6WyJtYW5hZ2UtYWNjb3VudCIsIm1hbmFnZS1hY2NvdW50LWxpbmtzIiwidmlldy1wcm9maWxlIl19fSwic2NvcGUiOiJlbWFpbCBwcm9maWxlIiwic2lkIjoiYWU0OWYwYjctNmMwNy00NmIyLTkwNDQtMDVlYjQ2NmQxYjNlIiwiZW1haWxfdmVyaWZpZWQiOnRydWUsIm5hbWUiOiJTYW5qYXkgTWFub2oiLCJwcmVmZXJyZWRfdXNlcm5hbWUiOiJzYW5qYXkiLCJnaXZlbl9uYW1lIjoiU2FuamF5IiwiZmFtaWx5X25hbWUiOiJNYW5vaiIsImVtYWlsIjoic2FuamF5bWFub2prQGdtYWlsLmNvbSJ9.wYTb2cU0xXn6tOidAQNowhrYKXmStwHTzwbhkLh2XdHly9X\_O7G-dBoDmJA7N8MUhF7i1ZeYczQ\_WcUpNi3xZ4A9\_sXz9LuWuDT11IVIGRaLt2U1gWO2iVL\_oufy4wC241Fr\_TX1WoGK5CMFIeiMYwJtrpby5jfpE7dpA00jDB4r1kH2svNJG1IOSxfO87Wdka4-FZbysK-RfOIoLnuVyuJi6Q6bW\_ddvctOkINr0hLSGGqMndjgRJhGlg76IsdrfmnROE6OD1aS5QbIeUttbwScr20-yUL48Oigl4yLGlbeLdKbc-UjL\_y6aOLdKISRyUSY5OqBtPsKFLQ3b3NPHg**



**-------------------------------------------------------------------------------------------------------------------------------------**

***Access token for Don***

**-------------------------------------------------------------------------------------------------------------------------------------**



**eyJhbGciOiJSUzI1NiIsInR5cCIgOiAiSldUIiwia2lkIiA6ICJ5MC1IQ0RmWUFyalhsd1dxTE9kckRQWFFkUjRTY3NoSF9FbExQaFotZUdnIn0.eyJleHAiOjE3NzA4OTI4NzIsImlhdCI6MTc3MDg5MjU3MiwianRpIjoiOGIwOTMwNWItMzk3NC00NmJkLWJhMmItNTAxMDI1ZGYzMGVjIiwiaXNzIjoiaHR0cDovL2xvY2FsaG9zdDo4MDgwL3JlYWxtcy9oZWFsdGgiLCJhdWQiOiJhY2NvdW50Iiwic3ViIjoiNzM1ZGU5ZWMtNjIyMS00MmFiLThkOWQtOWI0MmY3NGMwNjMwIiwidHlwIjoiQmVhcmVyIiwiYXpwIjoiaGVsdGgtYXBpIiwic2Vzc2lvbl9zdGF0ZSI6IjRjNmVhYTdkLTQ3NjAtNGUyNi04YmUyLTY4NzRhZGE5YWUxNiIsImFjciI6IjEiLCJhbGxvd2VkLW9yaWdpbnMiOlsiaHR0cHM6Ly9sb2NhbGhvc3Q6ODQ0MyJdLCJyZWFsbV9hY2Nlc3MiOnsicm9sZXMiOlsib2ZmbGluZV9hY2Nlc3MiLCJWaWV3ZXIiLCJ1bWFfYXV0aG9yaXphdGlvbiIsImRlZmF1bHQtcm9sZXMtaGVhbHRoIl19LCJyZXNvdXJjZV9hY2Nlc3MiOnsiYWNjb3VudCI6eyJyb2xlcyI6WyJtYW5hZ2UtYWNjb3VudCIsIm1hbmFnZS1hY2NvdW50LWxpbmtzIiwidmlldy1wcm9maWxlIl19fSwic2NvcGUiOiJlbWFpbCBwcm9maWxlIiwic2lkIjoiNGM2ZWFhN2QtNDc2MC00ZTI2LThiZTItNjg3NGFkYTlhZTE2IiwiZW1haWxfdmVyaWZpZWQiOnRydWUsIm5hbWUiOiJEb24gU2FiYXN0aWFuIiwicHJlZmVycmVkX3VzZXJuYW1lIjoiZG9uIiwiZ2l2ZW5fbmFtZSI6IkRvbiIsImZhbWlseV9uYW1lIjoiU2FiYXN0aWFuIiwiZW1haWwiOiJkb25zYWJhc3RpYW5AZ21haWwuY29tIn0.X6jKERSrQvvVLUemrYkPgYPV7VczrzBseStHAg8E6GVmq2KLeYnVmmosyXjHBZ2JQ3Mr4dEVU63Cwav-Op2Ji1DeSZfGPl70naWuAh416N0losH7EtB9ke\_BMO68YbCc9T4ybzhzxNo8XLAjXEY-N\_r5fMqhkZOpGt5UY1tuFOwdCn-wm4CpJT5SWR6CzvXED4Nn1wHuJZfqBej9iAj3TdEBST-jbCW3dVh3owncrvfdsoFqs2DDLwqCoDmKmg0zN8vBOl3Cpgu8cgXwD4IjQpMgqT7nX1CkADyNqki3plv8eRxL1O5mFgxp416ec-f01N1HvaYF3uCGQlpxzryobw**





**--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------**

**GET without the token**

curl -k https://localhost:8443/records/123"



**GET with invalid token**

curl -k https://localhost:8443/records/123 ^

  -H "Authorization: Bearer invalidtoken"



**GET with valid viewer Token**

curl -k https://localhost:8443/records/123 ^

  -H "Authorization: Bearer eyJhbGciOiJSUzI1NiIsInR5cCIgOiAiSldUIiwia2lkIiA6ICJ4OU1oRF9weUNmX3MyZ0tTaW9KWHdyTGtvNXBSNVpMYzVWTUo3Z09RUWlJIn0.eyJleHAiOjE3Njk0ODk5NzUsImlhdCI6MTc2OTQ4OTY3NSwianRpIjoiMjA2MmE1MDUtNjViMC00Mjc0LWFiNGEtNmJhZjUwZDQ0ODExIiwiaXNzIjoiaHR0cDovL2xvY2FsaG9zdDo4MDgwL3JlYWxtcy9oZWFsdGgiLCJhdWQiOiJhY2NvdW50Iiwic3ViIjoiZTI3OWQ2NzQtODkwMC00YWFlLTg4MjgtODRiYzYxZTZiZWYyIiwidHlwIjoiQmVhcmVyIiwiYXpwIjoiaGVhbHRoLWFwaSIsInNlc3Npb25fc3RhdGUiOiJiNjc3YjVkYi1kZTc3LTQwZGYtYjY4YS0yMDhlM2FmZDRkNjYiLCJhY3IiOiIxIiwiYWxsb3dlZC1vcmlnaW5zIjpbImh0dHBzOi8vbG9jYWxob3N0Ojg0NDMiXSwicmVhbG1fYWNjZXNzIjp7InJvbGVzIjpbInZpZXdlciIsIm9mZmxpbmVfYWNjZXNzIiwidW1hX2F1dGhvcml6YXRpb24iLCJkZWZhdWx0LXJvbGVzLWhlYWx0aCJdfSwicmVzb3VyY2VfYWNjZXNzIjp7ImFjY291bnQiOnsicm9sZXMiOlsibWFuYWdlLWFjY291bnQiLCJtYW5hZ2UtYWNjb3VudC1saW5rcyIsInZpZXctcHJvZmlsZSJdfX0sInNjb3BlIjoiZW1haWwgcHJvZmlsZSIsInNpZCI6ImI2NzdiNWRiLWRlNzctNDBkZi1iNjhhLTIwOGUzYWZkNGQ2NiIsImVtYWlsX3ZlcmlmaWVkIjp0cnVlLCJwcmVmZXJyZWRfdXNlcm5hbWUiOiJqb2huIiwiZW1haWwiOiJqb2hudHN0QGdtYWlsLmNvbSJ9.JSG3\_lpBKcOUWdwP1icaIAgERnhExvg-IrFkMU90V8OpwEY2BtArRrSM2Z1cKPm9xnn8or5hkf9lVnNnhOiuUrR93dziU4YsFpt65DL2IF8ja9kpl-QCXcMuuGhp-3wHnEF8V7y9ylPsT\_YKpOHjKhPc-B52SDgt8vE2Ec65jx950ftXf7qddFpNDP8phqffXC7jX1GNo3vo4Uqf32UpXdIR03pzPuTQ\_MkRg2LiUbihHzqq9X0LL9XBsNPAnWek6y3Vw8IYCammgj1UcmbxGi2N4iuEau037Blr7b95soDpI47ySOIhYEORTxdREQjwM03gq9Z5KWMCXH8Q30mNYg"









curl -k https://localhost:8443/records ^

&nbsp; -H "Authorization: Bearer eyJhbGciOiJSUzI1NiIsInR5cCIgOiAiSldUIiwia2lkIiA6ICJ5MC1IQ0RmWUFyalhsd1dxTE9kckRQWFFkUjRTY3NoSF9FbExQaFotZUdnIn0.eyJleHAiOjE3NzA4OTI4NzIsImlhdCI6MTc3MDg5MjU3MiwianRpIjoiOGIwOTMwNWItMzk3NC00NmJkLWJhMmItNTAxMDI1ZGYzMGVjIiwiaXNzIjoiaHR0cDovL2xvY2FsaG9zdDo4MDgwL3JlYWxtcy9oZWFsdGgiLCJhdWQiOiJhY2NvdW50Iiwic3ViIjoiNzM1ZGU5ZWMtNjIyMS00MmFiLThkOWQtOWI0MmY3NGMwNjMwIiwidHlwIjoiQmVhcmVyIiwiYXpwIjoiaGVsdGgtYXBpIiwic2Vzc2lvbl9zdGF0ZSI6IjRjNmVhYTdkLTQ3NjAtNGUyNi04YmUyLTY4NzRhZGE5YWUxNiIsImFjciI6IjEiLCJhbGxvd2VkLW9yaWdpbnMiOlsiaHR0cHM6Ly9sb2NhbGhvc3Q6ODQ0MyJdLCJyZWFsbV9hY2Nlc3MiOnsicm9sZXMiOlsib2ZmbGluZV9hY2Nlc3MiLCJWaWV3ZXIiLCJ1bWFfYXV0aG9yaXphdGlvbiIsImRlZmF1bHQtcm9sZXMtaGVhbHRoIl19LCJyZXNvdXJjZV9hY2Nlc3MiOnsiYWNjb3VudCI6eyJyb2xlcyI6WyJtYW5hZ2UtYWNjb3VudCIsIm1hbmFnZS1hY2NvdW50LWxpbmtzIiwidmlldy1wcm9maWxlIl19fSwic2NvcGUiOiJlbWFpbCBwcm9maWxlIiwic2lkIjoiNGM2ZWFhN2QtNDc2MC00ZTI2LThiZTItNjg3NGFkYTlhZTE2IiwiZW1haWxfdmVyaWZpZWQiOnRydWUsIm5hbWUiOiJEb24gU2FiYXN0aWFuIiwicHJlZmVycmVkX3VzZXJuYW1lIjoiZG9uIiwiZ2l2ZW5fbmFtZSI6IkRvbiIsImZhbWlseV9uYW1lIjoiU2FiYXN0aWFuIiwiZW1haWwiOiJkb25zYWJhc3RpYW5AZ21haWwuY29tIn0.X6jKERSrQvvVLUemrYkPgYPV7VczrzBseStHAg8E6GVmq2KLeYnVmmosyXjHBZ2JQ3Mr4dEVU63Cwav-Op2Ji1DeSZfGPl70naWuAh416N0losH7EtB9ke\_BMO68YbCc9T4ybzhzxNo8XLAjXEY-N\_r5fMqhkZOpGt5UY1tuFOwdCn-wm4CpJT5SWR6CzvXED4Nn1wHuJZfqBej9iAj3TdEBST-jbCW3dVh3owncrvfdsoFqs2DDLwqCoDmKmg0zN8vBOl3Cpgu8cgXwD4IjQpMgqT7nX1CkADyNqki3plv8eRxL1O5mFgxp416ec-f01N1HvaYF3uCGQlpxzryobw

" ^

&nbsp; -H "Content-Type: application/json" ^

&nbsp; -d "{ \\"patient\_id\\": \\"patient456\\", \\"name\\": \\"John Doe\\",  \\"age\\": 45, \\"diagnosis\\": \\"Diabetes\\" }"

