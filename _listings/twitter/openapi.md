swagger: "2.0"
x-collection-name: Twitter
x-complete: 1
info:
  title: Twitter
  description: the-twitter-api-gives-you-programmatic-control-over-any-twitter-account-and-most-aspect-of-the-platform--allowing-developers-to-build-social-applications-that-use-the-platform-and-automate-interactions-between-users-
  version: "1.1"
host: api.twitter.com
basePath: /1.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /application/rate_limit_status:
    get:
      summary: Get Rate Limit Sttaus
      description: Returns the current rate limits for methods belonging to the specified
        resource families
      operationId: returns-the-current-rate-limits-for-methods-belonging-to-the-specified-resource-families
      x-api-path-slug: applicationrate-limit-status-get
      parameters:
      - in: query
        name: resources
        description: A comma-separated list of resource families you want to know
          the current rate limit disposition for
      responses:
        200:
          description: OK
      tags:
      - Rate Limit