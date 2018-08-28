swagger: "2.0"
x-collection-name: VictorOps
x-complete: 1
info:
  title: Victor Ops
  description: this-api-allows-you-to-interact-with-the-victorops-platform-in-various-ways--your-account-may-be-limitedto-a-total-number-of-api-calls-per-month--also-some-of-these-api-calls-have-rate-limits-note-in-this-documentation-when-creating-a-sample-curl-request-clicking-the-try-it-out-button-in-some-apiviewing-interfaces-the--in-an-email-address-may-be-encoded--please-note-that-the-rest-endpoints-will-notprocess-the-encoded-version--make-sure-that-the-encoded-character-40-is-changed-to-its-unencoded-form-beforesubmitting-the-curl-request-
  version: 0.0.2
host: api.victorops.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api-reporting/v1/team/{team}/oncall/log:
    get:
      summary: A list of shift changes for a team
      description: |-
        Returns a log of user shift changes for the specified team. This is historical
        data, and may be up to 15 minutes behind real-time log data.

        This API may be called a maximum of 6 times per minute.
      operationId: api_reporting.v1.team.team.oncall.log.get
      x-api-path-slug: apireportingv1teamteamoncalllog-get
      parameters:
      - in: query
        name: end
        description: Return shift changes occurring before this timestamp
      - in: query
        name: No Name
      - in: query
        name: start
        description: Return shift changes occurring after this timestamp
      - in: path
        name: team
        description: The VictorOps team slug
      - in: query
        name: userName
        description: The VictorOps user ID
      responses:
        200:
          description: OK
      tags:
      - Api-reporting
      - V1
      - Team
      - Team
      - Oncall
      - Log