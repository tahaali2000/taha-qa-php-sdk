# API

```php
$aPIController = $client->getAPIController();
```

## Class Name

`APIController`

## Methods

* [Getusers](../../doc/controllers/api.md#getusers)
* [Createanewuser](../../doc/controllers/api.md#createanewuser)


# Getusers

Returns a list of users, optionally filtered by search.

```php
function getusers(?string $search = null, ?int $limit = null): array
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `search` | `?string` | Query, Optional | Filter users by search term |
| `limit` | `?int` | Query, Optional | Limit the number of users returned |

## Response Type

[`UsersResponse[]`](../../doc/models/users-response.md)

## Example Usage

```php
$result = $aPIController->getusers();
```


# Createanewuser

Creates a user with default values if not provided.

```php
function createanewuser(UsersRequest $body): UsersResponse1
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`UsersRequest`](../../doc/models/users-request.md) | Body, Required | - |

## Response Type

[`UsersResponse1`](../../doc/models/users-response-1.md)

## Example Usage

```php
$body = UsersRequestBuilder::init(
    2,
    DateTimeHelper::fromSimpleDateRequired('2016-03-13')
)->build();

$result = $aPIController->createanewuser($body);
```

