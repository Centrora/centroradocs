Joomla Fabrik Component Conflict
*********************************

If you are using the Joomla! Fabrik Component and encounter the following error in the browser console,
::

   Error: Mismatched anonymous define() module: function init($, undefined) {     ....require.js

This indicates the Fabrik Component System plugin is causing the conflicts with Centrora Security.

To resolve this, please open this file,
::

   /plugins/system/fabrik/fabrik.php

Find the following lines,
::

   public function onAfterRender()
   {
   // Could be component was unistalled but not the plugin
   if (!class_exists(‘FabrikString’))
   {
   return;
   }

Add the following codes to the plugin file,
::

   $option=JRequest::getVar(“option”,“”);
   if ($option ==‘com_ose_firewall’)
   { return; }

This will sort out the issue.