# MC Mod Scanner

## Overview
This is a basic tool for assisting in narrowing down what mods in a modpack are client-sided. By uploading a modlist generated from your modpack, this tool categorizes mods based on their likelihood of being client-sided using a predefined configuration file (`config.json`).

## Features
- **Simple File Upload**: Upload your `modlist.html` file to get instant categorization.
- **Automatic Categorization**: Mods are grouped into categories such as `Known`, `High Probability`, `Medium Probability`, `Low Probability`, `Unknown`, and `Not`.

## Usage
1. Open the website hosted on GitHub Pages.
2. Ensure you have a `modlist.html` file generated from your modpack.
3. Click the `Upload` button and select your `modlist.html` file.
4. View the categorized results instantly.

## Categories
The mods will be grouped into the following categories:
- **Known**: Mods explicitly listed as client-sided in the configuration.
- **High Probability**: Mods likely to be client-sided based on keywords.
- **Medium Probability**: Mods that might be client-sided.
- **Low Probability**: Mods unlikely to be client-sided.
- **Unknown**: Mods that could not be categorized.
- **Not**: Mods explicitly listed as not client-sided.

## Configuration
The tool uses a `config.json` file to define known mods and categorization rules. You can update this file to customize categorization for your use case.

### Example `config.json`
```json
{
  "Known": ["optifine", "modmenu"],
  "High": ["fps", "sound"],
  "Medium": ["menu", "zoom"],
  "Low": ["server", "biome"],
  "Not": ["industrialcraft", "buildcraft"]
}
```

## License
This project is open-source and can be freely modified and distributed under the [Unlicense license](LICENSE).

## Contributions
Contributions are welcome! Feel free to submit a pull request or open an issue for suggestions and improvements.
