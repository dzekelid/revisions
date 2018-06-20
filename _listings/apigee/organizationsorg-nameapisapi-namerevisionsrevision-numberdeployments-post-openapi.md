---
swagger: "2.0"
x-collection-name: Apigee
x-complete: 0
info:
  title: Apigee Edge Post Organizations Name API Name Revisions Revision Number Deployments
  description: Undeploys an API proxy revision from an environment.
  version: 1.0.0
host: api.enterprise.apigee.com
basePath: /v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizations/{org_name}/environments/{env_name}/apis/{api_name}/revisions/{revision_number}/deployments:
    get:
      summary: Get Organizations Name Environments Env Name API Name Revisions Revision
        Number Deployments
      description: "Gets the deployments for an API Proxy\xE2\x80\x99s revision for
        an environment in an organization."
      operationId: getOrganizationsOrgNameEnvironmentsEnvNameApisApiNameRevisionsRevisionNumberDeployments
      x-api-path-slug: organizationsorg-nameenvironmentsenv-nameapisapi-namerevisionsrevision-numberdeployments-get
      parameters:
      - in: path
        name: api_name
        description: Mention the API Proxy name
      - in: path
        name: env_name
        description: Mention the environment name
      - in: path
        name: org_name
        description: Mention the organization name
      - in: path
        name: revision_number
        description: Mention the revision
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Environments
      - Envs
      - APIs
      - Revisions
      - Revision
      - Number
      - Deployments
  /organizations/{org_name}/apis/{api_name}/revisions/{revision_number}/deployments:
    post:
      summary: Post Organizations Name API Name Revisions Revision Number Deployments
      description: Undeploys an API proxy revision from an environment.
      operationId: postOrganizationsOrgNameApisApiNameRevisionsRevisionNumberDeployments
      x-api-path-slug: organizationsorg-nameapisapi-namerevisionsrevision-numberdeployments-post
      parameters:
      - in: query
        name: action
        description: Specify the action
      - in: path
        name: api_name
        description: Mention the API Proxy name
      - in: query
        name: Content-Type
        description: Specify content type
      - in: query
        name: env
        description: Specify environment name
      - in: path
        name: org_name
        description: Mention the organization name
      - in: path
        name: revision_number
        description: Mention the API Proxy revision number
      responses:
        200:
          description: OK
      tags:
      - Organizationss
      - APIs
      - Revisions
      - Revision
      - Number
      - Deployments
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