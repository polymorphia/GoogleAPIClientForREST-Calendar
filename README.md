# GoogleAPIClientForREST-Calendar
Example App to implement Google Sign-In and use Google Calendar API with Pods version: ~> 1.3.
Using Swift 4.x

In some cases you may find this error message:
"Value of type 'GTLRCalendarService' has no member 'authorizer'"

To solve this, just add this lines in Swift Bridging Header:
#import <GTMSessionFetcher/GTMSessionFetcher.h>		
#import <GTMSessionFetcher/GTMSessionFetcherService.h>
