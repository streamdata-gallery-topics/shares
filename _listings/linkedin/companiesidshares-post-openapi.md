---
swagger: "2.0"
x-collection-name: LinkedIn
x-complete: 0
info:
  title: LinkedIn Add Companies Shares
  description: Post companies  shares
  version: 1.0.0
host: api.linkedin.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /people/shares:
    post:
      summary: Add People ~ Shares
      description: Post people ~ shares
      operationId: postPeople~Shares
      x-api-path-slug: peopleshares-post
      parameters:
      - in: header
        name: Content-Type
        description: The content type
      - in: query
        name: format
        description: The message format
        type: string
        format: string
      - in: header
        name: x-li-format
        description: The content type
      responses:
        200:
          description: OK
      tags:
      - People
      - Shares
  /companies/{id}/shares:
    post:
      summary: Add Companies Shares
      description: Post companies  shares
      operationId: postCompaniesShares
      x-api-path-slug: companiesidshares-post
      parameters:
      - in: query
        name: format
        description: The message format
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Companies
      - ""
      - Shares
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