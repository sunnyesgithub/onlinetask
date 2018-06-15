MODULE
------
Basic page node to json

CREDITS
--------
Developed by Sunny Singh Sharma <infoofsunnysharma@gmail.com>
https://www.drupal.org/u/sunnydrupal

JSON Encode URL
-----------------
URL : http://domain_name/node_json/<node_id>
test url : http://domain_name/node_json/<node_id>?key=<api_key>

REQUIREMENTS
------------
1) Alter Site information page in admin with field name 'Site API Key' under 'Site Detail' Section.

2) Make 'Site API key' is compulsory field.

3) Button text 'Save configuration' should be changed to 'Update configuration' at the time of updating key.

4) Create page using custom code which uses Site API key as parameter in URL.

5) If API key is present in URL, It would return content of content type 'Basic page' in json format.

6) If API Key is not present in URL, it would return Access denied.

7) If content type is not 'Basic page', it would return Access denied.

Reference links:
-----------------
https://api.drupal.org/api/drupal/modules%21system%21system.api.php/function/hook_menu/7.x
https://api.drupal.org/api/drupal/functions/7.x
https://www.agileana.com/blog/how-to-get-url-parameters-in-drupal-7/
https://api.drupal.org/api/drupal/modules%21system%21system.api.php/function/hook_form_alter/7.x
https://www.drupal.org/forum/support/module-development-and-code-questions/2010-04-06/solved-hooking-into-system_settings
https://api.drupal.org/api/drupal/modules%21system%21system.module/function/system_settings_form/7.x
https://www.drupal.org/docs/7/api/form-api
https://api.drupal.org/api/drupal/includes%21common.inc/function/drupal_json_output/7.x


