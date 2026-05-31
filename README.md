```sh
# Terminal 1 - To run the server.
cargo watch -q -c -w src/ -w .cargo/ -x "run"

# Terminal 2 - To run the quick_dev.
cargo catch -q -c -w examples/ -x "run --exmaple quick_dev"
```
