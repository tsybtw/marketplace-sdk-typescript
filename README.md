## marketplace-api-client@1.0.0

This generator creates TypeScript/JavaScript client that utilizes [axios](https://github.com/axios/axios). The generated Node module can be used in the following environments:

Environment
* Node.js
* Webpack
* Browserify

Language level
* ES5 - you must have a Promises/A+ library installed
* ES6

Module system
* CommonJS
* ES6 module system

It can be used in both TypeScript and JavaScript. In TypeScript, the definition will be automatically resolved via `package.json`. ([Reference](https://www.typescriptlang.org/docs/handbook/declaration-files/consumption.html))

### Building

To build and compile the typescript sources to javascript use:
```
npm install
npm run build
```

### Publishing

First build the package then run `npm publish`

### Consuming

navigate to the folder of your consuming project and run one of the following commands.

_published:_

```
npm install marketplace-api-client@1.0.0 --save
```

_unPublished (not recommended):_

```
npm install PATH_TO_GENERATED_PACKAGE --save
```

### Documentation for API Endpoints

All URIs are relative to *https://marketplace-api.com/v1*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*CategoriesApi* | [**categoriesCategoryIdDelete**](docs/CategoriesApi.md#categoriescategoryiddelete) | **DELETE** /categories/{categoryId} | Видалити категорію
*CategoriesApi* | [**categoriesCategoryIdGet**](docs/CategoriesApi.md#categoriescategoryidget) | **GET** /categories/{categoryId} | Отримати категорію за ID
*CategoriesApi* | [**categoriesCategoryIdPut**](docs/CategoriesApi.md#categoriescategoryidput) | **PUT** /categories/{categoryId} | Оновити категорію
*CategoriesApi* | [**categoriesGet**](docs/CategoriesApi.md#categoriesget) | **GET** /categories | Отримати список категорій
*CategoriesApi* | [**categoriesPost**](docs/CategoriesApi.md#categoriespost) | **POST** /categories | Створити нову категорію
*ProductsApi* | [**productsGet**](docs/ProductsApi.md#productsget) | **GET** /products | Отримати список продуктів
*ProductsApi* | [**productsPost**](docs/ProductsApi.md#productspost) | **POST** /products | Створити новий продукт
*ProductsApi* | [**productsProductIdDelete**](docs/ProductsApi.md#productsproductiddelete) | **DELETE** /products/{productId} | Видалити продукт
*ProductsApi* | [**productsProductIdGet**](docs/ProductsApi.md#productsproductidget) | **GET** /products/{productId} | Отримати продукт за ID
*ProductsApi* | [**productsProductIdPut**](docs/ProductsApi.md#productsproductidput) | **PUT** /products/{productId} | Оновити продукт


### Documentation For Models

 - [Category](docs/Category.md)
 - [CategoryInput](docs/CategoryInput.md)
 - [Product](docs/Product.md)
 - [ProductInput](docs/ProductInput.md)


<a id="documentation-for-authorization"></a>
## Documentation For Authorization


Authentication schemes defined for the API:
<a id="bearerAuth"></a>
### bearerAuth

- **Type**: Bearer authentication (JWT)

