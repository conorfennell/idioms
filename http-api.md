Item 1: Use lowercase `/items` not `/Items` to avoid the ambiguity around URL case-sensitivity

Item 2: Use plural `/items` not `/item` and edge case singular e.g. `/health` and `/config`

Item 3: CRUD paradigm only use nouns and leave action be the HTTP verb, unless you are adding something to your API that doesn't fit the CRUD paradigm

Item 4: For individual resources, include resource identifiers in the path, not the query. `/items/22` instead of `/items?id=22`

Item 5: Query part of the URL is for search and filtering and commonly used with a resource list endpoint `/items?attribute_a=anna?limit=20`

Item 6: Nouns that are compounds of multiple words should a hyphen as a separator `/legal-items/33`

Item 7: GET return 200
