# Import records

Users can use this page to batch create or edit records with a CSV file.

## Primary Table

The Primary table holds the metadata for each item.

1. Create a CSV using the Label for each OGM Aardvark metadata field

!!! tip

	Copy the [B1G Template](https://z.umn.edu/b1g-template) for an example of an importable CSV.

2. Upload the spreadsheet to GeoBlacklight Admin

	- Go to Admin Tools and select Imports. Click **New Import**.
	- Give a name to the upload and enter details about the source and description. These details are helpful later in tracking imports.
	- Select the CSV file for upload
	- For Type, choose **BTAA CSV**. 
	- Click the **Create Import** button
	- Review the _Field Mappings_ page. If the CSV was formatted with column headers spelled the same way as the template, the fields should automatically map to the correct elements. Otherwise, manually choose the crosswalk mapping.
	- Scroll to the bottom and click the button **Create Mapping**
	- On the _Import_ page, check that the number in the CSV Row Count matches your CSV.
	- Click the button **Run Import**
	- The import may take a few minutes. During the process, you can view the Import Results tab. Items in the queue will show up in the first sub-tab ("Failed"), but will transfer to the second tab upon import ("Success").
	- When complete, review and troubleshoot any items that did not import in the Failed tab.

3. Spot check records for errors and consistency

	- The newly uploaded records will be listed as **Draft** under the Publication State on the main Documents view.
	- Select 'Draft' under Publication State and select an item. This will open it in editing view.
	- Click the button **View in Geoportal**
	- Inspect the record and test the links.	- Repeat this process for about 3 records.


4. Convert records from 'Draft' to 'Published'

	- If the records are satisfactory, return to the Documents view and select all Draft items in the upload. 
	- Select All and then select the text "Select all results that match this search"
	- Click the State button. From the dropdown, select Published.
	- On the _Bulk Action_ page, click the button **Run Bulk Action**
	- Review 3-5 of the published records and test all the links.

## Secondary tables

Secondary tables are for selected external links and assets/file attachments.

### External Links

`Multiple Download Links` and `Institutional Access Links` use secondary tables.

* When using the Form view, these values can be entered directly.
* For CSV uploads, these values use a different template than for the Primary table.

* **Multiple Download Links**: 
	- on the Form view, scroll down to the Multiple Download Links inside the editor
	- to enter manually, click the New Download URL button
	- to upload multiple links, click the Import CSV button

* **Institutional Access Links**:
	- on the Form view, click the text "Institutional Access Links" on the bottom of the right hand navigation OR go to Admin Tools - Access Links
	- to enter manually, click the New Access URL button
	- to upload multiple links, click the Import CSV button

!!! Info "CSV field headers for secondary tables"

    === "Multiple Downloads"

        ``` markdown
        
			| friendlier_id       | label            | value      |
			|---------------------|------------------|------------|
			| ID of target record |  any string      | the link   |
        ```

    === "Institutional Access Links"

        ``` markdown
			| friendlier_id       | institution_code | access_URL |
			|---------------------|------------------|------------|
			| ID of target record |  2 digit code    | the link   |
        ```


### Assets/File Attachments

!!! warning "in development"

	This feature is currently in development