
# Kurabu API




## Endpoints

* [Get CLUB information](#get-club-information)
    1. [Club Info](#1-club-info)
* [Get Auth Token](#get-auth-token)
    1. [Admin LOGIN - TOKEN Copy](#1-admin-login---token-copy)
* [Using CLUB_SUBDOMAIN](#using-club_subdomain)
    1. [All published news articles](#1-all-published-news-articles)
    1. [Published news articles with Date params](#2-published-news-articles-with-date-params)
    1. [Public Events](#3-public-events)
    1. [All Events](#4-all-events)
* [Using CLUB_ID](#using-club_id)
    1. [All published news articles](#1-all-published-news-articles-1)
    1. [Published news articles with Date params](#2-published-news-articles-with-date-params-1)
    1. [Public Events](#3-public-events-1)
    1. [All Events](#4-all-events-1)

--------



## Get CLUB information



### 1. Club Info



***Endpoint:***

```bash
Method: GET
Type: 
URL: https://api.kurabu.com/v1/club-subdomain/[CLUB_SUBDOMAIN]
```



## Get Auth Token



### 1. Admin LOGIN - TOKEN Copy



***Endpoint:***

```bash
Method: POST
Type: RAW
URL: http://api.kurabu.local:4000/token
```



***Body:***

```js        
{
    "admin": {
        "email": "email@test.com",
        "password": "your_password",
        "club_subdomain": "club_subdomain"
    }
}
```



## Using CLUB_SUBDOMAIN



### 1. All published news articles



***Endpoint:***

```bash
Method: GET
Type: 
URL: https://api.kurabu.com/v1/club-subdomain/[CLUB_SUBDOMAIN]/news
```



### 2. Published news articles with Date params



***Endpoint:***

```bash
Method: GET
Type: 
URL: https://api.kurabu.com/v1/club-subdomain/[CLUB_SUBDOMAIN]/news
```



***Query params:***

| Key | Value | Description |
| --- | ------|-------------|
| from | 2023-04-01 |  |
| until | 2023-12-01 |  |



### 3. Public Events



***Endpoint:***

```bash
Method: GET
Type: 
URL: https://api.kurabu.com/v1/club-subdomain/[CLUB_SUBDOMAIN]/public_events
```



***Query params:***

| Key | Value | Description |
| --- | ------|-------------|
| from | 2023-05-12 |  |
| until | 2023-05-13 |  |



### 4. All Events



***Endpoint:***

```bash
Method: GET
Type: 
URL: https://api.kurabu.com/v1/club-subdomain/[CLUB_SUBDOMAIN]/events
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Authorization | Bearer {{token}} |  |



***Query params:***

| Key | Value | Description |
| --- | ------|-------------|
| from | 2023-05-01 |  |
| until | 2023-05-31 |  |



## Using CLUB_ID



### 1. All published news articles



***Endpoint:***

```bash
Method: GET
Type: 
URL: https://api.kurabu.com/v1/clubs/[CLUB_ID]/news
```



### 2. Published news articles with Date params



***Endpoint:***

```bash
Method: GET
Type: 
URL: https://api.kurabu.com/v1/clubs/[CLUB_ID]/news
```



***Query params:***

| Key | Value | Description |
| --- | ------|-------------|
| from | 2023-04-01 |  |
| until | 2023-12-02 |  |



### 3. Public Events



***Endpoint:***

```bash
Method: GET
Type: 
URL: https://api.kurabu.com/v1/clubs/[CLUB_ID]/public_events
```



***Query params:***

| Key | Value | Description |
| --- | ------|-------------|
| from | 2023-04-01 |  |
| until | 2023-04-30 |  |



### 4. All Events



***Endpoint:***

```bash
Method: GET
Type: 
URL: http://api.kurabu.local:4000/v1/clubs/89789191-e033-4f78-8d2e-e24e7e83eaa0/events
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Authorization | Bearer {{token}} |  |



***Query params:***

| Key | Value | Description |
| --- | ------|-------------|
| from | 2023-04-01 |  |
| until | 2023-04-30 |  |



---
[Back to top](#kurabu-api)
