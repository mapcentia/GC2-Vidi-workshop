# Database administration
In the Database tab, the database can be manage. This is where the overall characteristics of the layers can be set and the table structure can be changed.

## Layer grid
![Layer grid](http://mapcentia.screenstepslive.com/s/en/m/35406/l/346782/show_image?image_id=1400523)   

Layer properties can be changed by double-clicking on the grid cell you want to change.

1. Type: Layer geometry type, which can be (MULTI)POINT, (MULTI)LINESTRING (MULTI)POLYGON or GEOMETRY. The latter means that the layer may have a mixture of several different types. The layer type can not be changed.
2. Name: The technical name of the layer. If the layer is imported from a file, the name match the file name.
3. Title: A title for the layer. If a title is applied, this will appear in layer trees, legends, WMS / WFS titles etc.
4. Description: A descriptive text for the layer. Applied to WMS / WFS abstracts.
5. Group: Groups are used to divide layer trees in the Map tab and in the Viewer. This combo box: Either enter the name of a new group or select an already existing one.
6. Sort id: Location of the layer in layer hierarchy. Sets whether a layer is on top of or underneath another layer when they appear together in the Map tab or Viewer.
7. Authentication: What level of authentication is required for the individual layers in WMS and WFS services? Write = authentication only when writing, Read/Write = authentication when reading and writing, None = no authentication on the layer.
8. Editable: If turned off, the layer can not be edited in the Map tab or through WFS-T.
9. Tile cache: Manually bust the layer's tile cache. This is usually not necessary to do since GC2 do it automatically when needed.

## Table structure
![Table structure](http://mapcentia.screenstepslive.com/s/en/m/35406/l/346782/show_image?image_id=1400519)   

When a layer in the layer grid is selected, the structure of the table is shown below. Here you can set properties on columns. Properties can be changed by double-clicking on the cell yo want to change. Columns can also be added and deleted.

1. Sort ID: In which order columns appear in click-info queries in the Viewer. Columns with lower Sort ID appear topmost.
2. Column: Name of the column. The name can be changed, but consider the use of Alias​(4) instead.
3. Type: Show the data type the column has. Can not be changed.
4. Allow null: Allow the special value NULL in the field.
5. Alias: An alias for the column. Displayed when click-info queries is made in the Viewer.
6. Queryable: Should the column appear in  click-info queries in the Viewer? The starting point is that all columns appear. When 8. changes are made to these properties, only those that are checked off are displayed.
7. Show in mouse over: Instruction to Vidi
8. Searchable: Instruction to Vidi
9. Enable filtering: Deprecated
10. Make Link: If the content of the column are links, they can be made active in the Viewer.
11. Image: Instruction to Vidi
12. Link prefix: If links eg. is missing "http: //" it can be added here.
13. Properties: May contain any information to be used in custom applications.
14. Add new column: Add a new column to the layer table.
15. Delete column. Delete the selected column.
