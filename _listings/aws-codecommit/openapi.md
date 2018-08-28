swagger: "2.0"
x-collection-name: AWS CodeCommit
x-complete: 1
info:
  title: AWS CodeCommit API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=BatchGetRepositories:
    get:
      summary: Batch Get Repositories
      description: Returns information about one or more repositories.
      operationId: batchGetRepositories
      x-api-path-slug: actionbatchgetrepositories-get
      parameters:
      - in: query
        name: repositoryNames
        description: The names of the repositories to get information about
        type: string
      responses:
        200:
          description: OK
      tags:
      - Repositories
  /?Action=GetBranch:
    get:
      summary: Get Branch
      description: Returns information about a repository branch, including its name
        and the last commit ID.
      operationId: getBranch
      x-api-path-slug: actiongetbranch-get
      parameters:
      - in: query
        name: branchName
        description: The name of the branch for which you want to retrieve information
        type: string
      - in: query
        name: repositoryName
        description: The name of the repository that contains the branch for which
          you want to retrieve information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Branches
  /?Action=GetCommit:
    get:
      summary: Get Commit
      description: Returns information about a commit, including commit message and
        committer information.
      operationId: getCommit
      x-api-path-slug: actiongetcommit-get
      parameters:
      - in: query
        name: commitId
        description: The commit ID
        type: string
      - in: query
        name: repositoryName
        description: The name of the repository to which the commit was made
        type: string
      responses:
        200:
          description: OK
      tags:
      - Commits
  /?Action=GetRepository:
    get:
      summary: Get Repository
      description: Returns information about a repository.
      operationId: getRepository
      x-api-path-slug: actiongetrepository-get
      parameters:
      - in: query
        name: repositoryName
        description: The name of the repository to get information about
        type: string
      responses:
        200:
          description: OK
      tags:
      - Repositories