# Translations

Thanks to everyone who helped translate the app!

You are welcome to help translate the app at [Weblate](https://hosted.weblate.org/projects/losslesscut/losslesscut/). Weblate will automatically push translations as a Pull Request in this repo, but this PR is not merged immediately by maintainers.

Master language is english.

## Testing translations locally

To test new weblate translations you made in the app itself, you need to:
1. Download the translation for your language from Weblate: **Files -> Download translation**
2. Rename the downloaded `.json` file to: `translation.json`
3. Create a [folder structure](https://github.com/mifi/lossless-cut/tree/master/public/locales) somewhere on your computer that looks like this:
```
translations/locales/localeCode
```
You can find a list of the available [`localeCode`s here](https://github.com/mifi/lossless-cut/tree/master/public/locales). In our example we will use `nb_NO` (Norwegian) with this path:
```
/Users/mifi/Desktop/translations/locales/nb_NO
```

4. Now move your `translation.json` file into the folder:
```
/Users/mifi/Desktop/translations/locales/nb_NO/translation.json
```

5. Now run LosslessCut from the [command line](cli.md), with the special command line argument `--locales-path`. Use the path to the **folder containing the locales folder**, e.g.:
```bash
./LosslessCut --locales-path /Users/mifi/Desktop/translations
```

Now LosslessCut will use your language file.