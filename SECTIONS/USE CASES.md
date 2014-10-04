3. Use cases

3.1. User groups

The users of DecorGlass come in the following four varieties: Guest, User, Designer, Administrator
<table>
<tr>
<td>Guest</td>
<td>An unregistered user of the application. Has access to most functionalities, but cannot use remote file storage or social media sharing. Has the unique ability to register and log in.</td>

<tr>
<td>User</td>
<td>The basic user class. Has access to all functionality except catalog editing.</td>
</tr>

<tr>
<td>Designer</td>
<td>A certified designer, who can add items to the catalog as well as edit and remove their own entries. Also has access to all normal functionality.</td>
</tr>

<tr>
<td>Administrator</td>
<td>A person in charge of maintaining the service. Can edit and remove all catalog entries and change the privileges of other users. </td>
</tr>
</table>

3.2. Use case diagram


<img src="https://raw.githubusercontent.com/SmartDecor/DecorGlass/master/SECTIONS/usecases_diagram.png">Use case diagram</img>


3.3. Use case scenario

<table>
<tr>
<td>Use case</td>
<td>Create a design from scratch and share on social media</td>
</tr>

<tr>
<td>Description</td>
<td>Scanning a room, adding an item, and sharing on social media</td>
</tr>

<tr>
<td>Actors</td>
<td>User</td>
</tr>

<tr>
<td>Initial state</td>
<td>User is logged in at start screen</td>
</tr>

<tr>
<td>End state</td>
<td>User is at start screen and a design has been shared</td>
</tr>

<tr>
<td>Normal flow</td>
<td>1. User selects scan from start screen <br>
2. User starts the scan <br>
3. User holds up and rotates the device based on instructions <br>
4. User saves the scan to local storage and is returned to start screen <br>
<br>
5. User selects decorate from the start screen <br>
6. User opens the previously created scan file <br>
7. User opens the catalog <br>
8. User selects an entry from the catalog <br>
9. User places the entry and exits the catalog <br>
10. User selects the previously placed item <br>
11. User moves the item to its desired location <br>
12. User saves the design in local storage and is returned to start screen <br>
<br>
13. User selects view in start screen <br>
14. User opens the previously created design file <br>
15. User selects share and picks their preferred social media outlet
</td>
</tr>

<tr>
<td>Alternative flows</td>
<td>Adding multiple items <br>
12b. Repeat from 7. to 11. until desired amount of items have been placed <br>
<br>
Using remote storage
4b,6b,12b,14b. User selects to use remote storage instead of local filesystem and otherwise proceeds normally.
</td>
</tr>

<tr>
<td>Exceptions</td>
<td>A: Device not compatible(step 3) <br>
1. A dialog will inform the user that the device does not have the required hardware <br>
<br>
B: No storage space remaining(step 4 or 12) <br>
1. A dialog will inform the user about the issue, prompting them to try again after clearing space.  <br>
2. User removes some files using other tools <br>
3. User tries to save again, this time successfully. <br>
<br>
C: No internet connection(step 7-9 or 15) <br>
1. User is prompted to try again once connection is re-established <br>
2. User reconnects to the internet <br>
3. User retries, this time succesfully <br>
</td>
</tr>

<tr>
<td>Assumptions</td>
<td>A: The device contains the user's social media credentials</td>
</tr>
