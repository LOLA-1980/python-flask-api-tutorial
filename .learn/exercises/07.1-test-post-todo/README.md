# `07.1` Test your endpoint

This is what you should have so far for the `POST /todos` endpoint. Take some time to analyze each line and ask questions where needed:

```python
@app.route('/todos', methods=['POST'])
def add_new_todo():
    request_body = request.json
    print("Incoming request with the following body", request_body)
    return 'Response for the POST todo'
```

Use Postman, Insomnia or any other API Request Builder that you like to test your API.

|  |  |
| ------ | -------- |
| Method | Post |
| URL: | /todos |
| Request Body | `{ "done": true, "label": "Sample Todo 1" }` |

