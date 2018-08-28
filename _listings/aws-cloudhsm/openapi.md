swagger: "2.0"
x-collection-name: AWS CloudHSM
x-complete: 1
info:
  title: AWS CloudHSM API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListTagsForResource:
    get:
      summary: List Tags For Resource
      description: Returns a list of all tags for the specified AWS CloudHSM resource.
      operationId: listTagsForResource
      x-api-path-slug: actionlisttagsforresource-get
      parameters:
      - in: query
        name: ResourceArn
        description: The Amazon Resource Name (ARN) of the AWS CloudHSM resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags