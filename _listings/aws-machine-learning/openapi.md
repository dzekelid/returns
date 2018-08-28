swagger: "2.0"
x-collection-name: AWS Machine Learning
x-complete: 1
info:
  title: AWS Machine Learning API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeBatchPredictions:
    get:
      summary: Describe Batch Predictions
      description: Returns a list of BatchPrediction operations that match the search
        criteria in the request.
      operationId: describeBatchPredictions
      x-api-path-slug: actiondescribebatchpredictions-get
      parameters:
      - in: query
        name: EQ
        description: The equal to operator
        type: string
      - in: query
        name: FilterVariable
        description: 'Use one of the following variables to filter a list of BatchPrediction:'
        type: string
      - in: query
        name: GE
        description: The greater than or equal to operator
        type: string
      - in: query
        name: GT
        description: The greater than operator
        type: string
      - in: query
        name: LE
        description: The less than or equal to operator
        type: string
      - in: query
        name: Limit
        description: The number of pages of information to include in the result
        type: string
      - in: query
        name: LT
        description: The less than operator
        type: string
      - in: query
        name: NE
        description: The not equal to operator
        type: string
      - in: query
        name: NextToken
        description: An ID of the page in the paginated results
        type: string
      - in: query
        name: Prefix
        description: A string that is found at the beginning of a variable, such as
          Name or Id
        type: string
      - in: query
        name: SortOrder
        description: A two-value parameter that determines the sequence of the resulting
          list of MLModels
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Batches
  /?Action=DescribeDataSources:
    get:
      summary: Describe Data Sources
      description: Returns a list of DataSource that match the search criteria in
        the request.
      operationId: describeDataSources
      x-api-path-slug: actiondescribedatasources-get
      parameters:
      - in: query
        name: EQ
        description: The equal to operator
        type: string
      - in: query
        name: FilterVariable
        description: 'Use one of the following variables to filter a list of DataSource:'
        type: string
      - in: query
        name: GE
        description: The greater than or equal to operator
        type: string
      - in: query
        name: GT
        description: The greater than operator
        type: string
      - in: query
        name: LE
        description: The less than or equal to operator
        type: string
      - in: query
        name: Limit
        description: The maximum number of DataSource to include in the result
        type: string
      - in: query
        name: LT
        description: The less than operator
        type: string
      - in: query
        name: NE
        description: The not equal to operator
        type: string
      - in: query
        name: NextToken
        description: The ID of the page in the paginated results
        type: string
      - in: query
        name: Prefix
        description: A string that is found at the beginning of a variable, such as
          Name or Id
        type: string
      - in: query
        name: SortOrder
        description: A two-value parameter that determines the sequence of the resulting
          list of DataSource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Data Sources
  /?Action=DescribeEvaluations:
    get:
      summary: Describe Evaluations
      description: Returns a list of DescribeEvaluations that match the search criteria
        in the request.
      operationId: describeEvaluations
      x-api-path-slug: actiondescribeevaluations-get
      parameters:
      - in: query
        name: EQ
        description: The equal to operator
        type: string
      - in: query
        name: FilterVariable
        description: 'Use one of the following variable to filter a list of Evaluation
          objects:'
        type: string
      - in: query
        name: GE
        description: The greater than or equal to operator
        type: string
      - in: query
        name: GT
        description: The greater than operator
        type: string
      - in: query
        name: LE
        description: The less than or equal to operator
        type: string
      - in: query
        name: Limit
        description: The maximum number of Evaluation to include in the result
        type: string
      - in: query
        name: LT
        description: The less than operator
        type: string
      - in: query
        name: NE
        description: The not equal to operator
        type: string
      - in: query
        name: NextToken
        description: The ID of the page in the paginated results
        type: string
      - in: query
        name: Prefix
        description: A string that is found at the beginning of a variable, such as
          Name or Id
        type: string
      - in: query
        name: SortOrder
        description: A two-value parameter that determines the sequence of the resulting
          list of Evaluation
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Evaluations
  /?Action=DescribeMLModels:
    get:
      summary: Describe M L Models
      description: Returns a list of MLModel that match the search criteria in the
        request.
      operationId: describeMLModels
      x-api-path-slug: actiondescribemlmodels-get
      parameters:
      - in: query
        name: EQ
        description: The equal to operator
        type: string
      - in: query
        name: FilterVariable
        description: 'Use one of the following variables to filter a list of MLModel:'
        type: string
      - in: query
        name: GE
        description: The greater than or equal to operator
        type: string
      - in: query
        name: GT
        description: The greater than operator
        type: string
      - in: query
        name: LE
        description: The less than or equal to operator
        type: string
      - in: query
        name: Limit
        description: The number of pages of information to include in the result
        type: string
      - in: query
        name: LT
        description: The less than operator
        type: string
      - in: query
        name: NE
        description: The not equal to operator
        type: string
      - in: query
        name: NextToken
        description: The ID of the page in the paginated results
        type: string
      - in: query
        name: Prefix
        description: A string that is found at the beginning of a variable, such as
          Name or Id
        type: string
      - in: query
        name: SortOrder
        description: A two-value parameter that determines the sequence of the resulting
          list of MLModel
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Models
  /?Action=GetBatchPrediction:
    get:
      summary: Get Batch Prediction
      description: |-
        Returns a BatchPrediction that includes detailed metadata, status, and data file information for a
                    Batch Prediction request.
      operationId: getBatchPrediction
      x-api-path-slug: actiongetbatchprediction-get
      parameters:
      - in: query
        name: BatchPredictionId
        description: An ID assigned to the BatchPrediction at creation
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Batches
  /?Action=GetDataSource:
    get:
      summary: Get Data Source
      description: Returns a DataSource that includes metadata and data file information,
        as well as the current status of the DataSource.
      operationId: getDataSource
      x-api-path-slug: actiongetdatasource-get
      parameters:
      - in: query
        name: DataSourceId
        description: The ID assigned to the DataSource at creation
        type: string
      - in: query
        name: Verbose
        description: Specifies whether the GetDataSource operation should return DataSourceSchema
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Data Sources
  /?Action=GetEvaluation:
    get:
      summary: Get Evaluation
      description: Returns an Evaluation that includes metadata as well as the current
        status of the Evaluation.
      operationId: getEvaluation
      x-api-path-slug: actiongetevaluation-get
      parameters:
      - in: query
        name: EvaluationId
        description: The ID of the Evaluation to retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Evaluations
  /?Action=GetMLModel:
    get:
      summary: Get M L Model
      description: Returns an MLModel that includes detailed metadata, data source
        information, and the current status of the MLModel.
      operationId: getMLModel
      x-api-path-slug: actiongetmlmodel-get
      parameters:
      - in: query
        name: MLModelId
        description: The ID assigned to the MLModel at creation
        type: string
      - in: query
        name: Verbose
        description: Specifies whether the GetMLModel operation should return Recipe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Models