# Webhooks

Webhooks are easy use for creating plugins, this only requires function labels and let us do the work.

### Valid Webhooks

| Name | Description | Usage |
| ---- | ----------- | ----- |
| meta | Loads meta tags in the header | `*_meta()` |
| css  | Executes code as a CSS code at the head tag | `*_css()` |
| js   | Executes script after page load | `*_js()` |
| beforePage | Loads code before the page loads up | `*_beforePage()` |
| afterPage | Loads code after the page us loaded up | `*_afterPage()` |
| dbnav | Loads up code at the dashboard navagation bar | `*_dbnav()` |
| profileSettings | Loads code at the profile settings | `*_profileSettings()` |
| profile | Loads code on the profile page | `*_profile(string $username)` |
| editor | Loads up elements in the message editor | `*_editor()` | 
