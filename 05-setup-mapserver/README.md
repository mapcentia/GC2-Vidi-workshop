# 05 Setup of MapServer
Now it's time for styling the map.

## Start of class wizard
![Start of class wizard](http://mapcentia.screenstepslive.com/s/en/m/35406/l/346781/show_image?image_id=1401453)   
1. In the layer tree to the left, select a layer by clicking on the title so the background turns grey.
2. Then click on "Class Wizard".

## Class Wizard
![Class Wizard](https://media.screensteps.com/image_assets/assets/001/401/447/original/4c5203ba-591a-4a92-9fc3-c24d3c479d01.png)   
Class wizard always shows the latest used wizard and its options.

1. "Single" is the most simple styling (being set as the default for all new uploads). Will create a class with a chosen color.
2. "Unique values" create classes for distinct values from the selected field.
3. "Intervals" creates classes for intervals from the selected field. Only numeric fields can be used. Number of classes (# of colors) and start and end color must be set. You can choose between two types of intervals: Equal and Quantiles.
3. "Clustering" creates clusters of points. A distance in pixels is set to cluster threshold.

All wizards have a "Required" section in which properties that are specific to the selected wizard must be set.
In the "Symbol" and "Label" sections, the created classes are assigned additional properties. These two sections are the same for all wizards.

## "Symbol" properties
!["Symbol" properties](https://media.screensteps.com/image_assets/assets/001/401/457/original/ac71270b-ab2a-4c31-9792-8130f3904947.png)   
1. Symbol: Which symbol should be used? Leave blank if a solid surface or line is desired on polygon and line layers.
2. Angle: Rotate the symbols against the clock a number of degrees. This is combo box**.
3. Size. The symbol's height in pixels. This is combo box*.
4. Outline color: color to be used for the edge of surfaces and certain marker symbols. Has no effect on lines.
5. Line width: Thickness of lines in pixels.
6. Opacity: Object transparency on the scale of 1-100, where 100 is solid.

** Either write a value or select a attribute field with the value to be used.

## "Label" properties
!["Label" properties](https://media.screensteps.com/image_assets/assets/001/401/449/original/9e37afea-cc39-4598-9fc3-d6484e621080.png)   

1. Text: Add labels. Which text to be displayed? This is a combo box*. You can also combine multiple columns and static 2.text: eg "No. [id] \n [text]" where \n indicates a line break.
3. Color: The color of the labels.
Size: Size of labels in pixels. This is combo box**.
4. Position: The position of the label relative to the anchor point.
5. Angle: Rotate the labels against the clock a number of degrees. This is combo box*.
6. Background: Select a background color for labels. This will place a square behind the labels, so they are easier to read.
7. Font. Select the font to be used for labels.
7. Font weight. Choose what type of font: normal, bold, italic and so on.

** Either write a value or select a attribute field with the value to be used.

## Manual setup / modification of classes
![Manual setup / modification of classes](http://mapcentia.screenstepslive.com/s/en/m/35406/l/346781/show_image?image_id=1401455)   

After using "Class wizard" or if you want to build classes from scratch, it can be done from the right side panel.

1. Open the panel for the by clicking on the selected layer.

## The Classes tab
![The Classes tab](https://media.screensteps.com/image_assets/assets/001/401/451/original/1a2371e1-915d-428b-bf73-771f48655506.png)   

1. The top grid lists all the classes of the layer. There must be a minimum of one class or layer will not be visible on the map. If a class is selected its properties get shown in the dialogue below.
2. A class properties are divided into five tabs: Base, Symbol1, Symbol2, Label1 and Label2.

## The Base tab
![The Base tab](https://media.screensteps.com/image_assets/assets/001/401/459/original/ff57b09a-f49c-4e0c-83ab-de433c505ed7.png)   

In the Base tab, the basic properties of the class are set. The two most important are:

1. Name: If the class is given a name, it appears in the legend under the name.
2. Expression: Each object in the layer is evaluated against Expression. If the result is true, its assigned the object class. If the layer only has one class, Expression is not necessary. Without Expression the class will be assigned to all the objects in the layer. Read more about expressions.
3. Min scale: Minimum scale at which this class is drawn. Scale is given as the denominator of the actual scale fraction, for example for a map at a scale of 1:24,000 use 24000.
4. Max scale: Maximum scale at which this CLASS is drawn. Scale is given as the denominator of the actual scale fraction, for example for a map at a scale of 1:24,000 use 24000.
5. Sort id: Specifies the order in which classes appear on the legend. Lower value appears at the top. Note that Sort ID does not affect the order of which the objects are drawn in the map.

## The Symbol1 and Symbol2 tab
![The Symbol1 and Symbol2 tab](https://media.screensteps.com/image_assets/assets/001/401/461/original/164be200-2f6c-495f-a811-84a45edc1256.png)   

You can add two independent symbols to a class. Symbol1 is placed at the bottom and Symbol2 on top. This can create a more complex symbology. This can create a more complex symbology. Typically, however, Symbol1 will suffice.

1. Symbol Size and Symbol Angle's combo boxes. This means that both can be written a value (integer) or select a column from which the value should be. This can be used to rotate the arrow symbols for an attribute on individual objects.

## The Label1 and Label2 tab
![The Label1 and Label2 tab](https://media.screensteps.com/image_assets/assets/001/401/445/original/c94d95b3-6b05-4d5f-99f0-b8291839679d.png)   
Two independent labels can be assigned to a class. Typically, however, Label1 will suffice.

1. On: Set to true to display label on the class.
2. Text: Text to label features with? This is a combo box where you either can write a text or select a reference to feature attributes (the most typical). You can also combine multiple columns and static text: eg "No. [id] \ n [text]" where \ n indicates a line break.
3. Force: Forces labels for a particular class on, regardless of collisions.
4. Min scale: Minimum scale at which the labels are drawn. Scale is given as the denominator of the actual scale fraction, for example for a map at a scale of 1:24,000 use 24000.
5. Max scale: Maximum scale at which the labels are drawn. Scale is given as the denominator of the actual scale fraction, for example for a map at a scale of 1:24,000 use 24000.
6. Position: Position of the label relative to the labeling point. âAutoâ will calculate a label position that will not interfere with other labels. If all positions cause a conflict, then the label is not drawn (Unless the labelâs Force a parameter is set to âtrueâ)
7. Size: Size of labels in pixels. This is combo box. This means that both can be written a value (integer) or select a column from which the value to be taken.
