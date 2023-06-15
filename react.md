>API Call Using React Hook:

```javascript
import { useEffect, useState } from 'react';

function APICall() {
  const [apiInfo, setApiInfo] = useState();

  useEffect(() => {
    async function fetchAPI() {
      const response = await fetch('/url');
      const fetchedAPI = await response.json();
      setApiInfo(fetchedAPI);
    }

    fetchAPI();
  }, []);

  return (
    <div></div>
  );
}
```
