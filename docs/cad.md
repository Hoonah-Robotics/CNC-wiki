## Step 1. CAD by design
> "design or draw from your imagination and wishes"

![CAD graphic](images/cad-concept.png)

### What is this step?

**CAD** stands for **Computer-Aided Design**. This is the starting point for any project. It's where you use computer software to create a 2D or 3D digital model of your idea. Think of it as a high-tech drawing board.

For our CNC machine, we typically start with a 2D "vector" drawing, which is like a digital connect-the-dots outline that the machine can follow.

### Key Vocabulary

* **CAD (Computer-Aided Design):** Using software to create digital drawings or models.
* **Vector (or SVG):** A type of graphic that uses mathematical lines and curves to create an image. This is perfect for CNC because the machine can follow these lines. This is different from a "pixel" image (like a photo or .jpg) which has no clear path for a machine to follow.
* **Export:** Saving your work in a specific file format. We will export our designs to **SVG (Scalable Vector Graphics)**.

### Workflow Steps

1.  ***Imagine:*** Decide what you want to make. A sign? A keychain? A wall hanging? For your first CNC project start with a basic design.

	/// admonition | **Design knowing the limits of CNC**
		type: note

	We will be using a standard 1/8" (3.175mm) straight end mill to cut. You cannot cut a channel narrower than 1/8"! Also, a rotating tool cannot cut a perfectly sharp internal 90° corner. The finest internal corner will have a 1/16" radius. Compare this to 3d Printers that can extrude lines to 0.1mm width!
	///

2.  **Choose Your Software:** We recommend one of these two options:
    * **[Autodesk Tinkercad](https://www.tinkercad.com):** A very easy to use, free, browser-based tool. While it's known for 3D, you can easily create 2D shapes, text, or export the "bottom" of a 3D design as an SVG.
    * **[Adobe Illustrator](https://www.adobe.com/products/illustrator.html):** A professional tool (available at Alaska STEAM hub) that is excellent for creating detailed vector art, text, and logos.
    * There are dozens of other good design software that also can be used. They must be able to export vectors in SVG format. Painting and photo editing software like Photoshop will ***not*** work!
    * **[Canva](https://www.canva.com)** only allows downloading your design as an SVG file with the Pro subscription. The resulting file may require cleanup in the software listed above especially if you used complex shapes or text since it is the Canva AI translating your design into SVG.
3.  **Create Your Design:**
    * Draw your shapes. 
    	* In Tinkercad the `Extrude Sketch` and `Scribble` tools are the most flexible. 
    	* Any extruded basic shape or text with a flat top and bottom will also work. `Box`, `Polygon`, `Star`, `Heart`, `Script` are all good shapes. But a `Pyramid` with a pointed top will export to SVG as a square. 
    	* `Import` > `SVG` images work, and you can convert the image to an outline using `Fill Mode: Outer Line`  from the shape attributes panel. A helpful video shows this: **[Use the Tinkercad SVG Tool to Create Laser & CNC Designs in Minutes!](https://youtu.be/AzG8kJMFDLM?si=agvdSwsEe1r4-umi)** 
    * Ensure all your lines are "closed polygons" (no gaps, no tails).
	* In Adobe Illustrator text needs to be "outlined" (converted from a text-font into a shape) using the `Type > Create Outlines` command. 
4.  **Export to SVG:**
    * For Tinkercad make sure your design is positioned flat on the workplane at `z = 0`
    * Go to `File > Export` and choose **SVG** as the file type. This `.svg` file is what you will use in the next step (CAM).