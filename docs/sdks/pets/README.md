# Pets

## Overview

the pet grouping

### Available Operations

* [createPets](#createpets) - createPets
* [listPets](#listpets) - listPets
* [showPetById](#showpetbyid) - showPetById

## createPets

Create a pet and key characteristics

### Example Usage

```typescript
import { TahiraKhattak } from "TahiraKhattak";
import { CreatePetsResponse } from "TahiraKhattak/dist/sdk/models/operations";
import { PetType } from "TahiraKhattak/dist/sdk/models/shared";

const sdk = new TahiraKhattak({
  security: {
    bearerAuth: "",
  },
});

sdk.pets.createPets({
  id: 1234,
  name: "Fido",
  type: PetType.Cat,
}).then((res: CreatePetsResponse) => {
  if (res.statusCode == 200) {
    // handle response
  }
});
```

### Parameters

| Parameter                                                    | Type                                                         | Required                                                     | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| `request`                                                    | [shared.Pet](../../models/shared/pet.md)                     | :heavy_check_mark:                                           | The request object to use for the request.                   |
| `config`                                                     | [AxiosRequestConfig](https://axios-http.com/docs/req_config) | :heavy_minus_sign:                                           | Available config options for making requests.                |


### Response

**Promise<[operations.CreatePetsResponse](../../models/operations/createpetsresponse.md)>**


## listPets

List all pets

### Example Usage

```typescript
import { TahiraKhattak } from "TahiraKhattak";
import { ListPetsResponse } from "TahiraKhattak/dist/sdk/models/operations";

const sdk = new TahiraKhattak({
  security: {
    bearerAuth: "",
  },
});

sdk.pets.listPets({
  limit: 715190,
}).then((res: ListPetsResponse) => {
  if (res.statusCode == 200) {
    // handle response
  }
});
```

### Parameters

| Parameter                                                                | Type                                                                     | Required                                                                 | Description                                                              |
| ------------------------------------------------------------------------ | ------------------------------------------------------------------------ | ------------------------------------------------------------------------ | ------------------------------------------------------------------------ |
| `request`                                                                | [operations.ListPetsRequest](../../models/operations/listpetsrequest.md) | :heavy_check_mark:                                                       | The request object to use for the request.                               |
| `config`                                                                 | [AxiosRequestConfig](https://axios-http.com/docs/req_config)             | :heavy_minus_sign:                                                       | Available config options for making requests.                            |


### Response

**Promise<[operations.ListPetsResponse](../../models/operations/listpetsresponse.md)>**


## showPetById

Info for a specific pet

### Example Usage

```typescript
import { TahiraKhattak } from "TahiraKhattak";
import { ShowPetByIdResponse } from "TahiraKhattak/dist/sdk/models/operations";

const sdk = new TahiraKhattak({
  security: {
    bearerAuth: "",
  },
});

sdk.pets.showPetById({
  petId: "quibusdam",
}).then((res: ShowPetByIdResponse) => {
  if (res.statusCode == 200) {
    // handle response
  }
});
```

### Parameters

| Parameter                                                                      | Type                                                                           | Required                                                                       | Description                                                                    |
| ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ |
| `request`                                                                      | [operations.ShowPetByIdRequest](../../models/operations/showpetbyidrequest.md) | :heavy_check_mark:                                                             | The request object to use for the request.                                     |
| `config`                                                                       | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                   | :heavy_minus_sign:                                                             | Available config options for making requests.                                  |


### Response

**Promise<[operations.ShowPetByIdResponse](../../models/operations/showpetbyidresponse.md)>**
