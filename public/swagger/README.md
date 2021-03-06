# user-administration-api

UserAdministrationApi - JavaScript client for user-administration-api
An API to access UserAdministration
This SDK is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:

- API version: 1.0.0
- Package version: 1.0.0
- Build date: 2016-12-10T06:59:37.955-04:00
- Build package: class io.swagger.codegen.languages.JavascriptClientCodegen
For more information, please visit [http://openbank2.com/](http://openbank2.com/)

## Installation

### For [Node.js](https://nodejs.org/)

#### npm

To publish the library as a [npm](https://www.npmjs.com/),
please follow the procedure in ["Publishing npm packages"](https://docs.npmjs.com/getting-started/publishing-npm-packages).

Then install it via:

```shell
npm install user-administration-api --save
```

#### git
#
If the library is hosted at a git repository, e.g.
https://github.com/YOUR_USERNAME/YOUR_GIT_REPO_ID
then install it via:

```shell
npm install YOUR_USERNAME/YOUR_GIT_REPO_ID --save
```

### For browser

The library also works in the browser environment via npm and [browserify](http://browserify.org/). After following
the above steps with Node.js and installing browserify with `npm install -g browserify`,
perform the following (assuming *main.js* is your entry file):

```shell
browserify main.js > bundle.js
```

Then include *bundle.js* in the HTML pages.

## Getting Started

Please follow the [installation](#installation) instruction and execute the following JS code:

```javascript
var UserAdministrationApi = require('user-administration-api');

var defaultClient = UserAdministrationApi.ApiClient.default;

// Configure API key authorization: internalApiKey
var internalApiKey = defaultClient.authentications['internalApiKey'];
internalApiKey.apiKey = "YOUR API KEY"
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//internalApiKey.apiKeyPrefix['access_token'] = "Token"

// Configure OAuth2 access token for authorization: PasswordGrant
var PasswordGrant = defaultClient.authentications['PasswordGrant'];
PasswordGrant.accessToken = "YOUR ACCESS TOKEN"

var api = new UserAdministrationApi.NanoApi()

var loginCreateItem = new UserAdministrationApi.LoginCreateItem(); // {LoginCreateItem} JsonApi with the login object to add


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
api.addLogin(loginCreateItem, callback);

```

## Documentation for API Endpoints

All URIs are relative to *http://localhost/api/v1*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*UserAdministrationApi.NanoApi* | [**addLogin**](docs/NanoApi.md#addLogin) | **POST** /logins | 
*UserAdministrationApi.NanoApi* | [**addPhone**](docs/NanoApi.md#addPhone) | **POST** /phones | 
*UserAdministrationApi.NanoApi* | [**addRole**](docs/NanoApi.md#addRole) | **POST** /roles | 
*UserAdministrationApi.NanoApi* | [**addUser**](docs/NanoApi.md#addUser) | **POST** /users | 
*UserAdministrationApi.NanoApi* | [**deleteLogin**](docs/NanoApi.md#deleteLogin) | **DELETE** /logins/{id} | 
*UserAdministrationApi.NanoApi* | [**deletePhone**](docs/NanoApi.md#deletePhone) | **DELETE** /phones/{id} | 
*UserAdministrationApi.NanoApi* | [**deleteRole**](docs/NanoApi.md#deleteRole) | **DELETE** /roles/{id} | 
*UserAdministrationApi.NanoApi* | [**deleteUser**](docs/NanoApi.md#deleteUser) | **DELETE** /users/{id} | 
*UserAdministrationApi.NanoApi* | [**findLoginById**](docs/NanoApi.md#findLoginById) | **GET** /logins/{id} | 
*UserAdministrationApi.NanoApi* | [**findLogins**](docs/NanoApi.md#findLogins) | **GET** /logins | 
*UserAdministrationApi.NanoApi* | [**findPhoneById**](docs/NanoApi.md#findPhoneById) | **GET** /phones/{id} | 
*UserAdministrationApi.NanoApi* | [**findPhones**](docs/NanoApi.md#findPhones) | **GET** /phones | 
*UserAdministrationApi.NanoApi* | [**findRoleById**](docs/NanoApi.md#findRoleById) | **GET** /roles/{id} | 
*UserAdministrationApi.NanoApi* | [**findRoles**](docs/NanoApi.md#findRoles) | **GET** /roles | 
*UserAdministrationApi.NanoApi* | [**findUserById**](docs/NanoApi.md#findUserById) | **GET** /users/{id} | 
*UserAdministrationApi.NanoApi* | [**findUsers**](docs/NanoApi.md#findUsers) | **GET** /users | 
*UserAdministrationApi.NanoApi* | [**updateLogin**](docs/NanoApi.md#updateLogin) | **PUT** /logins/{id} | 
*UserAdministrationApi.NanoApi* | [**updatePhone**](docs/NanoApi.md#updatePhone) | **PUT** /phones/{id} | 
*UserAdministrationApi.NanoApi* | [**updateRole**](docs/NanoApi.md#updateRole) | **PUT** /roles/{id} | 
*UserAdministrationApi.NanoApi* | [**updateUser**](docs/NanoApi.md#updateUser) | **PUT** /users/{id} | 


## Documentation for Models

 - [UserAdministrationApi.DateTime](docs/DateTime.md)
 - [UserAdministrationApi.Error](docs/Error.md)
 - [UserAdministrationApi.ErrorArray](docs/ErrorArray.md)
 - [UserAdministrationApi.InlineResponse200](docs/InlineResponse200.md)
 - [UserAdministrationApi.InlineResponse2001](docs/InlineResponse2001.md)
 - [UserAdministrationApi.InlineResponse2002](docs/InlineResponse2002.md)
 - [UserAdministrationApi.InlineResponse2003](docs/InlineResponse2003.md)
 - [UserAdministrationApi.InlineResponse2004](docs/InlineResponse2004.md)
 - [UserAdministrationApi.InlineResponse2005](docs/InlineResponse2005.md)
 - [UserAdministrationApi.InlineResponse2006](docs/InlineResponse2006.md)
 - [UserAdministrationApi.InlineResponse2007](docs/InlineResponse2007.md)
 - [UserAdministrationApi.Login](docs/Login.md)
 - [UserAdministrationApi.LoginCreateItem](docs/LoginCreateItem.md)
 - [UserAdministrationApi.LoginUpdateItem](docs/LoginUpdateItem.md)
 - [UserAdministrationApi.Meta](docs/Meta.md)
 - [UserAdministrationApi.Pagination](docs/Pagination.md)
 - [UserAdministrationApi.PaginationLinks](docs/PaginationLinks.md)
 - [UserAdministrationApi.Phone](docs/Phone.md)
 - [UserAdministrationApi.PhoneCreateItem](docs/PhoneCreateItem.md)
 - [UserAdministrationApi.PhoneUpdateItem](docs/PhoneUpdateItem.md)
 - [UserAdministrationApi.ResultSuccess](docs/ResultSuccess.md)
 - [UserAdministrationApi.ResultSuccessMeta](docs/ResultSuccessMeta.md)
 - [UserAdministrationApi.Role](docs/Role.md)
 - [UserAdministrationApi.RoleCreateItem](docs/RoleCreateItem.md)
 - [UserAdministrationApi.RoleUpdateItem](docs/RoleUpdateItem.md)
 - [UserAdministrationApi.User](docs/User.md)
 - [UserAdministrationApi.UserAttributes](docs/UserAttributes.md)
 - [UserAdministrationApi.UserCreateItem](docs/UserCreateItem.md)
 - [UserAdministrationApi.UserUpdateItem](docs/UserUpdateItem.md)


## Documentation for Authorization


### internalApiKey

- **Type**: API key
- **API key parameter name**: access_token
- **Location**: URL query string

### PasswordGrant

- **Type**: OAuth
- **Flow**: password
- **Authorizatoin URL**: 
- **Scopes**: N/A

