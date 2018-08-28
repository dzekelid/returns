swagger: "2.0"
x-collection-name: AWS Certificate Manager
x-complete: 1
info:
  title: AWS Certificate Manager API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeCertificate:
    get:
      summary: Describe Certificate
      description: Returns a list of the fields contained in the specified ACM Certificate.
      operationId: DescribeCertificate
      x-api-path-slug: actiondescribecertificate-get
      parameters:
      - in: query
        name: CertificateArn
        description: String that contains an ACM Certificate ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates