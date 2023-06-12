>Front End Form Submit and API Call

```javascript
import { useState } from "react";

function App() {
  const [field, setField] = useState("");

  async function InputSubmit(event) {
    event.preventDefault();

    const response = await fetch("http://localhost:0000/api/submit", {
      method: "POST",
      headers: {
        "Content-Type": "application/json",
      },
      body: JSON.stringify({
        field,
      }),
    });

    const APIResponse = await response.json();
  }

  return (
    <div>
      <form onSubmit={InputSubmit}>
        <input
          value={field}
          onChange={(e) => setField(e.target.value)}
          type="text"
          placeholder="Text"
        />

        <br />

        <input type="submit" value="Submit" />
      </form>
    </div>
  );
}

export default App;
```

>Back End API Handler

```javascript
app.post("/api/submit", async (req, res) => {
  const fieldValue = req.body.field;

  res.json({ status: "ok" });
});
```
