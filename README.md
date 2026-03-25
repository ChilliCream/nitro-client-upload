# Nitro Client Upload

A GitHub Action that uploads client operations to the Nitro registry.

## Usage

```yaml
- uses: ChilliCream/nitro-client-upload@v16
  with:
    tag: <tag>
    client-id: <client-id>
    api-key: <api-key>
    operations-file: ./path/to/operations.json
```

## Inputs

| Name              | Required | Description                                   |
| ----------------- | -------- | --------------------------------------------- |
| `tag`             | Yes      | The tag of the client version                 |
| `client-id`       | Yes      | The ID of the client                          |
| `api-key`         | Yes      | API key for authentication                    |
| `operations-file` | Yes      | The path to the JSON file with the operations |
| `cloud-url`       | No       | The URL of the Nitro registry                 |

If you self-host Nitro or use a dedicated hosted instance, you can specify the `cloud-url` input to point to your instance.
