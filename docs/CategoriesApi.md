# CategoriesApi

All URIs are relative to *https://marketplace-api.com/v1*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**categoriesCategoryIdDelete**](#categoriescategoryiddelete) | **DELETE** /categories/{categoryId} | Видалити категорію|
|[**categoriesCategoryIdGet**](#categoriescategoryidget) | **GET** /categories/{categoryId} | Отримати категорію за ID|
|[**categoriesCategoryIdPut**](#categoriescategoryidput) | **PUT** /categories/{categoryId} | Оновити категорію|
|[**categoriesGet**](#categoriesget) | **GET** /categories | Отримати список категорій|
|[**categoriesPost**](#categoriespost) | **POST** /categories | Створити нову категорію|

# **categoriesCategoryIdDelete**
> categoriesCategoryIdDelete()


### Example

```typescript
import {
    CategoriesApi,
    Configuration
} from 'marketplace-api-client';

const configuration = new Configuration();
const apiInstance = new CategoriesApi(configuration);

let categoryId: number; // (default to undefined)

const { status, data } = await apiInstance.categoriesCategoryIdDelete(
    categoryId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **categoryId** | [**number**] |  | defaults to undefined|


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
|**204** | Категорію успішно видалено |  -  |
|**404** | Категорію не знайдено |  -  |
|**500** | Внутрішня помилка сервера |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **categoriesCategoryIdGet**
> Category categoriesCategoryIdGet()


### Example

```typescript
import {
    CategoriesApi,
    Configuration
} from 'marketplace-api-client';

const configuration = new Configuration();
const apiInstance = new CategoriesApi(configuration);

let categoryId: number; //ID категорії (default to undefined)

const { status, data } = await apiInstance.categoriesCategoryIdGet(
    categoryId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **categoryId** | [**number**] | ID категорії | defaults to undefined|


### Return type

**Category**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Категорію знайдено |  -  |
|**404** | Категорію не знайдено |  -  |
|**500** | Внутрішня помилка сервера |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **categoriesCategoryIdPut**
> Category categoriesCategoryIdPut(categoryInput)


### Example

```typescript
import {
    CategoriesApi,
    Configuration,
    CategoryInput
} from 'marketplace-api-client';

const configuration = new Configuration();
const apiInstance = new CategoriesApi(configuration);

let categoryId: number; // (default to undefined)
let categoryInput: CategoryInput; //

const { status, data } = await apiInstance.categoriesCategoryIdPut(
    categoryId,
    categoryInput
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **categoryInput** | **CategoryInput**|  | |
| **categoryId** | [**number**] |  | defaults to undefined|


### Return type

**Category**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Категорію успішно оновлено |  -  |
|**400** | Невірні дані запиту |  -  |
|**404** | Категорію не знайдено |  -  |
|**500** | Внутрішня помилка сервера |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **categoriesGet**
> Array<Category> categoriesGet()


### Example

```typescript
import {
    CategoriesApi,
    Configuration
} from 'marketplace-api-client';

const configuration = new Configuration();
const apiInstance = new CategoriesApi(configuration);

const { status, data } = await apiInstance.categoriesGet();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<Category>**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Список категорій успішно отримано |  -  |
|**500** | Внутрішня помилка сервера |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **categoriesPost**
> Category categoriesPost(categoryInput)


### Example

```typescript
import {
    CategoriesApi,
    Configuration,
    CategoryInput
} from 'marketplace-api-client';

const configuration = new Configuration();
const apiInstance = new CategoriesApi(configuration);

let categoryInput: CategoryInput; //

const { status, data } = await apiInstance.categoriesPost(
    categoryInput
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **categoryInput** | **CategoryInput**|  | |


### Return type

**Category**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Категорію успішно створено |  -  |
|**400** | Невірні дані запиту |  -  |
|**500** | Внутрішня помилка сервера |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

