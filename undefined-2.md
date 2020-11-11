# 식당 정보

## 개요

요청된 URL 매개 변수를 기반으로 가게 정보를 조회합니다.

## 사용방법

###  가게 정보 보기

{% api-method method="get" host="wkdgml96.iptime.org:8080" path="/storeInfo.php?name=\'Store Name\'" %}
{% api-method-summary %}
StoreInfo API
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="name" type="string" required=false %}
 String name \(필수\)
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "storeInfo": [
        {
            "id": id,
            "name": "storeName",
            "phone": "storePhone",
            "address": "storeAddress",
            "intro": "storeIntro",
            "menu_name": "menuName",
            "menu_price": "menuPrice"
        }
    ]
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



###  대기인원 파악

{% api-method method="get" host="http://wkdgml96.iptime.org:8080" path="/reservation/num.php?storeName=\'Store Name\'" %}
{% api-method-summary %}
Store Waiting Number API
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="storeName" type="string" required=false %}
 String storeName \(필수\)
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    // 대기 인원이 있을때 
    "success": true,
    "num": "대기 팀 숫자"
}

{
    // 대기 인원이 없을 
    "success": false
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

