---
swagger: "2.0"
x-collection-name: NxtPort
x-complete: 0
info:
  title: NxtPort UN Location Codes API Get Locations Latitude Longitude Radius
  description: This api will return locations in a certain radius of a point, ordered
    by distance , not necessarily in the same country
  version: 1.0.0
host: api.nxtport.eu
basePath: /unlocodes/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /locations/{latitude}/{longitude}/{radius}:
    get:
      summary: Get Locations Latitude Longitude Radius
      description: This api will return locations in a certain radius of a point,
        ordered by distance , not necessarily in the same country
      operationId: locations_getinNeighbourhood
      x-api-path-slug: locationslatitudelongituderadius-get
      parameters:
      - in: path
        name: latitude
        description: the latitude of the specified point
      - in: path
        name: longitude
        description: the longitude of the specified point
      - in: query
        name: page
        description: the page number to allow paging (needs to be an integer > 0)
      - in: path
        name: radius
        description: the radius in km (max 75km)
      - in: query
        name: size
        description: the page size to allow paging (needs to be an integer 0 < pagesize
          < 1000)
      responses:
        200:
          description: OK
      tags:
      - Locations
      - Latitude
      - Longitude
      - Radius
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