---
swagger: "2.0"
x-collection-name: TVmaze
x-complete: 0
info:
  title: TVmaze user Delete User Follows Shows
  description: Delete user follows shows.
  version: "1.0"
host: api.tvmaze.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/episodes:
    get:
      summary: Get User Episodes
      description: Get user episodes.
      operationId: getUserEpisodes
      x-api-path-slug: userepisodes-get
      parameters:
      - in: query
        name: show_id
        description: Only return episodes from this specific show
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Episodes
  /user/episodes/{episode_id}:
    delete:
      summary: Delete User Episodes
      description: Delete user episodes.
      operationId: deleteUserEpisodesEpisode
      x-api-path-slug: userepisodesepisode-id-delete
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Episodes
    get:
      summary: Get User Episodes
      description: Get user episodes.
      operationId: getUserEpisodesEpisode
      x-api-path-slug: userepisodesepisode-id-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Episodes
    parameters:
      summary: Parameters User Episodes
      description: Parameters user episodes.
      operationId: parametersUserEpisodesEpisode
      x-api-path-slug: userepisodesepisode-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Television
      - Parameters
      - User
      - Episodes
    put:
      summary: Put User Episodes
      description: Set `marked_at` to `NULL` or leave it out to use the current time.
      operationId: putUserEpisodesEpisode
      x-api-path-slug: userepisodesepisode-id-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Episodes
  /user/follows/networks:
    get:
      summary: Get User Follows Networks
      description: Get user follows networks.
      operationId: getUserFollowsNetworks
      x-api-path-slug: userfollowsnetworks-get
      parameters:
      - in: query
        name: embed
        description: Embed full network info
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - Networks
  /user/follows/networks/{network_id}:
    delete:
      summary: Delete User Follows Networks
      description: Delete user follows networks.
      operationId: deleteUserFollowsNetworksNetwork
      x-api-path-slug: userfollowsnetworksnetwork-id-delete
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - Networks
    get:
      summary: Get User Follows Networks
      description: Get user follows networks.
      operationId: getUserFollowsNetworksNetwork
      x-api-path-slug: userfollowsnetworksnetwork-id-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - Networks
    parameters:
      summary: Parameters User Follows Networks
      description: Parameters user follows networks.
      operationId: parametersUserFollowsNetworksNetwork
      x-api-path-slug: userfollowsnetworksnetwork-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Television
      - Parameters
      - User
      - Follows
      - Networks
    put:
      summary: Put User Follows Networks
      description: Put user follows networks.
      operationId: putUserFollowsNetworksNetwork
      x-api-path-slug: userfollowsnetworksnetwork-id-put
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - Networks
  /user/follows/people:
    get:
      summary: Get User Follows People
      description: Get user follows people.
      operationId: getUserFollowsPeople
      x-api-path-slug: userfollowspeople-get
      parameters:
      - in: query
        name: embed
        description: Embed full person info
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - People
  /user/follows/people/{person_id}:
    delete:
      summary: Delete User Follows People Person
      description: Delete user follows people person.
      operationId: deleteUserFollowsPeoplePerson
      x-api-path-slug: userfollowspeopleperson-id-delete
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - People
      - Person
    get:
      summary: Get User Follows People Person
      description: Get user follows people person.
      operationId: getUserFollowsPeoplePerson
      x-api-path-slug: userfollowspeopleperson-id-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - People
      - Person
    parameters:
      summary: Parameters User Follows People Person
      description: Parameters user follows people person.
      operationId: parametersUserFollowsPeoplePerson
      x-api-path-slug: userfollowspeopleperson-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Television
      - Parameters
      - User
      - Follows
      - People
      - Person
    put:
      summary: Put User Follows People Person
      description: Put user follows people person.
      operationId: putUserFollowsPeoplePerson
      x-api-path-slug: userfollowspeopleperson-id-put
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - People
      - Person
  /user/follows/shows:
    get:
      summary: Get User Follows Shows
      description: Get user follows shows.
      operationId: getUserFollowsShows
      x-api-path-slug: userfollowsshows-get
      parameters:
      - in: query
        name: embed
        description: Embed full show info
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - Shows
  /user/follows/shows/{show_id}:
    delete:
      summary: Delete User Follows Shows
      description: Delete user follows shows.
      operationId: deleteUserFollowsShowsShow
      x-api-path-slug: userfollowsshowsshow-id-delete
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - Shows
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