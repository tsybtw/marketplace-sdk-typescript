# ProductsApi

All URIs are relative to *https://marketplace-api.com/v1*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**productsGet**](#productsget) | **GET** /products | Отримати список продуктів|
|[**productsPost**](#productspost) | **POST** /products | Створити новий продукт|
|[**productsProductIdDelete**](#productsproductiddelete) | **DELETE** /products/{productId} | Видалити продукт|
|[**productsProductIdGet**](#productsproductidget) | **GET** /products/{productId} | Отримати продукт за ID|
|[**productsProductIdPut**](#productsproductidput) | **PUT** /products/{productId} | Оновити продукт|

# **productsGet**
> Array<Product> productsGet()


### Example

```typescript
import {
    ProductsApi,
    Configuration
} from 'marketplace-api-client';

const configuration = new Configuration();
const apiInstance = new ProductsApi(configuration);

let categoryId: number; //Фільтр за ID категорії (optional) (default to undefined)
let minPrice: number; //Мінімальна ціна (optional) (default to undefined)
let maxPrice: number; //Максимальна ціна (optional) (default to undefined)

const { status, data } = await apiInstance.productsGet(
    categoryId,
    minPrice,
    maxPrice
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **categoryId** | [**number**] | Фільтр за ID категорії | (optional) defaults to undefined|
| **minPrice** | [**number**] | Мінімальна ціна | (optional) defaults to undefined|
| **maxPrice** | [**number**] | Максимальна ціна | (optional) defaults to undefined|


### Return type

**Array<Product>**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Список продуктів успішно отримано |  -  |
|**500** | Внутрішня помилка сервера |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **productsPost**
> Product productsPost(productInput)


### Example

```typescript
import {
    ProductsApi,
    Configuration,
    ProductInput
} from 'marketplace-api-client';

const configuration = new Configuration();
const apiInstance = new ProductsApi(configuration);

let productInput: ProductInput; //

const { status, data } = await apiInstance.productsPost(
    productInput
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **productInput** | **ProductInput**|  | |


### Return type

**Product**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Продукт успішно створено |  -  |
|**400** | Невірні дані запиту |  -  |
|**500** | Внутрішня помилка сервера |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **productsProductIdDelete**
> productsProductIdDelete()


### Example

```typescript
import {
    ProductsApi,
    Configuration
} from 'marketplace-api-client';

const configuration = new Configuration();
const apiInstance = new ProductsApi(configuration);

let productId: number; // (default to undefined)

const { status, data } = await apiInstance.productsProductIdDelete(
    productId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **productId** | [**number**] |  | defaults to undefined|


### Return type

void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**204** | Продукт успішно видалено |  -  |
|**404** | Продукт не знайдено |  -  |
|**500** | Внутрішня помилка сервера |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **productsProductIdGet**
> Product productsProductIdGet()


### Example

```typescript
import {
    ProductsApi,
    Configuration
} from 'marketplace-api-client';

const configuration = new Configuration();
const apiInstance = new ProductsApi(configuration);

let productId: number; //ID продукту (default to undefined)

const { status, data } = await apiInstance.productsProductIdGet(
    productId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **productId** | [**number**] | ID продукту | defaults to undefined|


### Return type

**Product**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Продукт знайдено |  -  |
|**404** | Продукт не знайдено |  -  |
|**500** | Внутрішня помилка сервера |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **productsProductIdPut**
> Product productsProductIdPut(productInput)


### Example

```typescript
import {
    ProductsApi,
    Configuration,
    ProductInput
} from 'marketplace-api-client';

const configuration = new Configuration();
const apiInstance = new ProductsApi(configuration);

let productId: number; // (default to undefined)
let productInput: ProductInput; //

const { status, data } = await apiInstance.productsProductIdPut(
    productId,
    productInput
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **productInput** | **ProductInput**|  | |
| **productId** | [**number**] |  | defaults to undefined|


### Return type

**Product**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Продукт успішно оновлено |  -  |
|**400** | Невірні дані запиту |  -  |
|**404** | Продукт не знайдено |  -  |
|**500** | Внутрішня помилка сервера |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

