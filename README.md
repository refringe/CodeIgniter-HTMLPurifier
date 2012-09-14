Codeigniter HTMLPurifier Helper
-------------------------------
 - Purify input using the HTMLPurifier standalone class.
 - Easily use multiple purifier configurations.

Installation
------------
 - Copy HTMLPurifier helper to:  
   `./application/helpers/htmlpurifier_helper.php`
 - Download the [HTMLPurifier standalone version](http://htmlpurifier.org/download) and copy to:  
   `./application/third_party/htmlpurifier-4.4.0-standalone/*`
 - Make the following directory writable by your web server:  
   `./application/third_party/htmlpurifier-4.4.0-standalone/standalone/HTMLPurifier/DefinitionCache/Serializer`
   Permission 775 (-rwxrwxr-x) is usually sufficient, depending on your web server configuration.

Usage
-----
 - Create and customize configurations
 - Use the following code to purify:  
   `$this->load->helper('htmlpurifier');`  
   `$clean_html = html_purify($dirty_html);`  
   Or to use a config:  
   `$clean_html = html_purify($dirty_html, 'comment');`