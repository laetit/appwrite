# Users Service

## List Users

```http request
GET https://https://appwrite.io/v1/users
```

** Get a list of all the project users. You can use the query params to filter your results. **

### Parameters

| Field Name | Type | Description | Default |
| --- | --- | --- | --- |
| search | string | Search term to filter your list results. |  |
| limit | integer | Results limit value. By default will return maximum 25 results. Maximum of 100 results allowed per request. | 25 |
| offset | integer | Results offset. The default value is 0. Use this param to manage pagination. | 0 |
| orderType | string | Order result by ASC or DESC order. | ASC |

## Create User

```http request
POST https://https://appwrite.io/v1/users
```

** Create a new user. **

### Parameters

| Field Name | Type | Description | Default |
| --- | --- | --- | --- |
| email | string | User account email. |  |
| password | string | User account password. |  |
| name | string | User account name. |  |

## Get User

```http request
GET https://https://appwrite.io/v1/users/{userId}
```

** Get user by its unique ID. **

### Parameters

| Field Name | Type | Description | Default |
| --- | --- | --- | --- |
| userId | string | **Required** User unique ID. |  |

## Get User Logs

```http request
GET https://https://appwrite.io/v1/users/{userId}/logs
```

** Get user activity logs list by its unique ID. **

### Parameters

| Field Name | Type | Description | Default |
| --- | --- | --- | --- |
| userId | string | **Required** User unique ID. |  |

## Get User Prefs

```http request
GET https://https://appwrite.io/v1/users/{userId}/prefs
```

** Get user preferences by its unique ID. **

### Parameters

| Field Name | Type | Description | Default |
| --- | --- | --- | --- |
| userId | string | **Required** User unique ID. |  |

## Get User Sessions

```http request
GET https://https://appwrite.io/v1/users/{userId}/sessions
```

** Get user sessions list by its unique ID. **

### Parameters

| Field Name | Type | Description | Default |
| --- | --- | --- | --- |
| userId | string | **Required** User unique ID. |  |

## Delete User Sessions

```http request
DELETE https://https://appwrite.io/v1/users/{userId}/sessions
```

** Delete all user sessions by its unique ID. **

### Parameters

| Field Name | Type | Description | Default |
| --- | --- | --- | --- |
| userId | string | **Required** User unique ID. |  |

## Delete User Session

```http request
DELETE https://https://appwrite.io/v1/users/{userId}/sessions/:session
```

** Delete user sessions by its unique ID. **

### Parameters

| Field Name | Type | Description | Default |
| --- | --- | --- | --- |
| userId | string | **Required** User unique ID. |  |
| sessionId | string | User unique session ID. |  |

## Update user status

```http request
PATCH https://https://appwrite.io/v1/users/{userId}/status
```

** Update user status by its unique ID. **

### Parameters

| Field Name | Type | Description | Default |
| --- | --- | --- | --- |
| userId | string | **Required** User unique ID. |  |
| status | string | User Status code. To activate the user pass 1, to blocking the user pass 2 and for disabling the user pass 0 |  |

