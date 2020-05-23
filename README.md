# Adapter Pattern in Salesforce by Volodymyr Derkach (May 2020)

After you've pushed the medatada to the scratch org please assign the 'Admin' permission set to the user by running 
the following command in your CLI:
`sfdx force:user:permset:assign -n Admin -u <your_user_name>`

## Project Descritpion

In order to test the functionality please open the tab called 'Custom Lookup Test' in the App Launcher, click 'Open Modal'
button and play with 'Custom Lookup' input. Other form element are dummy.

The project implements a workaround of inability to create lwc components dynamically. In order to do that the lwc component
'customLookup' was wrapped into 'CustomLookupWrapper' aura component which in its turn can be created dynamically.
