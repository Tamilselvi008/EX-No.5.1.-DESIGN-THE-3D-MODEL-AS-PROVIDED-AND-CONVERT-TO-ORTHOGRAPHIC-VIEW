# EX No.5.1.DESIGN THE 3D MODEL AS PROVIDED AND CONVERT TO ORTHOGRAPHIC VIEW
## DATE:11/11/2026

## AIM: 
To create orthographic view of given 3D model

## REQUIREMENTS: 
1. Autodesk fusion 360
2. Windows 10
3. 16 GB of RAM (integrated graphics recommend 1 GB or more)
4. 2.5 Mbps or faster download; 500 Kbps or faster upload 

## PROCEDURE:

## 1. Create the base slot

1. Open a new Fusion 360 design and set the document units.
2. Select **Create Sketch**, then choose the **XY plane**.
<img width="1920" height="1004" alt="Screenshot (403)" src="https://github.com/user-attachments/assets/0fe8c901-81b3-4347-ad1d-f86b5283f559" />
3. From **Create**, choose **Slot → Two-Point Slot**.
4. Click the first endpoint, click the second endpoint, then move the cursor to set the slot width and click again.
<img width="1920" height="1014" alt="Screenshot (405)" src="https://github.com/user-attachments/assets/a504f91f-3733-4fae-b4a2-a449172dc6be" />

5. Enter the required slot length and width, or dimension them later with **Sketch Dimension**.
6. Finish the sketch.
7. Select the slot profile and choose **Extrude**.
8. Set the distance to **15 mm** and confirm.
<img width="1920" height="1010" alt="Screenshot (374)" src="https://github.com/user-attachments/assets/b84043a4-25c7-4177-9287-d5b456ce87fe" />

## 2. Sketch the circular layout on the top face

1. Select the top face of the base and choose **Create Sketch**.
2. Use **Look At** or the ViewCube to set the view to **Top**.
3. Select **Create → Circle → Center Diameter Circle**.
4. Draw three concentric circles at the center of the part:
   - **Ø55 mm**
   - **Ø46 mm**
   - **Ø40 mm**
5. Use **Sketch Dimension** to set each circle’s diameter accurately.
6. <img width="1920" height="1015" alt="Screenshot (377)" src="https://github.com/user-attachments/assets/1aead608-fb4c-457f-9b66-3da4b43d1556" />

7. Create the mounting circles:
   - Choose **Center Diameter Circle** again.
   - Draw a circle of **radius 6 mm** at each required mounting position.
   - Dimension the center-to-center spacing to **100 mm** as specified.
   - If the mounting circles are equally spaced or symmetric, constrain their centers with symmetry or equal-distance dimensions.
8. Use **Create → Line** to connect the mounting-circle regions to the **Ø55 mm** circle, as shown in your model.
   - Make sure line endpoints coincide with the intended circle edges.
   - Add **Coincident** constraints where needed so the sketch remains connected.
9. Finish the sketch.
10. Select the closed regions that should form the raised shape and choose **Extrude**.
11. Set the extrusion height according to your design and confirm. Use **Join** if it should merge with the base.
<img width="1920" height="1015" alt="Screenshot (378)" src="https://github.com/user-attachments/assets/8f17fb5d-a74d-46ce-b466-f2fff89fbd51" />

## 3. Repeat the raised geometry from the bottom

1. Rotate the model and select the bottom face, or use the ViewCube’s **Bottom** view.
2. Select the bottom face and choose **Create Sketch**.
3. Repeat the same layout process used on the top:
   - Draw the specified concentric circles.
   - Add the mounting circles with **6 mm radius** and the specified **100 mm** spacing.
   - Connect the mounting-circle areas to the **Ø55 mm** circle with lines.
4. Finish the sketch.
 <img width="1920" height="1013" alt="Screenshot (380)" src="https://github.com/user-attachments/assets/20730c2c-531b-49b4-aba8-352651e09099" />
6. Select the required closed profiles and choose **Extrude**.
7. Set the direction outward from the bottom face and enter **25 mm**.
8. Confirm the extrusion. Check the preview arrow before confirming so the feature extends downward from the part.
<img width="1920" height="1013" alt="Screenshot (381)" src="https://github.com/user-attachments/assets/c81fe0c2-abeb-4f5f-ad8c-591ed23ce53f" />

## 4. Add holes to the raised features

1. Select the face of an extruded mounting feature and choose **Create Sketch**.
2. Draw a circle at its center.
3. Dimension its **radius to 5 mm**. This is a **Ø10 mm** hole.
   ![Uploading Screenshot (382).png…]
4. Finish the sketch.
5. Select the hole profiles and choose **Extrude → Cut**.
6. Set the extent to **Through All** if the holes should pass through the part; otherwise enter the required depth.
7. Confirm the cut.
<img width="1920" height="1015" alt="Screenshot (382)" src="https://github.com/user-attachments/assets/5ab9c941-e7f6-4603-87b8-03e49f0d1933" />

## 5. Add the central opening and internal details

1. Select the top face and orient the view to **Top**.
2. Start a sketch on the face.
3. Draw two concentric circles inside the existing **Ø40 mm** circle:
   - **Ø20 mm**
   - **Ø10 mm**
4. Dimension both circles.
5. To create the internal line details, use **Create → Line**:
   - Draw the first line across the intended area.
   - Draw the second line parallel to it.
   - Dimension the gap between the lines to **5 mm**.
6. Select trim options to remove the extra parts of the lines.
   <img width="1920" height="1017" alt="Screenshot (387)" src="https://github.com/user-attachments/assets/1eb66a95-32fa-4791-a894-f16c9fd210d7" />
7. Finish the sketch.
## 6. Circular-pattern the internal lines

1. Select **Create → Pattern → Circular Pattern**.
<img width="1920" height="1010" alt="Screenshot (384)" src="https://github.com/user-attachments/assets/1508c30c-a16a-46d3-83b0-4c6a38ed40b7" />

2. Set **Pattern Type** to **Features** if you have already extruded the lines; use **Faces** or **Sketch Objects** if they remain sketch geometry.
3. Select the two line-based features or sketch objects.
4. Select the central axis of the circular opening as the pattern axis.
5. Preview the pattern and confirm that the repeated details are evenly spaced around the center.
6. Click **OK**.
<img width="1920" height="1015" alt="Screenshot (385)" src="https://github.com/user-attachments/assets/ab99782d-7709-40f9-be8e-1b4c86db199f" />
### 7. Create the 55 mm angular dimension

1. In the active sketch, choose **Sketch Dimension**.
2. Select the two lines that form the angle.
3. Move the cursor to position the angular dimension, then click.
4. Enter **55°** and press **Enter**.
5. Click **Finish Sketch**.
6. <img width="1920" height="1002" alt="Screenshot (390)" src="https://github.com/user-attachments/assets/82ea6c99-783f-473e-afc1-723448ab48a2" />
### 8.Counterbored holes in the base

1. Sketch mounting-hole points on the base and dimension their positions.
2. Choose **Create → Hole**, select the points, and set **Hole Type** to **Counterbore**.
3. Enter the hole diameter, counterbore diameter, and depth. Set the hole extent to **Through All** if needed.
4. Check the preview and confirm.
5. Then choose mirror option to make it on all four corners.
6. <img width="1920" height="1004" alt="Screenshot (400)" src="https://github.com/user-attachments/assets/46c32b8b-e914-4288-ada7-df955189f20c" />
## 9. Create offset planes and side rectangles

1. Choose **Construct → Offset Plane**.
2. Select the first side face or reference plane.
3. Enter the required offset distance and confirm.
4. Repeat on the opposite side to create the second offset plane.
5. Select the first offset plane and choose **Create Sketch**.
6. Draw the required rectangle on that plane using **Create → Rectangle**.
7. Dimension its width, height, and position from your drawing.
8. Finish the sketch.
9. <img width="1920" height="1021" alt="Screenshot (401)" src="https://github.com/user-attachments/assets/d6d97441-7928-4ea7-9b45-4a2b77f9def8" />

10. Repeat on the second offset plane to draw the matching rectangle.
11. Select each rectangle profile and use **Extrude** with the appropriate operation and distance to create the side features.

## 10. Chamfer both sides

1. Choose **Modify → Chamfer**.
2. Select the edges on the first side that need trimming.
3. Enter the specified chamfer distance or distances.
4. Repeat for the corresponding edges on the opposite side.
5. Inspect both sides to confirm the chamfers are symmetric and do not remove more material than intended.
6. Confirm the feature.
<img width="1920" height="993" alt="Screenshot (402)" src="https://github.com/user-attachments/assets/c46210d8-2f17-467e-8dec-3ce0eab8496e" />

## 11. Fillet the internal line edges

1. Choose **Modify → Fillet**.
2. Select the sharp edges around the internal line features.
3. Enter the required fillet radius.
4. Check the preview for overlaps or failed edges.
5. Confirm the fillet.
<img width="1920" height="1021" alt="Screenshot (404)" src="https://github.com/user-attachments/assets/bdab5681-8845-4226-82d4-68963b199d78" />

## 12. Apply the final edge fillets

1. Choose **Modify → Fillet**.
2. Select the remaining exterior edges that should be rounded. You can select multiple edges, but avoid selecting edges that already have fillets or chamfers if that causes errors.
3. Enter the required final radius.
<img width="1920" height="999" alt="Screenshot (397)" src="https://github.com/user-attachments/assets/73089a90-4666-4f45-beee-37daa05bc0b7" />

## 13. Create the drawing

1. In the Design workspace, choose **File → New Drawing → From Design**.
2. Select the sheet size, units, and projection angle required for your drawing.
3. Place the base view, then add projected **top**, **front**, **side**, and **bottom** views.
4. Add an **isometric** view if it helps show the overall shape.
5. Use **Dimension** to add the important sizes:
   - Base slot length and width
   - Base thickness: **15 mm**
   - Lower extrusion height: **25 mm**
   - Circle diameters: **55 mm, 46 mm, 40 mm, 20 mm, and 10 mm**
   - Mounting-circle radius: **6 mm**
   - Hole radius: **5 mm**
   - Mounting spacing: **100 mm**
   - Internal line spacing: **5 mm**
6. Add center marks to circular features and centerlines where useful.
7. Add any missing dimensions for the rectangles, chamfers, fillets, and feature heights from your design.
8. Fill in the title block with the part name, drawing number, date, scale, and units.
9. Review the drawing for overlapping dimensions and missing views.
10. Save the drawing.

## INPUT
![image](https://user-images.githubusercontent.com/113594316/199408705-ed302b2a-90c3-41c0-9cc4-791a93366e2a.png)

## OUTPUT
<img width="1920" height="1008" alt="Screenshot (398)" src="https://github.com/user-attachments/assets/27304dc3-1995-4854-9740-3da2238ac686" />


## RESULT:
Thus, the given 3D model is converted into orthographic view.


