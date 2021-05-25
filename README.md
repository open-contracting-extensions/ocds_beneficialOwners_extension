# Beneficial owners

Adds a beneficialOwners array to the organization object to indicate the beneficial owners of an organization.

If beneficial ownership (BO) information is collected via contracting processes, then this extension is appropriate: for example, if tenderers are obligated to disclose their beneficial owners within their bid submission.

On the other hand, if BO information is collected in a central register via other means, then it is recommended to publish that information as a separate dataset. The BO dataset and the OCDS dataset should [identify organizations](https://standard.open-contracting.org/latest/en/schema/identifiers/#organization-ids) in the same way, so that users can cross-reference the datasets. The BO dataset can follow the [Beneficial Ownership Data Standard](https://standard.openownership.org/en/latest/).

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