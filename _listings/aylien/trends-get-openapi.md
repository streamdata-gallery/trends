---
swagger: "2.0"
x-collection-name: Aylien
x-complete: 0
info:
  title: Aylien List trends
  description: The trends endpoint allows you to identify the most-mentioned entities,
    concepts and keywords relevant to your query. For example, this endpoint allows
    you to set parameters like a time period, a subject category, or an entity, and
    your request will return the most mentioned entities or keywords that are mentioned
    in relation to your query.
  termsOfService: https://newsapi.aylien.com/tos
  contact:
    name: API support
    url: https://newsapi.aylien.com/
    email: support@aylien.com
  version: 1.0.0
host: api.newsapi.aylien.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /trends:
    get:
      summary: List trends
      description: The trends endpoint allows you to identify the most-mentioned entities,
        concepts and keywords relevant to your query. For example, this endpoint allows
        you to set parameters like a time period, a subject category, or an entity,
        and your request will return the most mentioned entities or keywords that
        are mentioned in relation to your query.
      operationId: listTrends
      x-api-path-slug: trends-get
      parameters:
      - in: query
        name: No Name
      responses:
        100:
          description: Invalid API Key - The API key passed was not valid or has expired
        105:
          description: Service currently unavailable - The requested service is temporarily
            unavailable
        106:
          description: Write operation failed - The requested operation failed due
            to a temporary issue
        111:
          description: Format "xxx" not found - The requested response format was
            not found
        112:
          description: Method "xxx" not found - The requested method was not found
        114:
          description: Invalid SOAP envelope - The SOAP envelope send in the request
            could not be parsed
        115:
          description: Invalid XML-RPC Method Call - The XML-RPC request document
            could not be parsed
        116:
          description: Bad URL found - One or more arguments contained a URL that
            has been used for abuse on Flickr
        200:
          description: OK
      tags:
      - News
      - List
      - Trends
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