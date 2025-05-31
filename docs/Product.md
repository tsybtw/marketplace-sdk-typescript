# Product


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Унікальний ідентифікатор продукту | [default to undefined]
**name** | **string** | Назва продукту | [default to undefined]
**description** | **string** | Опис продукту | [optional] [default to undefined]
**price** | **number** | Ціна продукту | [default to undefined]
**categoryId** | **number** | ID категорії, до якої належить продукт | [default to undefined]
**category** | [**Category**](Category.md) |  | [optional] [default to undefined]
**inStock** | **boolean** | Чи є продукт в наявності | [optional] [default to undefined]
**createdAt** | **string** | Дата створення | [optional] [default to undefined]
**updatedAt** | **string** | Дата останнього оновлення | [optional] [default to undefined]

## Example

```typescript
import { Product } from 'marketplace-api-client';

const instance: Product = {
    id,
    name,
    description,
    price,
    categoryId,
    category,
    inStock,
    createdAt,
    updatedAt,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
