---
swagger: "2.0"
x-collection-name: Starred
x-complete: 1
info:
  title: Starred API
  description: starred-apistarredapiintrostarred-provides-rest-apis-to-help-our-clients-automate-feedback-process--with-starred-api-organizations-can-send-survey-invites-generate-survey-links-or-get-the-summary-of-survey-forms--starred-webhook-allows-your-to-subscribe-to-feedback-notifications-in-real-time-with-feedback-data-the-easiest-way-to-start-using-the-starred-api-is-by-clicking-the-run-in-postman-button-above--postman-is-a-free-tool-which-helps-developers-run-and-debug-api-requests--every-endpoint-you-see-documented-here-is-readily-available-by-running-our-postman-collection--tls-1-0-deprecatedstarred-has-deprecated-support-for-transport-layer-security-tls-1-0-because-of-the-security-issues--this-means-we-only-support-transport-layer-security-tls-1-1-and-tls-1-2if-your-programming-language-requires-you-to-define-security-protocol-then-please-use-tls-1-1-or-above--need-helpthe-starred-team-is-always-around-to-answer-your-questions--send-your-questions-to-apistarred-commailtoapistarred-com-restfulthe-only-thing-you-need-to-get-going-is-an-active-account-with-the-api-enabled--each-request-requires-the-two-parameters-stated-to-the-right--you-can-find-those-in-your-settings-page-the-starred-api-is-organized-around-rest--json-is-returned-by-all-api-responses-including-errors-although-our-api-libraries-convert-responses-to-appropriate-languagespecific-objects--api-endpointthis-shows-a-basic-api-endpoint--all-endpoints-are-relative-to-this-path-javascripthttpsapi-starred-commost-endpoints-have-their-own-set-of-additional-parameters--those-can-either-be-added-to-the-endpoint-url-or-be-set-as-http-post-parameters--authenticationthe-starred-uses-basic-authentication--authenticate-your-requests-when-using-the-api-by-including-your-secret-api-key-and-company-id-in-the-request--your-api-key-carry-many-privileges-so-be-sure-to-keep-them-secret-do-not-share-your-secret-api-keys-in-publicly-accessible-areas-such-github-clientside-code-etc--all-api-requests-must-be-made-over-https--calls-made-over-plain-http-will-fail--api-requests-without-authentication-will-also-fail-mandatory-parameters-parameter--description------company--the-company-key-which-is-available-from-your-company-settings-page--auth--the-api-key-which-is-available-from-your-company-settings-page-your-api-request-will-look-like-this-after-adding-authentication-parameters-javascripthttpsapi-starred-comsomeendpointmethodcompanycompanykeyauthapikeystarred-api-keystarredapikey-responseevery-request-gets-back-a-response-which-contains-response-headers-and-response-body--response-headersyou-will-receive-following-response-headers-with-every-response---response-header--description------contentlength--the-length-of-response-body--contenttype--the-type-of-this-content--date--the-time-when-the-request-was-sent--expires--the-date-and-time-after-which-the-response-is-considered-slate--contentencoding--the-type-of-encoding-used-on-data-response-bodyresponses-are-always-json--success-responsejson----status-ok----message-invitations-queued-for-delivery-error-responsejson----status-fail----errorcode-404----message-not-found-response-codesstarred-uses-http-response-codes-to-indicate-the-success-or-failure-of-an-api-request--in-general-codes-in-the-2xx-range-indicate-success-codes-in-the-4xx-range-indicate-an-error-that-failed-given-the-information-provided-and-codes-in-the-5xx-range-indicate-an-error-with-the-starred-server-this-happens-rarely--response-code--description------200--request-successful---403--access-is-denied-because-you-have-not-used-the-proper-access-token-for-the-request---404--endpoint-url-is-invalid---400--invalid-request---500--internal-server-error---feedbackwe-love-feedback-please-give-us-feedback-on-this-api-at-apistarred-commailtoapistarred-com-starred-jobsstarredjobsdo-you-want-to-be-the-part-of-our-journey-to-create-the-best-and-simplest-api-for-feedback-take-a-look-at-starred-jobshttpsjobs-starred-comutm-sourceapidocsutm-mediumkhizar--api-referencestarredapikey-httpwww-starred-comwpcontentuploads201805starredapi-pngstarredapiintro-httpwww-starred-comwpcontentuploads201805apiheader-pngstarredjobs-httpwww-starred-comwpcontentuploads201805jobstarredcom-png
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /segment/summary:
    get:
      summary: Dashboard Summary
      description: "Retrieve segment summary from your account. This summary includes
        your NPS score and detailed breakdown.\n\n**Request Parameters**\n\n| Parameter
        | Required | Description |\n| ------ | ------ | ------ |\n| `form` | Required
        | ID of the form that will be sent out |\n| `segment` | Optional | Group ID
        to get summary data for (defaults to 0) |\n\nNote: Segment is an alias for
        Groups in Starred Platform. You can retrieve Segment ID on Groups page in
        Starred Platform. [Groups in Starred](https://app.starred.com/segments/overview)\n\n####
        Steps to retrieve Segment ID\n1. Login to Starred Platform\n2. Go to Clients
        tab\n3. Click on a Group you want to get data for. \n4. In Group detail view
        copy the Segment ID from URL\n\n![Starred API Key][starred-segment-id]\n[See
        Full Image](http://www.starred.com/wp-content/uploads/2018/05/starred-segment-id.png)\n[starred-segment-id]:
        http://www.starred.com/wp-content/uploads/2018/05/starred-segment-id.png"
      operationId: SegmentSummaryGet
      x-api-path-slug: segmentsummary-get
      responses:
        200:
          description: OK
      tags:
      - Dashboard
      - Summary
---