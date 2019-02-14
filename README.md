# GoogleAPIClientForREST-Calendar

Example App to implement Google Sign-In and use Google Calendar API with **Pods version: ~> 1.3.** 
Using **Swift 4.x**

# Instructions

 1. Install pod dependencies from 'Podfile'
 2. Add missing classes in Bridging Header (See Fix error)
 3. Download from Firebase Console the GoogleService.plist and add it to your project.
 4. In 'Info' section of your configuration project add a new URL Type with the REVERSE_CLIENT_ID of your GoogleService.plist
 

# Fix error

In some cases you may find this error message: 

> Value of type 'GTLRCalendarService' has no member 'authorizer'

To solve this, just add this lines in **Swift Bridging Header** after installed your pod dependencies: 

    #import <GTMSessionFetcher/GTMSessionFetcher.h> 
    #import <GTMSessionFetcher/GTMSessionFetcherService.h>
