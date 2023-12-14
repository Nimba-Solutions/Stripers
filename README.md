# Stripers

Add a brief description of this project here, in Markdown format.
It will be shown on the main page of the project's GitHub repository.

## Development

To work on this project in a scratch org:

1. [Set up CumulusCI](https://cumulusci.readthedocs.io/en/latest/tutorial.html)
2. Run `cci flow run dev_org --org dev` to deploy this project.
3. Run `cci org browser dev` to open the org in your browser.

## Release

To release this project as a 2nd Generation Unlocked Package:

1. Run `cci flow run dependencies --org beta --debug` to prepare a "beta packaging scratch org"
2. Run `cci flow run release_unlocked_beta --org dev --debug` to deploy this project.
3. Run `cci org browser dev` to open the org in your browser.
4. Thoroughly test all functionality.
5. Run `cci flow run release_unlocked_production --org release`