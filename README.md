# ai-tools-table

A table of AI coding tools for developers. Built using [AG Grid](https://github.com/ag-grid/ag-grid).

## Adding a dataset

Datasets are stored in the `dist/datasets` folder as JSON files. To add a new dataset, create a new JSON file in this folder with the following structure:

```jsonc
[
    {
        "avatar": "relative/path/to/avatar.webp",
        "Name": "Tool Name",
        "Plan": "Tool Plan",
        "Company": "Company Name",
        "Country": "Company Country",
        "Hosting": "Hosting Type",
        "DataCenter": "Data Center Location",
        "DataRetentionDays": 0, // Number of days prompts and responses are stored
        "UserPromptsResponses": false, // Whether user prompts and responses are used for training
        "Non-permissivelyLicensedCode": true, // Whether the underlying LLM is trained on non-permissively licensed code
        "SuggestionsForNewAndExistingCode": true, // Whether the tool provides suggestions for new and existing code
        "Explanations": true, // Whether the tool provides explanations for its suggestions
        "IDEAutocomplete": true, // Whether the tool provides autocomplete in the IDE
        "IDEChat": true, // Whether the tool provides chat in the IDE
        "IDEInlineChat": false, // Whether the tool provides inline chat in the IDE
        "VSCode": true, // Whether the tool supports VSCode
        "VisualStudio": true, // Whether the tool supports Visual Studio
        "Rider": true, // Whether the tool supports Rider
        "Eclipse": false // Whether the tool supports Eclipse
    },
    ... // More tools
]
```

Then add the file to the `datasets` array in the `dist/datasets.json` file.

## License

MIT
