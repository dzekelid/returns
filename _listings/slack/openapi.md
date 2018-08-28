swagger: "2.0"
x-collection-name: Slack
x-complete: 1
info:
  title: Slack
  description: one-way-to-interact-with-the-slack-platform-is-its-http-rpcbased-web-api-a-collection-of-methods-requiring-oauth-2-0based-user-bot-or-workspace-tokens-blessed-with-related-oauth-scopes-
  version: 1.0.3
host: slack.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /apps.permissions.info:
    get:
      summary: App Permissions
      description: Returns list of permissions this app has on a team.
      operationId: apps_permissions_info
      x-api-path-slug: apps-permissions-info-get
      parameters:
      - in: query
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Permissions