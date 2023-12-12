<!-- Start SDK Example Usage [usage] -->
```typescript
import { WidgetService } from "Widget-Service";

async function run() {
    const sdk = new WidgetService();

    const res = await sdk.pets.createPets();

    if (res.statusCode == 200) {
        // handle response
    }
}

run();

```
<!-- End SDK Example Usage [usage] -->