# dcf-hub

Community collector templates for [dcf](https://github.com/zephschafer/dcf).

## Usage

```bash
dcf import stack_exchange
dcf import nws
```

Each import copies a single YAML template into your project's `collectors/` directory. After importing, fill in any credentials shown in the output and run:

```bash
dcf run <collector_name>
```

## Available collectors

| Name | Source | Auth |
|---|---|---|
| `stack_exchange` | Stack Exchange API | None |

## Contributing

1. Fork this repo
2. Add your collector as `collectors/<name>.yml`
3. Open a pull request

Templates should use `{{ env.VAR }}` for any credentials and include a `description:` field explaining what data is collected. See [existing collectors](collectors/) for examples.
