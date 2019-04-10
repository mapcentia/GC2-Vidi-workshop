# 07 QGIS integration

To start with, create a WFS connection from QGIS to GC2.

![QGIS integration](http://mapcentia.screenstepslive.com/s/da/m/24713/l/937864/show_image?image_id=1733549)   

1. In the Database tab, click the Services button.
2. Copy the string from the top field (WFS-T)

Then you go over to QGIS.

![qgis](https://media.screensteps.com/image_assets/assets/001/733/531/original/4ddfde39-5171-4010-bdff-80b7b8088695.png)   

Note that your QGIS setup may look different from the pictures.

1. Establish a new WFS connection.

![qgis](https://media.screensteps.com/image_assets/assets/001/733/524/original/a12c33db-751b-4960-96be-28458c5e8253.png)   

1. In the WFS dialog, click New.
2. In URL, insert the string from GC2 and in Name write any name.
3. Click OK.
4. Click Connect.

![qgis](https://media.screensteps.com/image_assets/assets/001/733/535/original/ddbdf5e4-e671-4844-8f7e-cb3ae3708d57.png)

1. Choose which layers you want to download and set up.
2. Click Add.

![qgis](https://media.screensteps.com/image_assets/assets/001/733/528/original/edb7c547-9184-4119-b551-dde0d2fec12e.png)

1. Set up the layer with the desired styling.
2. Save the project.

![qgis](https://media.screensteps.com/image_assets/assets/001/739/000/original/5d564fb6-299c-450c-89d6-ed0e95bf643f.png)

1. Back in GC2 Admin click on New layer.
2. In the upload dialog, select QGIS.
3. Click Add Files and select your QGIS project file (here Untitled.qgs)
4. Click start upload.

![qgis](https://media.screensteps.com/image_assets/assets/001/738/998/original/6121e9a7-a9c9-4fb8-9097-5829bbebe97c.png)

1. Subsequently, which layers have "received" QGIS styling are shown.

![qgis](https://media.screensteps.com/image_assets/assets/001/738/999/original/6f961bcb-4d09-4bba-ad5a-91dbf40651ec.png)   

Now used QGIS Server graphic back-end and styling from QGIS can be seen.

1. Note that it may be necessary to click Update in the Tile cache tab to recreate the tile cache.
