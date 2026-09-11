This is analysis using [[Mesh|Meshes]], and it is easiest for circuits with few or no current sources. It is done by taking all the mesh's and declaring a current around them in a direction (conventionally clockwise to be consistent). From there, we write a [[Kirchhoff's Loop Law]] for each of the meshes, and then solve the resulting system of equations. 
>[!Note]
>For places where two meshes touch, we then take this to be the difference of the two currents, with the current with respect to our current mesh to be positive, and the other one to be negative

>[!Warning]
>If there are any current sources, then we have to make a super mesh around this, and then write a equation relating the current source to the sources of the two meshes