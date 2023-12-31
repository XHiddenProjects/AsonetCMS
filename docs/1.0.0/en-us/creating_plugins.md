# Creating plugins

This is a whole page for starting up creating your own addon to the software and will require you need to know the [Webhooks](#webhooks). This will go at a step-by-step process with some example to the code.
***
_**ALL NAMES ARE CASE-SENSIATIVE!**_

1. Startup
    1. Locate the _/plugins_ folder 
    2. Create a folder with your `{plugin_name}`
    3. Create a file inside that folder name `{plugin_name}.plg.php`
    4. Open it up to continue
2. Writting the code
    1. For the first step, you must include the **ASONET PLUGIN NAMESPACE** which can be defined as this `namespace asonet\Plugins;`
    2. Next, set your plugins class by typing this
     ```php
      class (plugin_name){
         protected static $baseName = '{plugin_name}';
        # content
     }
     ```
    3. Inside the class you would want to return the plugin name; type this
       ```php
        
        public function __construct()
        {
            return self::$baseName;
        }
       ```
    4. Installation to your plugin: By writting this your plugin will automatically inject the settings that can be preformed on the configuration by default
     ```php
      public static function install(){
        $data[self::$baseName.'state'] = false; # Sets the state of the plugin to false, which means it's off
        $data[self::$baseName.'canDisabled'] = true; # Can disabled is weather or not it can be changed
        $data[self::$baseName.'Config'] = true; # Allows configuration to your plugin.
        return $data;
      }
     ```
    5. If you want to add more and do more stuff, here is the format to allow that access
     ```php
      public static function {webhooks}(param){
        # Enter code
     }
     ```
