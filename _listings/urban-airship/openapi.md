swagger: "2.0"
x-collection-name: Urban Airship
x-complete: 1
info:
  title: Urban Airship
  description: the-urban-airships-api-powers-mobile-applications-with-push-rich-push-inapp-purchases-and-subscription-services-
  version: v3
host: go.urbanairship.com
basePath: /api/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/{user_id}/subscriptions/{subscription_key}/purchase:
    post:
      summary: Post User User Subscriptions Subscription Key Purchase
      description: Adds a new subscription.
      operationId: user.user_id.subscriptions.subscription_key.purchase.post
      x-api-path-slug: useruser-idsubscriptionssubscription-keypurchase-post
      parameters:
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      - in: query
        name: subscription_key
        description: Subscription Key
      - in: path
        name: subscription_key
      - in: query
        name: user_id
        description: User ID
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Id
      - Subscriptions
      - Subscription
      - Key
      - Purchase