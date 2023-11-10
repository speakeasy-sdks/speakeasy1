<!-- Start SDK Example Usage -->
```typescript
import { TahiraKhattak } from "TahiraKhattak";
import { PetType } from "TahiraKhattak/dist/sdk/models/shared";

(async () => {
    const sdk = new TahiraKhattak({
        security: {
            bearerAuth: "",
        },
    });

    const res = await sdk.pets.createPets({
        id: 1234,
        name: "Fido",
    });

    if (res.statusCode == 200) {
        // handle response
    }
})();

```
<!-- End SDK Example Usage -->