---
swagger: "2.0"
x-collection-name: Apica
x-complete: 1
info:
  title: Roles API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  '/roles ':
    ' get ':
      summary: Get Roles
      description: Return user roles
      operationId: getRoles
      x-api-path-slug: roles-get
      responses:
        200:
          description: OK
      tags:
      - Roles
---