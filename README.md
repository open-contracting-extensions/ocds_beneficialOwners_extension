# Beneficial Owners
Adds a beneficialOwners array to the organization object to indicate the beneficial owners of a organization.

At present this extension includes the identifier, name and nationality of each beneficial owner, but this may be further extended with additional information about each person if needed.

This extension should only be used if the information about the beneficial onwers is only available during the contracting process life-cycle. If there is a separate beneficial ownership registry, the recommended approach is to publish a separate dataset using the [Beneficial Ownership Data Standard](http://standard.openownership.org/).

## Example

```json
{
  "parties": [
    {
      "id": "AHL",
      "name": "Alpha Holdings Ltd",
      "beneficialOwners": [
        {
          "id": "1",
          "name": "Juan Perez",
          "identifier": {
            "scheme": "PRY-IDCARD",
            "id": "12345"
          },
          "nationality": "PY"
        }
      ]
    }
  ]
}
```

## Issues

Report issues for this extension in the [ocds-extensions repository](https://github.com/open-contracting/ocds-extensions/issues), putting the extension's name in the issue's title.