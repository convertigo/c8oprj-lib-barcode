


# lib_barcode_scanner

Barcode Scanner Library


For more technical informations : [documentation](./project.md)

- [Installation](#installation)
- [Mobile Library](#mobile-library)
    - [Shared Actions](#shared-actions)
        - [barcode](#barcode)


## Installation

1. In your Convertigo Studio click on ![](https://github.com/convertigo/convertigo/blob/develop/eclipse-plugin-studio/icons/studio/project_import.gif?raw=true "Import a project in treeview") to import a project in the treeview
2. In the import wizard

   ![](https://github.com/convertigo/convertigo/blob/develop/eclipse-plugin-studio/tomcat/webapps/convertigo/templates/ftl/project_import_wzd.png?raw=true "Import Project")
   
   paste the text below into the `Project remote URL` field:
   <table>
     <tr><td>Usage</td><td>Click the copy button at the end of the line</td></tr>
     <tr><td>To contribute</td><td>

     ```
     lib_barcode_scanner=https://github.com/convertigo/c8oprj-lib-barcode.git:branch=master
     ```
     </td></tr>
     <tr><td>To simply use</td><td>

     ```
     lib_barcode_scanner=https://github.com/convertigo/c8oprj-lib-barcode/archive/master.zip
     ```
     </td></tr>
    </table>
3. Click the `Finish` button. This will automatically import the __lib_barcode_scanner__ project


## Mobile Library

Barcode Scanner Demo Application

### Shared Actions

#### barcode

### Barcode Scanner SharedAction

Ctrl + drag the 'barcode' SharedAction to your project to invoke the action and start scanning.  
The scanning result is saved in the local page variable named 'c8o_barcode_result' and in its resolve. Child components can use TS 'out' to get the result object.  
It contains the 'text', 'format' and 'cancelled' keys.

**variables**

<table>
<tr>
<th>name</th><th>comment</th>
</tr>
<tr>
<td>disableAnimations</td><td>iOS</td>
</tr>
<tr>
<td>disableSuccessBeep</td><td>iOS and Android</td>
</tr>
<tr>
<td>formats</td><td>default: all but PDF_417 and RSS_EXPANDED</td>
</tr>
<tr>
<td>mocked_cancel</td><td>The mocked cancel response for the barcode action in case of running not supported platform. Must be a boolean.</td>
</tr>
<tr>
<td>mocked_format</td><td>The mocked format response for the barcode action in case of running not supported platform. Must be a string.</td>
</tr>
<tr>
<td>mocked_text</td><td>The mocked text response for the barcode action in case of running not supported platform. Must be a string.</td>
</tr>
<tr>
<td>orientation</td><td>Android only (portrait|landscape), default unset so it rotates with the device</td>
</tr>
<tr>
<td>preferFrontCamera</td><td>iOS and Android</td>
</tr>
<tr>
<td>prompt</td><td>Android</td>
</tr>
<tr>
<td>resultDisplayDuration</td><td>Android, display scanned text for X ms. 0 suppresses it entirely, default 1500</td>
</tr>
<tr>
<td>saveHistory</td><td>Android, save scan history (default false)</td>
</tr>
<tr>
<td>showFlipCameraButton</td><td>iOS and Android</td>
</tr>
<tr>
<td>showTorchButton</td><td>iOS and Android</td>
</tr>
<tr>
<td>torchOn</td><td>Android, launch with the torch switched on (if available)</td>
</tr>
</table>



