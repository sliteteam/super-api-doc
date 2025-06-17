### Updating the API

:warning::warning: We have to update manually the openapi doc (some issue with mintlify, the right navigation structure doesnt work with auto generated docs ) :warning::warning:

1. Update the doc, copy paste https://api.super.work/super-openapi.json in ./super-openapi.json
2. Run `npx @mintlify/scraping openapi-file https://api.super.work/super-openapi.json -o api-reference`
3. If endpoints have been added / removed, update the `docs.json` file section with the new page list.

### Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mintlify) to preview the documentation changes locally. To install, use the following command

```
npm i -g mintlify
```

Run the following command at the root of your documentation (where docs.json is)

```
mintlify dev
```
