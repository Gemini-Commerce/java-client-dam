# openapi-java-client

Dam Service
- API version: 1.0.0
  - Build date: 2024-08-27T14:48:09.959308722Z[Etc/UTC]

No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)


*Automatically generated by the [OpenAPI Generator](https://openapi-generator.tech)*


## Requirements

Building the API client library requires:
1. Java 1.8+
2. Maven (3.8.3+)/Gradle (7.2+)

## Installation

To install the API client library to your local Maven repository, simply execute:

```shell
mvn clean install
```

To deploy it to a remote Maven repository instead, configure the settings of the repository and execute:

```shell
mvn clean deploy
```

Refer to the [OSSRH Guide](http://central.sonatype.org/pages/ossrh-guide.html) for more information.

### Maven users

Add this dependency to your project's POM:

```xml
<dependency>
  <groupId>org.openapitools</groupId>
  <artifactId>openapi-java-client</artifactId>
  <version>1.2.0</version>
  <scope>compile</scope>
</dependency>
```

### Gradle users

Add this dependency to your project's build file:

```groovy
  repositories {
    mavenCentral()     // Needed if the 'openapi-java-client' jar has been published to maven central.
    mavenLocal()       // Needed if the 'openapi-java-client' jar has been published to the local maven repo.
  }

  dependencies {
     implementation "org.openapitools:openapi-java-client:1.2.0"
  }
```

### Others

At first generate the JAR by executing:

```shell
mvn clean package
```

Then manually install the following JARs:

* `target/openapi-java-client-1.2.0.jar`
* `target/lib/*.jar`

## Getting Started

Please follow the [installation](#installation) instruction and execute the following Java code:

```java

// Import classes:
import GeminiCommerce_Dam.ApiClient;
import GeminiCommerce_Dam.ApiException;
import GeminiCommerce_Dam.Configuration;
import GeminiCommerce_Dam.auth.*;
import GeminiCommerce_Dam.models.*;
import org.openapitools.client.api.BasicOperationsApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://dam.api.gogemini.io");
    
    BasicOperationsApi apiInstance = new BasicOperationsApi(defaultClient);
    DamBatchUploadAssetsRequest body = new DamBatchUploadAssetsRequest(); // DamBatchUploadAssetsRequest | 
    try {
      DamBatchUploadAssetsResponse result = apiInstance.batchUploadAssets(body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling BasicOperationsApi#batchUploadAssets");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}

```

## Documentation for API Endpoints

All URIs are relative to *https://dam.api.gogemini.io*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*BasicOperationsApi* | [**batchUploadAssets**](docs/BasicOperationsApi.md#batchUploadAssets) | **POST** /dam.Dam/BatchUploadAssets | Batch Upload Assets
*BasicOperationsApi* | [**batchUploadAssets_0**](docs/BasicOperationsApi.md#batchUploadAssets_0) | **POST** /dam/batch_upload_assets | Batch Upload Assets
*BasicOperationsApi* | [**createAsset**](docs/BasicOperationsApi.md#createAsset) | **POST** /dam.Dam/CreateAsset | Create Asset
*BasicOperationsApi* | [**createAsset_0**](docs/BasicOperationsApi.md#createAsset_0) | **POST** /dam/create_asset | Create Asset
*BasicOperationsApi* | [**getAssetByCode**](docs/BasicOperationsApi.md#getAssetByCode) | **POST** /dam.Dam/GetAssetByCode | Get Asset By Code
*BasicOperationsApi* | [**getAssetByCode_0**](docs/BasicOperationsApi.md#getAssetByCode_0) | **POST** /dam/get_asset_by_code | Get Asset By Code
*BasicOperationsApi* | [**listAssets**](docs/BasicOperationsApi.md#listAssets) | **POST** /dam.Dam/ListAssets | List Assets
*BasicOperationsApi* | [**listAssetsByCodes**](docs/BasicOperationsApi.md#listAssetsByCodes) | **POST** /dam.Dam/ListAssetsByCodes | List Assets By Codes
*BasicOperationsApi* | [**listAssetsByCodes_0**](docs/BasicOperationsApi.md#listAssetsByCodes_0) | **POST** /dam/list_assets_by_codes | List Assets By Codes
*BasicOperationsApi* | [**listAssetsByIds**](docs/BasicOperationsApi.md#listAssetsByIds) | **POST** /dam.Dam/ListAssetsByIds | List Assets By Ids
*BasicOperationsApi* | [**listAssetsByIds_0**](docs/BasicOperationsApi.md#listAssetsByIds_0) | **POST** /dam/list_assets_by_ids | List Assets By Ids
*BasicOperationsApi* | [**listAssets_0**](docs/BasicOperationsApi.md#listAssets_0) | **POST** /dam/list_assets | List Assets
*BasicOperationsApi* | [**updateAsset**](docs/BasicOperationsApi.md#updateAsset) | **POST** /dam.Dam/UpdateAsset | Update Asset
*BasicOperationsApi* | [**updateAsset_0**](docs/BasicOperationsApi.md#updateAsset_0) | **POST** /dam/update_asset | Update Asset


## Documentation for Models

 - [AssetMetadata](docs/AssetMetadata.md)
 - [AssetOriginTypes](docs/AssetOriginTypes.md)
 - [BatchUploadAssetsRequestFiles](docs/BatchUploadAssetsRequestFiles.md)
 - [DamAsset](docs/DamAsset.md)
 - [DamAssetOrigin](docs/DamAssetOrigin.md)
 - [DamAssetType](docs/DamAssetType.md)
 - [DamBatchUploadAssetsRequest](docs/DamBatchUploadAssetsRequest.md)
 - [DamBatchUploadAssetsResponse](docs/DamBatchUploadAssetsResponse.md)
 - [DamCreateAssetRequest](docs/DamCreateAssetRequest.md)
 - [DamGetAssetByCodeRequest](docs/DamGetAssetByCodeRequest.md)
 - [DamListAssetsByCodesRequest](docs/DamListAssetsByCodesRequest.md)
 - [DamListAssetsByCodesResponse](docs/DamListAssetsByCodesResponse.md)
 - [DamListAssetsByIdsRequest](docs/DamListAssetsByIdsRequest.md)
 - [DamListAssetsByIdsResponse](docs/DamListAssetsByIdsResponse.md)
 - [DamListAssetsRequest](docs/DamListAssetsRequest.md)
 - [DamListAssetsResponse](docs/DamListAssetsResponse.md)
 - [DamUpdateAssetRequest](docs/DamUpdateAssetRequest.md)
 - [ProtobufAny](docs/ProtobufAny.md)
 - [RpcStatus](docs/RpcStatus.md)
 - [UpdateAssetRequestPayload](docs/UpdateAssetRequestPayload.md)


<a id="documentation-for-authorization"></a>
## Documentation for Authorization

Endpoints do not require authorization.


## Recommendation

It's recommended to create an instance of `ApiClient` per thread in a multithreaded environment to avoid any potential issues.

## Author

info@gemini-commerce.com

