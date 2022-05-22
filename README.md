# Delaunay-Flipping

Implementation of the Delaunay Flipping to maximize the angles of triangles in a plane triangulation.<br>
For a good explanation, I recommend https://en.wikipedia.org/wiki/Delaunay_triangulation

The Delaunay-Flipping algorithm searches for triangles, which are adjacent to another and are within the circumcircle of one of the triangle. In the example below the triangle (P1, P, P3) is within the circumcircle of the triangle (P1, P2, P3) and therefore flipping the edge (P1, P3) to (P, P2) maximizes the angles for both triangles.<br>
![image](https://user-images.githubusercontent.com/101653815/169706620-c8cb26af-1d2b-477a-914f-283bb6ab8c5a.png)<br>
(Image 1: Angles of the triangle (P1, P2, P3) and (P1, P, P3) can be maximized by flipping the edge (P1, P3) to (P, P2)
<br><br><br>

Flipping all possible triangles of Image 2 results in the new optimized triangulation shown in Image 3
<br><br>
![image](https://user-images.githubusercontent.com/101653815/169705704-1d8d904f-08ee-426b-8969-683acebbd0cc.png))<br>
(Image 2: Triangulation configuration before applying a Delaunay-Flipping

![image](https://user-images.githubusercontent.com/101653815/169705696-b2a0db5a-44c7-4aac-8ea1-f25fae62703d.png))<br>
(Image 3: Triangulation configuration after applying a Delaunay-Flipping)
<br><br>

This implementation in this repository includes all required functions and the shown exmaple.
