swagger: "2.0"
x-collection-name: CollabNet
x-complete: 1
info:
  title: Foundation API
  version: 1.0.0
basePath: /ctfrest/foundation/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /monitoring/users/{userid}/objects:
    get:
      summary: Returns the list of monitoring items for the given userid
      description: Returns the list of monitoring items for the given userid.
      operationId: monitorSubforUserId
      x-api-path-slug: monitoringusersuseridobjects-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: query
        name: offset
        description: Offset
      - in: query
        name: projectid
        description: Project Id
      - in: path
        name: userid
        description: User id
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Monitoring
      - Itemsthe
      - Given
      - Userid
  /monitoring/users/myself/objects:
    get:
      summary: Returns the list of monitoring items for current user
      description: Returns the list of monitoring items for current user.
      operationId: monitoringItemsForUser
      x-api-path-slug: monitoringusersmyselfobjects-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: query
        name: offset
        description: Offset
      - in: query
        name: projectid
        description: Project id
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Monitoring
      - Itemscurrent
      - User
  /monitoring/users/by-username/{username}/objects:
    get:
      summary: Returns the list of monitoring items for the given username
      description: Returns the list of monitoring items for the given username.
      operationId: monitoringItemsForUsername
      x-api-path-slug: monitoringusersbyusernameusernameobjects-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: query
        name: offset
        description: Offset
      - in: query
        name: projectid
        description: Project Id
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Monitoring
      - Itemsthe
      - Given
      - Username
  /monitoring/objects/{objectid}/users:
    get:
      summary: Returns the list of monitoring users for the object(Folder/Item).
      description: Returns the list of monitoring users for the object(folder/item)..
      operationId: listUsersForObject
      x-api-path-slug: monitoringobjectsobjectidusers-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: path
        name: objectid
        description: Object id
      - in: query
        name: offset
        description: Offset
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Monitoring
      - Usersthe
      - Object(Folder
      - Item)