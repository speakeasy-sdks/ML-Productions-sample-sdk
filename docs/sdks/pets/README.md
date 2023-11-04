# Pets
(*pets*)

### Available Operations

* [createPets](#createpets) - Create a pet
* [listPets](#listpets) - List all pets
* [showPetById](#showpetbyid) - Info for a specific pet

## createPets

Create a pet

### Example Usage

```typescript
import { WidgetService } from "Widget-Service";

(async() => {
  const sdk = new WidgetService();

  const res = await sdk.pets.createPets();


  if (res.statusCode == 200) {
    // handle response
  }
})();
```

### Parameters

| Parameter                                                    | Type                                                         | Required                                                     | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| `config`                                                     | [AxiosRequestConfig](https://axios-http.com/docs/req_config) | :heavy_minus_sign:                                           | Available config options for making requests.                |


### Response

**Promise<[operations.CreatePetsResponse](../../models/operations/createpetsresponse.md)>**


## listPets

List all pets

### Example Usage

```typescript
import { WidgetService } from "Widget-Service";
import { ListPetsRequest } from "Widget-Service/dist/sdk/models/operations";

(async() => {
  const sdk = new WidgetService();
const limit: number = 21453;

  const res = await sdk.pets.listPets(limit);


  if (res.statusCode == 200) {
    // handle response
  }
})();
```

### Parameters

| Parameter                                                    | Type                                                         | Required                                                     | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| `limit`                                                      | *number*                                                     | :heavy_minus_sign:                                           | How many items to return at one time (max 100)               |
| `config`                                                     | [AxiosRequestConfig](https://axios-http.com/docs/req_config) | :heavy_minus_sign:                                           | Available config options for making requests.                |


### Response

**Promise<[operations.ListPetsResponse](../../models/operations/listpetsresponse.md)>**


## showPetById

Info for a specific pet

### Example Usage

```typescript
import { WidgetService } from "Widget-Service";
import { ShowPetByIdRequest } from "Widget-Service/dist/sdk/models/operations";

(async() => {
  const sdk = new WidgetService();
const petId: string = "string";

  const res = await sdk.pets.showPetById(petId);


  if (res.statusCode == 200) {
    // handle response
  }
})();
```

### Parameters

| Parameter                                                    | Type                                                         | Required                                                     | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| `petId`                                                      | *string*                                                     | :heavy_check_mark:                                           | The id of the pet to retrieve                                |
| `config`                                                     | [AxiosRequestConfig](https://axios-http.com/docs/req_config) | :heavy_minus_sign:                                           | Available config options for making requests.                |


### Response

**Promise<[operations.ShowPetByIdResponse](../../models/operations/showpetbyidresponse.md)>**

