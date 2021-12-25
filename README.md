# Abort Controller

- To cancel an ongoing `fetch` request.

- Create a controller: `const controller = new AbortController()`.

- When `abort()` is called, `controller.signal` emits the "abort" event, and the `controller.signlar.aborted` property becomes true.

- You would pass `controller.signal` as an option to fetch (signal option)

- To abort you would call `controller.abort()` to cancel the request.

- An error will be thrown with the name `AbortError`.

- Also scalable, you can abort multiple fetches at the same time if they use the same signal.
