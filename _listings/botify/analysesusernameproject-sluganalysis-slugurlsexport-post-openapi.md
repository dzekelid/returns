---
swagger: "2.0"
x-collection-name: Botify
x-complete: 0
info:
  title: Botify Post Analyses Username Project Slug Analysis Slug Urls Export
  description: Creates a new UrlExport object and starts a task that will export the
    results into a csv. Returns the model id that manages the task
  version: 1.0.0
host: api.botify.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /analyses/{username}/{project_slug}/{analysis_slug}/crawl_statistics/time:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Crawl Statistics Time
      description: Return crawl statistics grouped by time frequency (1 min, 5 mins
        or 60 min) for an analysis
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugCrawlStatisticsTime
      x-api-path-slug: analysesusernameproject-sluganalysis-slugcrawl-statisticstime-get
      parameters:
      - in: query
        name: frequency
        description: Aggregation frequency
      - in: query
        name: limit
        description: max number of elements to retrieve
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Crawl
      - Statistics
      - Time
  /analyses/{username}/{project_slug}/{analysis_slug}/crawl_statistics/urls/{list_type}:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Crawl Statistics Urls
        List Type
      description: Return a list of 1000 latest URLs crawled (all crawled URLs or
        only URLS with HTTP errors)
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugCrawlStatisticsUrlsListType
      x-api-path-slug: analysesusernameproject-sluganalysis-slugcrawl-statisticsurlslist-type-get
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Crawl
      - Statistics
      - Urls
      - List
      - Type
  /analyses/{username}/{project_slug}/{analysis_slug}/urls/export:
    post:
      summary: Post Analyses Username Project Slug Analysis Slug Urls Export
      description: Creates a new UrlExport object and starts a task that will export
        the results into a csv. Returns the model id that manages the task
      operationId: postAnalysesUsernameProjectSlugAnalysisSlugUrlsExport
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlsexport-post
      parameters:
      - in: query
        name: area
        description: Analysis context
      - in: body
        name: UrlsQuery
        description: Urls query
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Urls
      - Export
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