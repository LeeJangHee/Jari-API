# 예약

##  개요

 요청된 URL 매개 변수를 기반으로 예약 정보를 조회합니다.

##  사용 방법

###  예약목록 조회

{% api-method method="post" host="http://wkdgml96.iptime.org:8080" path="/reservation/check.php" %}
{% api-method-summary %}
 Reservation Check API
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="userID" type="string" required=false %}
 String User ID \(필수\)
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    // 예약 정보가 있을 때
    "reservationCheck": [
        {
            "id": int id,
            "userID": "userID",
            "storeName": "storeName",
            "storePhone": "storePhone",
            "storeAddress": "storeAddress",
            "storeProfile": "ProfileImage_URL",
            "storeMenu": "MenuImage_URL"
        }
    ]
}

{
    // 예약 정보가 없을 때
    "reservationCheck": []
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



###  예약 취소

{% api-method method="post" host="http://wkdgml96.iptime.org:8080" path="/reservation/cancel.php" %}
{% api-method-summary %}
 Reservation Cancel API
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="id" type="string" required=false %}
 int 예약 목록 아이디 \(필수\)
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    // 취소 성공
    "success": true
}

{
    // 취소 실패
    "success": false
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}





