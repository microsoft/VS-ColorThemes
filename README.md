## Using this Extension

1. Download and install the extension
1. Restart Visual Studio
1. Navigate to _Tools > Options > Environment > General_ and select your color theme:
   ![](https://user-images.githubusercontent.com/350947/69694799-25e2a680-112e-11ea-85d0-f6fe476168d5.png)

## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.microsoft.com.

When you submit a pull request, a CLA-bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.


## Steps to create a custom theme for this project
0. Prerequisite: Install the Color Themes Editor extension for Visual Studio 2017 (https://marketplace.visualstudio.com/items?itemName=VisualStudioPlatformTeam.VisualStudio2017ColorThemeEditor).
1. Go to Tools -> Customize Colors.
2. Hover over the original theme you want to edit and click on 'Create Copy of Theme'.
3. Hover over the Custom Theme you created, and click on 'Edit Theme'.
4. Edit the colors to create a new custom theme.
5. Click on the Export Theme icon at the top and save the new theme as a vstheme. Then rename the file to xml.
6. Create a fork of the repo for your theme and add the file within the Themes folder.
7. Also update:

    a. The ThemeRegistration.pkgdef file (Please add entries in alphabetical order and rootkey token from the GUID of the xml file)
    
    b. The VSColorThemes.csproj file (include the theme file to the project)
    
    c. The source.extension.manifest (don’t update the version – just add to the assets)
8. Open a pull request and sign the Contributor License Agreement. We'll work with you to get it merged :)
