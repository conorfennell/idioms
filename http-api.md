### API Design Guidelines

1. **URL Case Sensitivity**: Use lowercase `/items` instead of `/Items` to avoid ambiguity around URL case-sensitivity.

2. **Plurality and Exceptions**: Prefer plural forms `/items` over singular `/item`, with exceptions for edge cases such as `/health` and `/config`.

3. **CRUD Paradigm**: Stick to nouns and use the HTTP verb to denote the action, except when adding non-CRUD elements to your API.

4. **Resource Identifiers**: For individual resources, include resource identifiers in the path (e.g., `/items/22`) instead of in the query parameters (`/items?id=22`).

5. **Search and Filtering**: The query part of the URL is reserved for search and filtering, typically used with resource list endpoints (e.g., `/items?attribute_a=anna&limit=20`).

6. **Compound Nouns**: Use a hyphen to separate compound words (e.g., `/legal-items/33`).

7. **Standard Response Codes**: For successful `GET` requests, return a `200` status code.

---