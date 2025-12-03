# Call24x7 Documentation

This repository contains the documentation for Call24x7.AI - an AI-driven phone calls platform that enables businesses to manage outbound and inbound calls using highly adaptable AI agents.

## Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mintlify) to preview the documentation changes locally. To install, use the following command:

```
npm i -g mintlify
```

Run the following command at the root of your documentation (where mint.json is):

```
mintlify dev
```

The documentation website will be available at `http://localhost:3000`.

### Custom Ports

You can use the `--port` flag to customize the port Mintlify runs on:

```
mintlify dev --port 3333
```

## Publishing Changes

Changes will be deployed to production automatically after pushing to the default branch when using Mintlify's GitHub integration.

### Troubleshooting

- Mintlify dev isn't running - Run `mintlify install` to re-install dependencies.
- Page loads as a 404 - Make sure you are running in a folder with `mint.json`
- Documentation looks different locally - Update to the latest Mintlify CLI: `npm i -g mintlify@latest`

## Documentation Structure

- **Get Started**: Introduction, quick start guide, and no-code integration options
- **Essentials**: Core concepts including authentication, webhooks, agents, voice models, and integrations
- **API Reference**: Complete API documentation with endpoint details and examples
