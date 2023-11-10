<!-- Start SDK Example Usage -->
```typescript
import { WidgetService } from "Widget-Service";

(async () => {
    const sdk = new WidgetService();

    const res = await sdk.pets.createPets();

    if (res.statusCode == 200) {
        // handle response
    }
})();

```
<!-- End SDK Example Usage -->