# 03 Upload vector files
In this exercise you will learn to vector import files from your PC.

Prerequisites: Some geo-spatial files and a browser.

You can open the Upload dialog from both the Map and Database tab:

### From the Map tab:
<div>![Upload1](https://media.screensteps.com/image_assets/assets/001/401/507/original/59973e2a-c142-4672-b10a-3e735efdb641.png)</div>

### From the database tab:
![Upload2](https://media.screensteps.com/image_assets/assets/001/401/505/original/30dccc80-ae6c-4d57-9e5c-055aadab2016.png)

## Upload dialog
![dialog](https://media.screensteps.com/image_assets/assets/001/401/509/original/ee0b673b-c1d6-4e7b-9d1d-854015feb470.png)

1. Click the "Add files" or drag files into the dialogue. You can drag multiple file sets in at once.   
2. Set EPSG code. For example, 4326 for wgs84.
3. If you upload other that Shape is a good idea to set the geometry type of the data. Otherwise there is a risk that the geometry is recorded as being mixed.
4. If the data contains texts beyond ASCII, encoding must be set correctly so letters is displayed correctly.
5. If the data contains errors, so some features can't be imported, then skip these.
6. If there is already a layer with the file name, it can be overwritten.
7. If append is checked, an existing layer will not be overwriting. But it'll be appended the new data.
8. If Delete / append is checked, an existing layer will not be overwriting. But it'll be emptied and the file is imported into the empty layer. Use this to avoid dropping depending database views.
9. Click "Start upload".

After upload, the new data sets are available in Map tab where it has been given a standard styling and in the Database tab where you can set additional properties of the data set.
