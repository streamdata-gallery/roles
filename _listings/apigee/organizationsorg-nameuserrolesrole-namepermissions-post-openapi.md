---
swagger: "2.0"
x-collection-name: Apigee
x-complete: 0
info:
  title: Apigee Edge Post Organizations Name Userroles Role Name Permissions
  description: Associates permissions for a resource with a user role.
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
  /organizations/{org_name}/userroles:
    get:
      summary: Get Organizations Name Userroles
      description: Gets a list of roles available to users in an organization.
      operationId: getOrganizationsOrgNameUserroles
      x-api-path-slug: organizationsorg-nameuserroles-get
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Userroles
    post:
      summary: Post Organizations Name Userroles
      description: Creates a role in an organization.
      operationId: postOrganizationsOrgNameUserroles
      x-api-path-slug: organizationsorg-nameuserroles-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the content type
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Userroles
  /organizations/{org_name}/userroles/{role_name}:
    get:
      summary: Get Organizations Name Userroles Role Name
      description: Gets a role.
      operationId: getOrganizationsOrgNameUserrolesRoleName
      x-api-path-slug: organizationsorg-nameuserrolesrole-name-get
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Userroles
      - Role
    delete:
      summary: Delete Organizations Name Userroles Role Name
      description: Deletes a role from an organization.
      operationId: deleteOrganizationsOrgNameUserrolesRoleName
      x-api-path-slug: organizationsorg-nameuserrolesrole-name-delete
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Userroles
      - Role
  /userroles:
    get:
      summary: Get Userroles
      description: Gets a list of roles available to users.
      operationId: getUserroles
      x-api-path-slug: userroles-get
      responses:
        200:
          description: OK
      tags:
      - Userroles
    post:
      summary: Post Userroles
      description: Creates a role at global level.
      operationId: postUserroles
      x-api-path-slug: userroles-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the Content Type
      responses:
        200:
          description: OK
      tags:
      - Userroles
  /userroles/{role_name}:
    get:
      summary: Get Userroles Role Name
      description: Gets a role.
      operationId: getUserrolesRoleName
      x-api-path-slug: userrolesrole-name-get
      parameters:
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Userroles
      - Role
    delete:
      summary: Delete Userroles Role Name
      description: Deletes a role.
      operationId: deleteUserrolesRoleName
      x-api-path-slug: userrolesrole-name-delete
      parameters:
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Userroles
      - Role
  /users/{user_email}/userroles:
    get:
      summary: Get Users User Email Userroles
      description: Gets roles for a user.
      operationId: getUsersUserEmailUserroles
      x-api-path-slug: usersuser-emailuserroles-get
      parameters:
      - in: path
        name: user_email
        description: Mention the user email
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Email
      - Userroles
    post:
      summary: Post Users User Email Userroles
      description: Associates a user with a organizational user role.
      operationId: postUsersUserEmailUserroles
      x-api-path-slug: usersuser-emailuserroles-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the content type
      - in: path
        name: user_email
        description: Mention the user email
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Email
      - Userroles
  /userroles/{role_name}/users:
    get:
      summary: Get Userroles Role Name Users
      description: Lists users for a role.
      operationId: getUserrolesRoleNameUsers
      x-api-path-slug: userrolesrole-nameusers-get
      parameters:
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Userroles
      - Role
      - Users
    post:
      summary: Post Userroles Role Name Users
      description: Adds user to role.
      operationId: postUserrolesRoleNameUsers
      x-api-path-slug: userrolesrole-nameusers-post
      parameters:
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Userroles
      - Role
      - Users
  /userroles/{role_name}/users/{user_email}:
    get:
      summary: Get Userroles Role Name Users User Email
      description: Checks user in a given system role
      operationId: getUserrolesRoleNameUsersUserEmail
      x-api-path-slug: userrolesrole-nameusersuser-email-get
      parameters:
      - in: path
        name: role_name
        description: Mention the role name
      - in: path
        name: user_email
        description: Mention the user email
      responses:
        200:
          description: OK
      tags:
      - Userroles
      - Role
      - Users
      - User
      - Email
    delete:
      summary: Delete Userroles Role Name Users User Email
      description: Deletes user for a role.
      operationId: deleteUserrolesRoleNameUsersUserEmail
      x-api-path-slug: userrolesrole-nameusersuser-email-delete
      parameters:
      - in: path
        name: role_name
        description: Mention the role name
      - in: path
        name: user_email
        description: Mention the user email
      responses:
        200:
          description: OK
      tags:
      - Userroles
      - Role
      - Users
      - User
      - Email
  /users/{user_email}/userroles/{role_name}:
    delete:
      summary: Delete Users User Email Userroles Role Name
      description: Deletes organizational role for a user.
      operationId: deleteUsersUserEmailUserrolesRoleName
      x-api-path-slug: usersuser-emailuserrolesrole-name-delete
      parameters:
      - in: query
        name: Content-Type
        description: Specify content type
      - in: query
        name: org
        description: Specify the organization name
      - in: path
        name: role_name
        description: Mention the role name
      - in: path
        name: user_email
        description: Mention the user email
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Email
      - Userroles
      - Role
  /organizations/{org_name}/userroles/{role_name}/permissions:
    get:
      summary: Get Organizations Name Userroles Role Name Permissions
      description: Gets a list of permissions associated with the specified resource
        for a single resource.
      operationId: getOrganizationsOrgNameUserrolesRoleNamePermissions
      x-api-path-slug: organizationsorg-nameuserrolesrole-namepermissions-get
      parameters:
      - in: query
        name: Content-Type
        description: Specify content type
      - in: path
        name: org_name
        description: Mention the organization name
      - in: query
        name: path
        description: Specify the resource path
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Userroles
      - Role
      - Permissions
    post:
      summary: Post Organizations Name Userroles Role Name Permissions
      description: Associates permissions for a resource with a user role.
      operationId: postOrganizationsOrgNameUserrolesRoleNamePermissions
      x-api-path-slug: organizationsorg-nameuserrolesrole-namepermissions-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the content type
      - in: path
        name: org_name
        description: Mention the organization name
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Userroles
      - Role
      - Permissions
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