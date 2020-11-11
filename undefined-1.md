# 가게 리스트

## 개요

요청된 URL 매개 변수를 기반으로 가게 리스트를 조회합니다.

## 사용방법

### 한식

{% api-method method="get" host="wkdgml96.iptime.org:8080" path="/storeKor.php" %}
{% api-method-summary %}
Store Korean API
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "storeKor": [
        {
            "id": id,
            "name": "storeName",
            "phone": "storePhone",
            "address": "storeAddress",
            "latitude": "storeLatitude",
            "longitude": "storeLongitude",
            "image_profile": "ProfileImage_URL",
            "image_menu": "MenuImage_URL"
        }
    ]
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



### 일식

{% api-method method="get" host="wkdgml96.iptime.org:8080" path="/storeJp.php" %}
{% api-method-summary %}
Store Japanese API
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "storeJp": [
        {
            "id": id,
            "name": "storeName",
            "phone": "storePhone",
            "address": "storeAddress",
            "latitude": "storeLatitude",
            "longitude": "storeLongitude",
            "image_profile": "ProfileImage_URL",
            "image_menu": "MenuImage_URL"
        }
    ]
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



### 중식

{% api-method method="get" host="wkdgml96.iptime.org:8080" path="/storeCh.php" %}
{% api-method-summary %}
Store Chinese API
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "storeCh": [
        {
            "id": id,
            "name": "storeName",
            "phone": "storePhone",
            "address": "storeAddress",
            "latitude": "storeLatitude",
            "longitude": "storeLongitude",
            "image_profile": "ProfileImage_URL",
            "image_menu": "MenuImage_URL"
        }
    ]
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



###  양식

{% api-method method="get" host="wkdgml96.iptime.org:8080" path="/storeWf.php" %}
{% api-method-summary %}
Store Western API
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "storeWf": [
        {
            "id": id,
            "name": "storeName",
            "phone": "storePhone",
            "address": "storeAddress",
            "latitude": "storeLatitude",
            "longitude": "storeLongitude",
            "image_profile": "ProfileImage_URL",
            "image_menu": "MenuImage_URL"
        }
    ]
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



###  카페 / 디저트

{% api-method method="get" host="wkdgml96.iptime.org:8080" path="/storeCafe.php" %}
{% api-method-summary %}
Store Cafe API
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "storeCafe": [
        {
            "id": id,
            "name": "storeName",
            "phone": "storePhone",
            "address": "storeAddress",
            "latitude": "storeLatitude",
            "longitude": "storeLongitude",
            "image_profile": "ProfileImage_URL",
            "image_menu": "MenuImage_URL"
        }
    ]
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



###  술집

{% api-method method="get" host="wkdgml96.iptime.org:8080" path="/storeBeer.php" %}
{% api-method-summary %}
Store Beer API
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "storeBeer": [
        {
            "id": id,
            "name": "storeName",
            "phone": "storePhone",
            "address": "storeAddress",
            "latitude": "storeLatitude",
            "longitude": "storeLongitude",
            "image_profile": "ProfileImage_URL",
            "image_menu": "MenuImage_URL"
        }
    ]
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



###  베스트 음식점

{% api-method method="get" host="wkdgml96.iptime.org:8080" path="/storeBest.php" %}
{% api-method-summary %}
Store Best API
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "storeBest": [
        {
            "id": id,
            "name": "storeName",
            "phone": "storePhone",
            "address": "storeAddress",
            "latitude": "storeLatitude",
            "longitude": "storeLongitude",
            "image_profile": "ProfileImage_URL",
            "image_menu": "MenuImage_URL"
        }
    ]
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

