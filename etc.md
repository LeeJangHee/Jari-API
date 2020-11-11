# 기타

##  사용 방법

###  검색

{% api-method method="get" host="http://wkdgml96.iptime.org:8080" path="/storeSearch.php?name=\'Store Name\'" %}
{% api-method-summary %}
 Store Search API
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="name" type="string" required=false %}
 String 가게 이름 \(필수\)
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "storeSearch": [
        {
            "id": int id,
            "name": "storeName",
            "phone": "storePhone",
            "address": "storeAddress",
            "latitude": "Latitude",
            "longitude": "Longitude",
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



### 공지사항

{% api-method method="get" host="http://wkdgml96.iptime.org:8080" path="/more/notice.php" %}
{% api-method-summary %}
 Notice API
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
    "notice": [
        {
            "id": int id,
            "title": String "Title",
            "date": date "Date",
            "content": String "Content"
        }
    ]
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

 

### 이벤트

{% api-method method="get" host="http://wkdgml96.iptime.org:8080" path="/more/event.php" %}
{% api-method-summary %}
 Event API
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
    "event": [
        {
            "id": int id,
            "title": String "Title",
            "date": date "Date",
            "content": String "Content"
        }
    ]
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



