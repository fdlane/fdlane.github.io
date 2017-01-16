---
layout: page
title: VBSmgr MS Access
showInNav: false
---
This version of the VBS Manager solution is a MS Access application that consists of two database files. A User Interface database and Backend database where the data is stored.

The User Interface or Front End of the application is named `VbsMgr.mdb`. This is the file that users will open. All users can open the same database file or a copy can be saved on each users’ machine.

Your data is stored in a file named `VbsMgr_BE.mdb`. The `_BE` portion of the file name is used to indicate the ‘Backend’ of the application. This is where all your data is stored and SHOULD be routinely backed up.

## Installation steps
1. [Download VbsMgr.zip](https://cdn.rawgit.com/fdlane/vbsmgr-ms-access/be70ac31/VbsMgr.zip) 
1. Unzip to a location on your harddrive. These instructions assume the location is  `c:\fdlane\vbsmgr\`
1. Open file `c:\fdlane\vbsmgr\VbsMgr.mdb`
1. On the MS Access top menu,  select Database Tools, Linked Table Manager
1. In the Linked Table Manager dialog box
1. click Select All button
1. check ‘Always prompt for new location’  checkbox
1. click OK button
1. Go to folder `c:\fdlane\VbsMgr\`
1. Click on `VbsMgr_BE.mdb`
1. Click on the Open button
>Note: You should see the message…
>‘All selected linked tables were successfully refreshed’
1. Click OK button on the message box
1. Click Close on the ‘Linked Table Manager’ dialog box
1. Close and Re-Open `c:\fdlane\vbsmgr\VbsMgr.mdb`

> #### Security Warning
> You may see this warning
> ![](/images/security-warning-ms-access.png){: .image-left }
> 
> #### Steps to disable warning
> 1. on the warning message bar, click the Options… button
> 1. in the Microsoft Office Security Options dialog box, click the ‘Open the Trust Center’ link
> 1. in the Trust Center dialog box, click the ‘Trusted Locations’ link
> 1. click the ‘Add new location…’ button
> 1. in the Path: field, enter `c:\fdlane\vbsmgr`
> 1. click OK to dismiss all the dialog boxes
> 1. reopen the application `VbsMgr.mdb`

## VBS Event Setup
- Open the application from `c:\fdlane\vbsmgr\VbsMgr.mdb`
- Enter data about your event
- Enter Children and Workers
- Print Reports
- Change the lives of as many Children as you can

### Pre-populated Tables

The following tables are populated with commonly used values and can be modified to meet your requirements:

- Ages
- Locations
- Neighborhood Types
- Worker Types
> Note: Do not delete Neighborhood types “Apartment” and “Subdivision”, these types are used to sort the roster reports for the bus routes. This makes for Happy Bus drivers!

### Classes

Enter all the classes for your VBS.  You can change the Age, Location, Master Teacher and Class workers at a later time

### Neighborhoods

Enter all of the neighborhoods that your VBS event will likely serve. Set the Neighborhood Type (Reports will sort Apartments alphabetically by Child name, and Subdivisions will sort numerically by house number). Makes for Happy Bus drivers!

You can add the neighborhood to a route later as you figure out bus capacity and a route’s current registration count.

### Children

You are now ready to start entering the children who are registered to your event.

### Buses

Enter your buses and their capacity

### Routes

Enter your routes,  assign a bus, and begin to assign neighborhoods.  This is where the fun begins…As you register children for each neighborhood, you will need to add/remove neighborhoods from a route or change the bus to a larger/smaller bus.

### Workers

You are now ready to start entering the workers who will be helping with the event.  Assign the workers to classes and buses.

### Reports

- Route Report
- Bus Roster
- Class Roster

### Attendance

Record attendance each day for children and workers.