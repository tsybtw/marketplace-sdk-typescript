# ProductInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Назва продукту | [default to undefined]
**description** | **string** | Опис продукту | [optional] [default to undefined]
**price** | **number** | Ціна продукту | [default to undefined]
**categoryId** | **number** | ID категорії, до якої належить продукт | [default to undefined]
**inStock** | **boolean** | Чи є продукт в наявності | [optional] [default to undefined]

## Example

```typescript
import { ProductInput } from 'marketplace-api-client';

const instance: ProductInput = {
    name,
    description,
    price,
    categoryId,
    inStock,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
