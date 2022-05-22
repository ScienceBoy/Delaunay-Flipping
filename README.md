# Delaunay-Flipping

If you are also interested in preparing and optimizing 3D objects, you might have heard about the Delaunay triangulation to cover a surface or an area by triangles.

One part of this triangulation is called Delaunay-Flipping to maximize the angles of the triangles in the triangulation.

The Delaunay-Flipping algorithm searches for a triangle, which is adjacent to another triangle and is within the circumcircle of the other triangle. In the example shown below in the images 1a and 1b, the green triangle (P1, P, P3) is within the red circumcircle of the pink triangle (P1, P2, P3) and therefore replacing ( = flipping) the edge (P1, P3) by (P, P2) maximizes the angles for both triangles at the corners P1 and P3.<br>

![image](https://user-images.githubusercontent.com/101653815/169706620-c8cb26af-1d2b-477a-914f-283bb6ab8c5a.png)<br>
(Image 1a: Angles of the triangle (P1, P2, P3) and (P1, P, P3) are small, which can result in sub-optimal area and rendering properties)

![image](https://user-images.githubusercontent.com/101653815/169712770-e71863c3-9788-46b3-a3e9-8678f3fafe27.png)<br>
(Image 1b: Angles of the triangle (P1, P2, P3) and (P1, P, P3) can be maximized by flipping the edge (P1, P3) to (P, P2))
<br><br><br>

Analyzing all triangles and flipping edges where possible can optimize a triangulation, as shown in the following Image 2, where the resulting new optimized triangulation is shown in Image 3 below.
<br><br>
![image](https://user-images.githubusercontent.com/101653815/169713946-1091793e-13d9-418f-81f9-a93a6dbf45f5.png)<br>
(Image 2: Triangulation configuration before applying a Delaunay-Flipping)

![image](https://user-images.githubusercontent.com/101653815/169705696-b2a0db5a-44c7-4aac-8ea1-f25fae62703d.png))<br>
(Image 3: Triangulation configuration after applying a Delaunay-Flipping)
<br><br>

The implementation of this algorithm in this repository includes all required functions as well as the example producing similar images as shown above.

License: CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/)

For a good explanation on Delaunay Triangulation, I recommend https://en.wikipedia.org/wiki/Delaunay_triangulation
