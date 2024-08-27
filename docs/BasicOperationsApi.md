# BasicOperationsApi

All URIs are relative to *https://dam.api.gogemini.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**batchUploadAssets**](BasicOperationsApi.md#batchUploadAssets) | **POST** /dam.Dam/BatchUploadAssets | Batch Upload Assets |
| [**batchUploadAssets_0**](BasicOperationsApi.md#batchUploadAssets_0) | **POST** /dam/batch_upload_assets | Batch Upload Assets |
| [**createAsset**](BasicOperationsApi.md#createAsset) | **POST** /dam.Dam/CreateAsset | Create Asset |
| [**createAsset_0**](BasicOperationsApi.md#createAsset_0) | **POST** /dam/create_asset | Create Asset |
| [**getAssetByCode**](BasicOperationsApi.md#getAssetByCode) | **POST** /dam.Dam/GetAssetByCode | Get Asset By Code |
| [**getAssetByCode_0**](BasicOperationsApi.md#getAssetByCode_0) | **POST** /dam/get_asset_by_code | Get Asset By Code |
| [**listAssets**](BasicOperationsApi.md#listAssets) | **POST** /dam.Dam/ListAssets | List Assets |
| [**listAssetsByCodes**](BasicOperationsApi.md#listAssetsByCodes) | **POST** /dam.Dam/ListAssetsByCodes | List Assets By Codes |
| [**listAssetsByCodes_0**](BasicOperationsApi.md#listAssetsByCodes_0) | **POST** /dam/list_assets_by_codes | List Assets By Codes |
| [**listAssetsByIds**](BasicOperationsApi.md#listAssetsByIds) | **POST** /dam.Dam/ListAssetsByIds | List Assets By Ids |
| [**listAssetsByIds_0**](BasicOperationsApi.md#listAssetsByIds_0) | **POST** /dam/list_assets_by_ids | List Assets By Ids |
| [**listAssets_0**](BasicOperationsApi.md#listAssets_0) | **POST** /dam/list_assets | List Assets |
| [**updateAsset**](BasicOperationsApi.md#updateAsset) | **POST** /dam.Dam/UpdateAsset | Update Asset |
| [**updateAsset_0**](BasicOperationsApi.md#updateAsset_0) | **POST** /dam/update_asset | Update Asset |


<a id="batchUploadAssets"></a>
# **batchUploadAssets**
> DamBatchUploadAssetsResponse batchUploadAssets(body)

Batch Upload Assets

### Example
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

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **body** | [**DamBatchUploadAssetsRequest**](DamBatchUploadAssetsRequest.md)|  | |

### Return type

[**DamBatchUploadAssetsResponse**](DamBatchUploadAssetsResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **401** | When an endpoint receives a request with an invalid or unauthorized JWT token, a 401 error (Unauthorized) is thrown. This error indicates that the client is not authenticated or lacks the necessary permissions to access the requested resource. The server responds with the 401 error to enforce security measures and restrict unauthorized access. Clients should handle this error by taking appropriate actions, such as re-authenticating or obtaining a valid token, to gain authorized access. |  -  |
| **500** | An internal error occurred is thrown when an incompatible payload is sent |  -  |
| **0** | An unexpected error response. |  -  |

<a id="batchUploadAssets_0"></a>
# **batchUploadAssets_0**
> DamBatchUploadAssetsResponse batchUploadAssets_0(body)

Batch Upload Assets

### Example
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
      DamBatchUploadAssetsResponse result = apiInstance.batchUploadAssets_0(body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling BasicOperationsApi#batchUploadAssets_0");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **body** | [**DamBatchUploadAssetsRequest**](DamBatchUploadAssetsRequest.md)|  | |

### Return type

[**DamBatchUploadAssetsResponse**](DamBatchUploadAssetsResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **401** | When an endpoint receives a request with an invalid or unauthorized JWT token, a 401 error (Unauthorized) is thrown. This error indicates that the client is not authenticated or lacks the necessary permissions to access the requested resource. The server responds with the 401 error to enforce security measures and restrict unauthorized access. Clients should handle this error by taking appropriate actions, such as re-authenticating or obtaining a valid token, to gain authorized access. |  -  |
| **500** | An internal error occurred is thrown when an incompatible payload is sent |  -  |
| **0** | An unexpected error response. |  -  |

<a id="createAsset"></a>
# **createAsset**
> DamAsset createAsset(body)

Create Asset

### Example
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
    DamCreateAssetRequest body = new DamCreateAssetRequest(); // DamCreateAssetRequest | 
    try {
      DamAsset result = apiInstance.createAsset(body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling BasicOperationsApi#createAsset");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **body** | [**DamCreateAssetRequest**](DamCreateAssetRequest.md)|  | |

### Return type

[**DamAsset**](DamAsset.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **401** | When an endpoint receives a request with an invalid or unauthorized JWT token, a 401 error (Unauthorized) is thrown. This error indicates that the client is not authenticated or lacks the necessary permissions to access the requested resource. The server responds with the 401 error to enforce security measures and restrict unauthorized access. Clients should handle this error by taking appropriate actions, such as re-authenticating or obtaining a valid token, to gain authorized access. |  -  |
| **500** | An internal error occurred is thrown when an incompatible payload is sent |  -  |
| **0** | An unexpected error response. |  -  |

<a id="createAsset_0"></a>
# **createAsset_0**
> DamAsset createAsset_0(body)

Create Asset

### Example
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
    DamCreateAssetRequest body = new DamCreateAssetRequest(); // DamCreateAssetRequest | 
    try {
      DamAsset result = apiInstance.createAsset_0(body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling BasicOperationsApi#createAsset_0");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **body** | [**DamCreateAssetRequest**](DamCreateAssetRequest.md)|  | |

### Return type

[**DamAsset**](DamAsset.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **401** | When an endpoint receives a request with an invalid or unauthorized JWT token, a 401 error (Unauthorized) is thrown. This error indicates that the client is not authenticated or lacks the necessary permissions to access the requested resource. The server responds with the 401 error to enforce security measures and restrict unauthorized access. Clients should handle this error by taking appropriate actions, such as re-authenticating or obtaining a valid token, to gain authorized access. |  -  |
| **500** | An internal error occurred is thrown when an incompatible payload is sent |  -  |
| **0** | An unexpected error response. |  -  |

<a id="getAssetByCode"></a>
# **getAssetByCode**
> DamAsset getAssetByCode(body)

Get Asset By Code

### Example
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
    DamGetAssetByCodeRequest body = new DamGetAssetByCodeRequest(); // DamGetAssetByCodeRequest | 
    try {
      DamAsset result = apiInstance.getAssetByCode(body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling BasicOperationsApi#getAssetByCode");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **body** | [**DamGetAssetByCodeRequest**](DamGetAssetByCodeRequest.md)|  | |

### Return type

[**DamAsset**](DamAsset.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **401** | When an endpoint receives a request with an invalid or unauthorized JWT token, a 401 error (Unauthorized) is thrown. This error indicates that the client is not authenticated or lacks the necessary permissions to access the requested resource. The server responds with the 401 error to enforce security measures and restrict unauthorized access. Clients should handle this error by taking appropriate actions, such as re-authenticating or obtaining a valid token, to gain authorized access. |  -  |
| **500** | An internal error occurred is thrown when an incompatible payload is sent |  -  |
| **0** | An unexpected error response. |  -  |

<a id="getAssetByCode_0"></a>
# **getAssetByCode_0**
> DamAsset getAssetByCode_0(body)

Get Asset By Code

### Example
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
    DamGetAssetByCodeRequest body = new DamGetAssetByCodeRequest(); // DamGetAssetByCodeRequest | 
    try {
      DamAsset result = apiInstance.getAssetByCode_0(body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling BasicOperationsApi#getAssetByCode_0");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **body** | [**DamGetAssetByCodeRequest**](DamGetAssetByCodeRequest.md)|  | |

### Return type

[**DamAsset**](DamAsset.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **401** | When an endpoint receives a request with an invalid or unauthorized JWT token, a 401 error (Unauthorized) is thrown. This error indicates that the client is not authenticated or lacks the necessary permissions to access the requested resource. The server responds with the 401 error to enforce security measures and restrict unauthorized access. Clients should handle this error by taking appropriate actions, such as re-authenticating or obtaining a valid token, to gain authorized access. |  -  |
| **500** | An internal error occurred is thrown when an incompatible payload is sent |  -  |
| **0** | An unexpected error response. |  -  |

<a id="listAssets"></a>
# **listAssets**
> DamListAssetsResponse listAssets(body)

List Assets

### Example
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
    DamListAssetsRequest body = new DamListAssetsRequest(); // DamListAssetsRequest | 
    try {
      DamListAssetsResponse result = apiInstance.listAssets(body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling BasicOperationsApi#listAssets");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **body** | [**DamListAssetsRequest**](DamListAssetsRequest.md)|  | |

### Return type

[**DamListAssetsResponse**](DamListAssetsResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **401** | When an endpoint receives a request with an invalid or unauthorized JWT token, a 401 error (Unauthorized) is thrown. This error indicates that the client is not authenticated or lacks the necessary permissions to access the requested resource. The server responds with the 401 error to enforce security measures and restrict unauthorized access. Clients should handle this error by taking appropriate actions, such as re-authenticating or obtaining a valid token, to gain authorized access. |  -  |
| **500** | An internal error occurred is thrown when an incompatible payload is sent |  -  |
| **0** | An unexpected error response. |  -  |

<a id="listAssetsByCodes"></a>
# **listAssetsByCodes**
> DamListAssetsByCodesResponse listAssetsByCodes(body)

List Assets By Codes

### Example
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
    DamListAssetsByCodesRequest body = new DamListAssetsByCodesRequest(); // DamListAssetsByCodesRequest | 
    try {
      DamListAssetsByCodesResponse result = apiInstance.listAssetsByCodes(body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling BasicOperationsApi#listAssetsByCodes");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **body** | [**DamListAssetsByCodesRequest**](DamListAssetsByCodesRequest.md)|  | |

### Return type

[**DamListAssetsByCodesResponse**](DamListAssetsByCodesResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **401** | When an endpoint receives a request with an invalid or unauthorized JWT token, a 401 error (Unauthorized) is thrown. This error indicates that the client is not authenticated or lacks the necessary permissions to access the requested resource. The server responds with the 401 error to enforce security measures and restrict unauthorized access. Clients should handle this error by taking appropriate actions, such as re-authenticating or obtaining a valid token, to gain authorized access. |  -  |
| **500** | An internal error occurred is thrown when an incompatible payload is sent |  -  |
| **0** | An unexpected error response. |  -  |

<a id="listAssetsByCodes_0"></a>
# **listAssetsByCodes_0**
> DamListAssetsByCodesResponse listAssetsByCodes_0(body)

List Assets By Codes

### Example
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
    DamListAssetsByCodesRequest body = new DamListAssetsByCodesRequest(); // DamListAssetsByCodesRequest | 
    try {
      DamListAssetsByCodesResponse result = apiInstance.listAssetsByCodes_0(body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling BasicOperationsApi#listAssetsByCodes_0");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **body** | [**DamListAssetsByCodesRequest**](DamListAssetsByCodesRequest.md)|  | |

### Return type

[**DamListAssetsByCodesResponse**](DamListAssetsByCodesResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **401** | When an endpoint receives a request with an invalid or unauthorized JWT token, a 401 error (Unauthorized) is thrown. This error indicates that the client is not authenticated or lacks the necessary permissions to access the requested resource. The server responds with the 401 error to enforce security measures and restrict unauthorized access. Clients should handle this error by taking appropriate actions, such as re-authenticating or obtaining a valid token, to gain authorized access. |  -  |
| **500** | An internal error occurred is thrown when an incompatible payload is sent |  -  |
| **0** | An unexpected error response. |  -  |

<a id="listAssetsByIds"></a>
# **listAssetsByIds**
> DamListAssetsByIdsResponse listAssetsByIds(body)

List Assets By Ids

### Example
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
    DamListAssetsByIdsRequest body = new DamListAssetsByIdsRequest(); // DamListAssetsByIdsRequest | 
    try {
      DamListAssetsByIdsResponse result = apiInstance.listAssetsByIds(body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling BasicOperationsApi#listAssetsByIds");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **body** | [**DamListAssetsByIdsRequest**](DamListAssetsByIdsRequest.md)|  | |

### Return type

[**DamListAssetsByIdsResponse**](DamListAssetsByIdsResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **401** | When an endpoint receives a request with an invalid or unauthorized JWT token, a 401 error (Unauthorized) is thrown. This error indicates that the client is not authenticated or lacks the necessary permissions to access the requested resource. The server responds with the 401 error to enforce security measures and restrict unauthorized access. Clients should handle this error by taking appropriate actions, such as re-authenticating or obtaining a valid token, to gain authorized access. |  -  |
| **500** | An internal error occurred is thrown when an incompatible payload is sent |  -  |
| **0** | An unexpected error response. |  -  |

<a id="listAssetsByIds_0"></a>
# **listAssetsByIds_0**
> DamListAssetsByIdsResponse listAssetsByIds_0(body)

List Assets By Ids

### Example
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
    DamListAssetsByIdsRequest body = new DamListAssetsByIdsRequest(); // DamListAssetsByIdsRequest | 
    try {
      DamListAssetsByIdsResponse result = apiInstance.listAssetsByIds_0(body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling BasicOperationsApi#listAssetsByIds_0");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **body** | [**DamListAssetsByIdsRequest**](DamListAssetsByIdsRequest.md)|  | |

### Return type

[**DamListAssetsByIdsResponse**](DamListAssetsByIdsResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **401** | When an endpoint receives a request with an invalid or unauthorized JWT token, a 401 error (Unauthorized) is thrown. This error indicates that the client is not authenticated or lacks the necessary permissions to access the requested resource. The server responds with the 401 error to enforce security measures and restrict unauthorized access. Clients should handle this error by taking appropriate actions, such as re-authenticating or obtaining a valid token, to gain authorized access. |  -  |
| **500** | An internal error occurred is thrown when an incompatible payload is sent |  -  |
| **0** | An unexpected error response. |  -  |

<a id="listAssets_0"></a>
# **listAssets_0**
> DamListAssetsResponse listAssets_0(body)

List Assets

### Example
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
    DamListAssetsRequest body = new DamListAssetsRequest(); // DamListAssetsRequest | 
    try {
      DamListAssetsResponse result = apiInstance.listAssets_0(body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling BasicOperationsApi#listAssets_0");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **body** | [**DamListAssetsRequest**](DamListAssetsRequest.md)|  | |

### Return type

[**DamListAssetsResponse**](DamListAssetsResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **401** | When an endpoint receives a request with an invalid or unauthorized JWT token, a 401 error (Unauthorized) is thrown. This error indicates that the client is not authenticated or lacks the necessary permissions to access the requested resource. The server responds with the 401 error to enforce security measures and restrict unauthorized access. Clients should handle this error by taking appropriate actions, such as re-authenticating or obtaining a valid token, to gain authorized access. |  -  |
| **500** | An internal error occurred is thrown when an incompatible payload is sent |  -  |
| **0** | An unexpected error response. |  -  |

<a id="updateAsset"></a>
# **updateAsset**
> DamAsset updateAsset(body)

Update Asset

### Example
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
    DamUpdateAssetRequest body = new DamUpdateAssetRequest(); // DamUpdateAssetRequest | 
    try {
      DamAsset result = apiInstance.updateAsset(body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling BasicOperationsApi#updateAsset");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **body** | [**DamUpdateAssetRequest**](DamUpdateAssetRequest.md)|  | |

### Return type

[**DamAsset**](DamAsset.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **401** | When an endpoint receives a request with an invalid or unauthorized JWT token, a 401 error (Unauthorized) is thrown. This error indicates that the client is not authenticated or lacks the necessary permissions to access the requested resource. The server responds with the 401 error to enforce security measures and restrict unauthorized access. Clients should handle this error by taking appropriate actions, such as re-authenticating or obtaining a valid token, to gain authorized access. |  -  |
| **500** | An internal error occurred is thrown when an incompatible payload is sent |  -  |
| **0** | An unexpected error response. |  -  |

<a id="updateAsset_0"></a>
# **updateAsset_0**
> DamAsset updateAsset_0(body)

Update Asset

### Example
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
    DamUpdateAssetRequest body = new DamUpdateAssetRequest(); // DamUpdateAssetRequest | 
    try {
      DamAsset result = apiInstance.updateAsset_0(body);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling BasicOperationsApi#updateAsset_0");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **body** | [**DamUpdateAssetRequest**](DamUpdateAssetRequest.md)|  | |

### Return type

[**DamAsset**](DamAsset.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **401** | When an endpoint receives a request with an invalid or unauthorized JWT token, a 401 error (Unauthorized) is thrown. This error indicates that the client is not authenticated or lacks the necessary permissions to access the requested resource. The server responds with the 401 error to enforce security measures and restrict unauthorized access. Clients should handle this error by taking appropriate actions, such as re-authenticating or obtaining a valid token, to gain authorized access. |  -  |
| **500** | An internal error occurred is thrown when an incompatible payload is sent |  -  |
| **0** | An unexpected error response. |  -  |

