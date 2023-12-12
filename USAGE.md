<!-- Start SDK Example Usage [usage] -->
```typescript
import { TahiraKhattak } from "TahiraKhattak";
import { PetType } from "TahiraKhattak/dist/sdk/models/shared";

async function run() {
    const sdk = new TahiraKhattak({
        security: {
            bearerAuth: "<YOUR_BEARER_TOKEN_HERE>",
        },
    });

    const res = await sdk.pets.createPets({
        id: 1234,
        name: "Fido",
    });

    if (res.statusCode == 200) {
        // handle response
    }
}

run();

```
<!-- End SDK Example Usage [usage] -->