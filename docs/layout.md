## Dashboard (Home page)

The Dashboard shows a list of all records in the index. These can be selected or filtered. The search functionality mimics the GeoBlacklight interface:

* a search bar at the top for text searches
* a list of facets on the left to filter records
* a Date Range filter above the facets to select items by Date Created (when they were first added).

![](images/dashboard.png)


----------
## Form view

This page shows all of the editable fields for an individual record. Users can create new records or edit existing records manually with the Form view.

![](images/formView.png)

!!! tip

	Click on the button "View in Geoportal" to open a new tab with the record live in GeoBlacklight. Note: the record is still viewable live via this button, even if it is a Draft or Unpublished.

------------
## Notifications

The Notificiations tab shows downloadable file links. When a user requests a set of files for export, GeoBlacklight Admin will dynamically generate the download. Once the files are ready, the Notifications tab will display a red visual indicator.

![](images/notifications.png)

------------
## Admin Tools

The Admin Tools is a dropdown menu item that contains links to the various actions.

![](images/adminTools.png)

### Documents

This link shows all the documents in the Dashboard. (It is a duplicate of the default homepage.)

### Imports

This tool enables users to upload CSV files of metadata records.  See the [Import records](import.md) page for more details.

### Bulk Actions

This link shows a list of batch edits a user has generated, such as setting the Publication State for a set of records. Bulk Actions cannot be created or edited from this page - it is currently only a list of previous actions. However, it may be useful to check on the status or history of an action.

### Download Links

This tool enables users to upload CSV files for items with multiple downloads. See the Secondary Tables section of the [Import records](import.md) page.

### Users

Administrators can add or remove users with this page.
