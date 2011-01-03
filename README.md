upForm
======
*By: Wen-Hao Lue*

upForm is a library for the DM Programming Language that handles a variety of 
HTML interfaces through the datum `/upForm`. Common functionality between 
forms are all defined for you, and the library maintains a set of critical and 
useful features while being easily extendable.

### Feature List
* Declare new interfaces by defining a child of the /upForm datum, and display it
  by simply calling `upForm()`
* Handles BYOND 4.0 browser control interfaces, and windows
* Easy definition of CSS and JavaScript code
* Handles multiple viewers at the same time
* Handles predefined and dynamic resources
* Easy implementation of HTML forms
* Contains basic time-keeping functions
 
## Example Usage

	upForm/helloworld
	  GenerateBody()
	    UpdatePage("Hello")
	
	mob/Login()
		..()
		upForm(src, /upForm/helloworld)
	
## Release History

Version 1.0 (January 21st, 2008)
* Library released

Version 1.1 (January 22nd, 2008)
* Fixed demo errors, and added more comments to demo code (Gughunter)
* Documentation proofread for accuracy (Gughunter)

Version 1.2 (March 21st, 2008)
* Fixed demo interface anchor for text box, and modified demo code
* Removed unneccessary assertion text being sent to the default
   output interface (old testing code)
* Renamed javascript functions for quick linking to be shorter (all links
  are now prefixed with 'upF_' rather than 'upForm_')
* Added new javascript function `upF_sAction()`, which allows a link to be sent
  with an action and value param

Version 1.3 (May 17th, 2008)
* `upForm_formatViewerList()` was not completly formatting all objects
  in the list