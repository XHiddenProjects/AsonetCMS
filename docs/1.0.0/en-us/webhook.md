# Webhooks

Webhooks are easy use for creating plugins, this only requires function labels and let us do the work.

### Valid Webhooks

| Name | Description | Usage |
| ---- | ----------- | ----- |
| meta | Loads meta tags in the header | `*\meta()` |
| css  | Executes code as a CSS code at the head tag | `*\css()` |
| js   | Executes script after page load | `*\js()` |
| beforePage | Loads code before the page loads up | `*\beforePage()` |
| afterPage | Loads code after the page us loaded up | `*\afterPage()` |
| dbnav | Loads up code at the dashboard navagation bar | `*\dbnav()` |
| profileSettings | Loads code at the profile settings | `*\profileSettings()` |
| profile | Loads code on the profile page | `*\profile(string $username)` |
| editor | Loads up elements in the message editor | `*\editor(string $codeLang)` | 
| topicHead(**Body/Foot**) | Loads the elements in the topic | `*\topicHead[Body/Foot](string $topicid, string $title, string $author)` |
| install | Executes code when plugin is installed | `*\install()` |
| loaded | Executes code when plugin is loaded [enabled\disabled] | `*\loaded()` |
| config | Loads configuration for plugins | `*\config()` |
| view | Displays program at the _/viewer.php/{plugin}_ | `*\view()` |
