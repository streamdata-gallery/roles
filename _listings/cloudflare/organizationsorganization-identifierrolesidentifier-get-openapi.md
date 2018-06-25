---
swagger: "2.0"
x-collection-name: CloudFlare
x-complete: 0
info:
  title: CloudFlare Get information about a specific role for an organization
  version: 1.0.0
  description: Get information about a specific role for an organization
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizations/:organization_identifier/roles:
    get:
      summary: Get all available roles for an organization
      description: Get all available roles for an organization
      operationId: cloudflare-organization-roles-api
      x-api-path-slug: organizationsorganization-identifierroles-get
      responses:
        200:
          description: OK
      tags:
      - Organization Roles
  /organizations/:organization_identifier/roles/:identifier:
    get:
      summary: Get information about a specific role for an organization
      description: Get information about a specific role for an organization
      operationId: cloudflare-organization-roles-api
      x-api-path-slug: organizationsorganization-identifierrolesidentifier-get
      responses:
        200:
          description: OK
      tags:
      - Organization Roles
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---