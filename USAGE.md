<!-- Start SDK Example Usage -->


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
<!-- End SDK Example Usage -->