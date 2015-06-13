Personnalisation
===========

Choix du Thème
-------------

Il existe un gimmick `ThemeChooser` qui ajoutera un sous-menu à la barre de navigation avec touts les thèmes disponibles. L'activer en ajoutant

    [gimmick:themechooser](Choose theme)

au fichier `navigation.md` (ou dans chaque page individuellement).

### Sélectionner un thème

Vous pouvez installer manuellement un thème spécifique qui sera utilisé si le gimmick  ThemeChooser n'est pas utilisé ou installé dans le thème par default :

    [gimmick:theme](flatly)

Cela installera `flatly` comme thème par défaut. Vous pouvez consulter la liste des noms de thème dans le gimmick `ThemeChooser` ou sur cette page (sélectionnez `Change theme` dans la barre de navigation).

Pour appliquer le thème globalement sur chaque fichier, déposer l'entrée dans le fichier  `navigation.md`. Vous pouvez aussi changer le mode "inverse" , qui changera les colors de certains themes (voir <http://www.bootswatch.com/> pour les details)

    [gimmick:theme (inverse: true)](flatly)

Note: Only the default `bootstrap` theme is bundled with MDwiki and available offline. All other themes require internet connection, as the styles are dynamically loaded on demand.

Configuration
-------------

You can create a `config.json` file in the same folder as the `mdwiki.html` file which is then used for configuration. The file has to be valid JSON. Currently these options are available:

  * `"useSideMenu": false` - disable the side navigation
  * `"lineBreaks": "original"` - Instead of using the [GFM] line breaks, use the original line breaking as [introduced by John Gruber][DaringFireball]:
    * line breaks in the markdown files are ignored, except if a line ends with two spaces
    * Default is `lineBreaks: "gfm"` (line breaks in markdown will create a new paragraph)
  * `"additionalFooterText": ""`
    * Can be used to add text to the copyright footer at the bottom, like custom copyright notices.
    * Example: `additionalFooterText: "All content and images &copy; by John Doe"`
    * Default: `""` (empty string)
  * `"anchorCharacter": "&para;"`
    * The character/text displayed and used as a hyperlink when hovering over headings.
    * Unicode characters can be used in HTML notation. Example: `&#x2693;` will render as &#x2693;
    * Default: The pilcrow (paragraph) sign: &para;
  * `"title": "ACME Industries Wiki"`
	* Changes the title of the webpage.
	* Default: `"MDWiki"`
	* Note - this parameter does not change the title of your wiki in Google search results. Edit `mdwiki.html` directly to correct this. ([Issue #58](https://github.com/Dynalon/mdwiki/issues/58)) 

A sample `config.json` might thus look like this:

```javascript
{
    "useSideMenu": true,
    "lineBreaks": "gfm",
    "additionalFooterText": "All content and images &copy; by John Doe",
    "anchorCharacter": "#"
}
```

Note: More configuration options will be available in future versions of MDwiki.

Hint: It is adviced that you create an empty config.json in each cases, to avoid 404 errors which will not get cached by your browser. Having an `config.json` file present thus will speed up page loading (even if its empty).

  [GFM]: https://help.github.com/articles/github-flavored-markdown
  [DaringFireball]: http://daringfireball.net/projects/markdown/
