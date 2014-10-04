4. System architecture

The system is a mobile app that enables users to scan rooms, add virtual decorations to them from a catalog, and then view and share their interior designs. They can also save and load files to the local filesystem or a remote database. Certified designer users can also add entries to the catalog. 


4.1. Modules

The application is divided into the following modules:


Scanning
Preparing a virtual representation of a room for decorating using camera and gyroscope.
 * Create a scan


Decorating
Placing 3D-modelled furniture into a scanned room.
 * Select an item
 * Move an item
 * Remove an item

    Catalog
    A list of models available for placement.
     * Select an entry
     * Place item
     * Go to webstore


Previewing
Viewing a previously created design.
 * View a design

   Sharing
   Publish a design in social media
    * Share a design


File operations
Saving and opening previously created scans and designs.

    Local Files
    Operations using the local filesystem.
     * Save a file
     * Open scan in design module
     * Open design in view module

    Remote Files
    Operations using the remote database.
     * Upload a file
     * Open scan in design module
     * Open design in view module
     * Remove a file


Accounts
Operations that deal with the user accounts, such as logging in.
 * Register
 * Log in
 * Log out
 * Change user type(admin only)


Additionally designers and administrators have access to the following module:


Edit catalog
Add, edit and remove catalog entries.
 * Add entry
 * Edit entry
 * Remove entry


4.2. Data types

The system uses four specified types of data in its operations - the scan file, the design file, the user account and the catalog item. 

Scan file
A panoramic representation of a room with guides for 3d object placement. Created in the scanning module using a camera and a gyroscope, as well as user input as necessary.

Design file
A data markup file denoting a room file and the location of catalog items in it. Created in the design module based by the user.

User account
Database information containing login credentials and user privileges.

Catalog item
An entry in the furniture catalog consisting of a 3D-model and assorted metadata, including a link to the designer's webstore or site. Created by designers in the edit catalog module.