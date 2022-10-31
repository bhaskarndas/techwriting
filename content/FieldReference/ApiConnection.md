## ApiConnection
Connections contains authentication and other information required by NetMatix in order log into external services through their Application Program Interface (API) endpoints to access data stored in those services.  
  
| Field Label | Field Name | Field Type | Description |  
| ---- | ---- | ---- | ---- |  
| Api Connection Id | ApiConnectionId | Guid<br/>  [Key]<br/>  [Required]<br/>  [ReadOnly] |  |  
| Name | ApiConnectionName | String<br/>  [Descriptor] | The name of the external service you want to set up a connection for.  |  
| Description | ApiConnectionDescription | String<br/>  [Template: MultilineText] | Use the Connection Description property to describe the Connection in more detail and provide guidance to other users.  |  
| Connection API Name | ApiConnectionApiName | String<br/>  [TenantUnique]<br/>  [MinLen: 2]<br/>  [MaxLen: 50]<br/>  [Regex: ^[a-zA-Z_][a-zA-Z0-9_.-]*$]<br/>  [ReadOnlyAfterInsert] | A unique and url-safe API name for this Connection. It is used to refer to the Connection in processes and in the external API. The name is derived from the Connection Name by default and can only be edited when creating a new Connection.  |  
| Authorization | AuthorizationType | AuthorizationType | The authorization/authentication scheme/technique NetMatix will use to log into the service provider's API endpoint. NetMatix supports most popular authentication schemes, including basic auth with username and password, API key auth, and OAuth v2.<br/>  Allowable Values: <br/>  <br/>  **ApiKey**<br/>  **BearerToken**<br/>  **Basic**<br/>  **Oauth2** |  
| User Name | UserName | String | The provided username and password will be automatically encrypted with base64 algorithm and passed as header in the format: basic <encrypted_username>:<encrypted_password>.  |  
| Password | Password | String |  |  
| Http Verb | HttpVerb | HttpVerb | Specifies the REST verb that will be used to make the request, eg Post, Get, or Put.<br/>  Allowable Values: <br/>  <br/>  **Post**<br/>  **Get**<br/>  **Put**<br/>  **Delete** |  
| API Endpoint | ApiUrl | String | Enter the URL for the API endpoint with the data you wish to access.  |  
| API Key Name | ApiKeyName | String |  |  
| API Key Value | ApiKeyValue | String |  |  
| API Key Add To | ApiKeyType | ApiKeyType | <br/>  Allowable Values: <br/>  <br/>  **Query**<br/>  **Header** |  
| Bearer Token | BearerToken | String | Bearer tokens allow requests to authenticate using an access key, such as a JSON Web Token (JWT).  |  
| OAuth Token Name | OAuthTokenName | String | Specify a name that uniquely identifies this token.  |  
| Grant Type | GrantType | GrantType | The OAuth2 grant type that the service provider uses to perform authorization. Options: Authorization code and client credentials<br/>  Allowable Values: <br/>  <br/>  **AuthorizationCode**<br/>  **ClientCredentials** |  
| Callback URL | CallbackUrl | String | This is the callback URL that you will be redirected to after your connection is authorized. NetMatix uses this to extract the authorization code or access token. The Callback URL should match the one you use during the application registration process.  |  
| Authorization URL | AuthorizationUrl | String | The endpoint for the authorization server. This is used to get the Authentication code.  |  
| Access Token URL | AccessTokenRequestUrl | String | The endpoint for the Authorization server. This Url is used to exchange the authorization code for an access token. |  
| Client Id | ClientId | String | Client ID that is issued by the service provider. May also be called a Consumer Key or API key.  |  
| API Secret | ClientSecret | String | Your client secret to authorize your application's access to the data. May also be called the Consumer Secret or API Secret.  |  
| Scope | OAuthScope | String | The scope of the access request. It may have multiple space-delimited values.  |  
| State | OAuthState | String | An opaque value that is used for preventing cross-site request forgery.  |  
| Client Authentication | OAuthClientAuthType | OAuthClientAuthType | <br/>  Allowable Values: <br/>  <br/>  **SendAsBasicAuthHeader**<br/>  **SendClientCredentialsInBody** |  
| Refresh Token Request URL | RefreshTokenRequestUrl | String | An optional Refresh Token Request URL where NetMatix can refresh the access token if it expires.  |  
| Test API Endpoint | TestApiUrl | String | Enter an API endpoint URL to test authentication credentials. Preferably one needing no configuration such as /me |  
| Header Prefix | OauthHeaderPrefix | String | Added to the Authorization header before the access token.  |  
| Query Params | RequestParams | List<ApiParameter> | Query parameters are appended to the end of the request URL, following the ? and listed in key value pairs, and separated by & using the following syntax: ?id=1&type=new |  
| Headers | RequestHeaders | List<ApiParameter> | Some APIs require you to send particular headers along with requests, typically to provide additional metadata about the operation you are performing. You can set these up in the Headers tab.  |  
| Body | RequestBody | String | The body is used to send with requests whenever you need to add or update structured data. For example, if you're sending a request to add a new customer to an external service, you might include the customer details in JSON.  |  
| Request Body Type | RequestBodyType | RequestBodyType | <br/>  Allowable Values: <br/>  <br/>  **None**<br/>  **Raw**<br/>  **FormData** |  
| Api Class Name | ApiClassName | String | Select an Api Class such as the DropboxApi from the list of classes with an IApiConnection interface. Methods on the class such as GetFile() and PutFile() will be called to implement specific behaviors for the connection.  |  
| Raw | ResponseRaw | String | Contains the raw unformatted contents of the API response returned by the external service. Includes the body, headers and the status code.  |  
| Status | ResponseStatus | HttpStatusCode | Contains the full raw contest. <br/>  Allowable Values: <br/>  <br/>  **Continue**<br/>  **SwitchingProtocols**<br/>  **Processing**<br/>  **EarlyHints**<br/>  **OK**<br/>  **Created**<br/>  **Accepted**<br/>  **NonAuthoritativeInformation**<br/>  **NoContent**<br/>  **ResetContent**<br/>  **PartialContent**<br/>  **MultiStatus**<br/>  **AlreadyReported**<br/>  **IMUsed**<br/>  **Ambiguous**<br/>  **Ambiguous**<br/>  **Moved**<br/>  **Moved**<br/>  **Redirect**<br/>  **Redirect**<br/>  **RedirectMethod**<br/>  **RedirectMethod**<br/>  **NotModified**<br/>  **UseProxy**<br/>  **Unused**<br/>  **TemporaryRedirect**<br/>  **TemporaryRedirect**<br/>  **PermanentRedirect**<br/>  **BadRequest**<br/>  **Unauthorized**<br/>  **PaymentRequired**<br/>  **Forbidden**<br/>  **NotFound**<br/>  **MethodNotAllowed**<br/>  **NotAcceptable**<br/>  **ProxyAuthenticationRequired**<br/>  **RequestTimeout**<br/>  **Conflict**<br/>  **Gone**<br/>  **LengthRequired**<br/>  **PreconditionFailed**<br/>  **RequestEntityTooLarge**<br/>  **RequestUriTooLong**<br/>  **UnsupportedMediaType**<br/>  **RequestedRangeNotSatisfiable**<br/>  **ExpectationFailed**<br/>  **MisdirectedRequest**<br/>  **UnprocessableEntity**<br/>  **Locked**<br/>  **FailedDependency**<br/>  **UpgradeRequired**<br/>  **PreconditionRequired**<br/>  **TooManyRequests**<br/>  **RequestHeaderFieldsTooLarge**<br/>  **UnavailableForLegalReasons**<br/>  **InternalServerError**<br/>  **NotImplemented**<br/>  **BadGateway**<br/>  **ServiceUnavailable**<br/>  **GatewayTimeout**<br/>  **HttpVersionNotSupported**<br/>  **VariantAlsoNegotiates**<br/>  **InsufficientStorage**<br/>  **LoopDetected**<br/>  **NotExtended**<br/>  **NetworkAuthenticationRequired** |  
| Time | ResponseElapsedTime | Int | Time required to retrieve a response from the external service in millisecnts.  |  
| Size | ResponseSize | String | Size of the response in bytes returned by the external service.  |  
| Created Date | CreatedDate | DateTime |  |  
| Created By | CreatedBy | String |  |  
| Modified Date | ModifiedDate | DateTime |  |  
| Modified By | ModifiedBy | String |  |  
| Row Version | RowVersion | Int |  |  
| Organization Id | OrganizationId | Guid?<br/>  [ForeignKey Organization] |  |  
