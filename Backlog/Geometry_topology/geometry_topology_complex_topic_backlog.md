# Topic Backlog: Experimental Geometry, Topology, and Complex Geometry

This backlog is for a geometry and topology module in an experimental mathematics course. The emphasis is on visual and computational exploration: drawing, deforming, triangulating, tessellating, counting, and discovering invariants experimentally.

The guiding idea is:

> Geometry studies quantities that change with shape; topology studies properties that survive deformation. Computation lets us draw, deform, count, tile, map, and experimentally discover invariants.

This module includes polyhedra, Euler characteristic, Gauss-Bonnet, surfaces, Voronoi and Delaunay tessellations, simplicial complexes, homology, hyperbolic geometry, conformal maps, winding number, and a visual proof of the Fundamental Theorem of Algebra.

---

## 1. Polyhedra and Euler characteristic

**Central question:**  
What remains constant when we change or subdivide a polyhedron?

**Experiments:**

- Build or load triangulated polyhedra:
  - tetrahedron,
  - cube,
  - octahedron,
  - dodecahedron,
  - icosahedron.
- Count vertices \(V\), edges \(E\), and faces \(F\).
- Compute

\[
\chi = V-E+F.
\]

- Subdivide faces and check whether \(\chi\) changes.
- Glue polyhedra together.
- Compare sphere-like and torus-like meshes.

**Patterns to discover:**

- For sphere-like polyhedra,

\[
V-E+F=2.
\]

- Subdivision does not change Euler characteristic.
- Euler characteristic is topological, not metric.

---

## 2. Platonic solids and duality

**Central question:**  
Why are there only five regular polyhedra?

**Experiments:**

- Generate the Platonic solids.
- Count vertices, edges, and faces.
- Compute face degrees and vertex degrees.
- Visualize dual polyhedra.
- Compare:
  - cube and octahedron,
  - dodecahedron and icosahedron.
- Explore why regular tessellations fail to close up in 3D.

**Patterns to discover:**

- Regularity imposes strong combinatorial constraints.
- Duality swaps vertices and faces.
- Curvature is concentrated at vertices.

---

## 3. Triangulated surfaces and genus

**Central question:**  
Can we read the topology of a surface from a mesh?

**Experiments:**

- Generate triangulated surfaces:
  - sphere,
  - torus,
  - double torus,
  - triple torus.
- Count \(V,E,F\).
- Compute

\[
\chi=V-E+F.
\]

- Infer genus:

\[
g=1-\frac{\chi}{2}.
\]

- Add handles and observe how \(\chi\) changes.
- Subdivide triangulations and check invariance.

**Patterns to discover:**

- For a closed orientable surface of genus \(g\),

\[
\chi=2-2g.
\]

- Adding a handle lowers \(\chi\) by \(2\).
- Different triangulations can represent the same topology.

---

## 4. Polygon gluings

**Central question:**  
What surface do we get by gluing edges of a polygon?

**Experiments:**

- Glue opposite edges of a square in different ways.
- Produce:
  - cylinder,
  - torus,
  - Möbius strip,
  - Klein bottle,
  - projective plane.
- Use edge-label diagrams.
- Compute Euler characteristic from identifications.
- Test orientability.
- Compare torus and Klein bottle.

**Patterns to discover:**

- Topology can be encoded combinatorially.
- The torus and Klein bottle differ by orientation reversal in the gluing.
- Surfaces can be built from polygons.

---

## 5. Orientability and the Möbius strip

**Central question:**  
What does it mean for a surface to have one side?

**Experiments:**

- Visualize a cylinder and a Möbius strip.
- Transport a normal vector along a loop.
- Observe whether the normal returns reversed.
- Cut the Möbius strip along its centerline.
- Cut it at one-third width.
- Compare with cutting a cylinder.

**Patterns to discover:**

- Orientability can be tested by transporting local orientation.
- A Möbius strip has only one side.
- Cutting surfaces reveals topology.

---

## 6. Discrete curvature on polyhedra

**Central question:**  
Where is curvature located on a polyhedron?

**Experiments:**

- For each vertex, compute angle defect:

\[
K(v)=2\pi-\sum_{\text{faces at }v}\theta_f(v).
\]

- Compute defects for Platonic solids.
- Color vertices by curvature.
- Subdivide polyhedra and check total curvature.
- Create irregular triangulated spheres.
- Compare convex and nonconvex examples.

**Patterns to discover:**

- Curvature of a polyhedron is concentrated at vertices.
- Total curvature is independent of the triangulation.
- Discrete curvature leads naturally to Gauss-Bonnet.

---

## 7. Discrete Gauss-Bonnet

**Central question:**  
How does curvature know topology?

**Experiments:**

- Compute angle defects on triangulated surfaces.
- Sum the total curvature.
- Try:
  - sphere,
  - torus,
  - double torus,
  - higher-genus surfaces.
- Deform the mesh and observe local curvature changes.
- Check that total curvature stays constant.

**Pattern to discover:**

\[
\sum_v K(v)=2\pi\chi.
\]

For a sphere:

\[
\sum_v K(v)=4\pi.
\]

For a torus:

\[
\sum_v K(v)=0.
\]

---

## 8. Smooth Gauss-Bonnet on surfaces

**Central question:**  
How does Gaussian curvature determine topology?

**Experiments:**

- Visualize a sphere, torus, double torus, and higher-genus surfaces.
- Approximate Gaussian curvature numerically on a mesh.
- Color surfaces by curvature.
- Estimate total curvature by summing over mesh elements.
- Deform surfaces and observe local curvature changes.
- Compare total curvature before and after deformation.

**Pattern to discover:**

\[
\int_M K\,dA=2\pi\chi(M).
\]

For a closed orientable surface of genus \(g\),

\[
\chi=2-2g.
\]

---

## 9. Voronoi tessellations on surfaces

**Central question:**  
Can random points create a cell decomposition whose Euler characteristic reveals the surface?

**Experiments:**

- Sample random points on a sphere.
- Construct the spherical Voronoi diagram.
- Count:
  - number of Voronoi cells \(F\),
  - number of Voronoi edges \(E\),
  - number of Voronoi vertices \(V\).
- Check

\[
V-E+F=2.
\]

- Repeat with more random points.
- Compare with Voronoi diagrams on a flat torus.
- Check that for the torus:

\[
V-E+F=0.
\]

- Try higher-genus surfaces if computationally feasible.

**Patterns to discover:**

- Voronoi diagrams produce random cell decompositions of a surface.
- Every sufficiently nice decomposition should recover the same Euler characteristic.
- Euler characteristic is not an artifact of Platonic solids or triangulations.

---

## 10. Delaunay triangulations and duality

**Central question:**  
How are Voronoi diagrams and triangulations related?

**Experiments:**

- Generate random points on the plane, sphere, or torus.
- Compute the Voronoi diagram.
- Compute the dual Delaunay triangulation.
- Count \(V,E,F\) in both structures.
- Compare Euler characteristic in the primal and dual decompositions.
- Visualize the duality:
  - Voronoi cells correspond to Delaunay vertices.
  - Voronoi edges correspond to Delaunay edges.
  - Voronoi vertices correspond to Delaunay faces.

**Patterns to discover:**

- Voronoi and Delaunay decompositions are dual.
- Dual decompositions have the same Euler characteristic.
- Random point clouds produce natural triangulations of surfaces.

---

## 11. Tessellations of the Euclidean plane

**Central question:**  
How can shapes tile the plane?

**Experiments:**

- Generate regular tessellations:
  - triangular,
  - square,
  - hexagonal.
- Try semiregular tilings.
- Compute angles around vertices.
- Explore why some polygons tile and others do not.
- Compare local and global conditions.

**Patterns to discover:**

- Tiling depends on angle sums.
- There are only three regular Euclidean tessellations.
- Local angle conditions control global geometry.

---

## 12. Spherical tessellations

**Central question:**  
How do tilings change on the sphere?

**Experiments:**

- Tile the sphere using Platonic solids.
- Draw geodesic triangles.
- Compute spherical angle excess.
- Compare planar and spherical triangles.
- Relate tessellations to polyhedra.
- Study how positive curvature affects angle sums.

**Patterns to discover:**

- Spherical triangles have angle sum greater than \(\pi\).
- Positive curvature allows fewer tiles around a vertex.
- Polyhedra are spherical tessellations.

---

## 13. Hyperbolic disk, hyperbolic plane, and straight lines

**Central question:**  
What does “straight” mean in hyperbolic geometry?

**Experiments:**

- Draw the Poincaré disk model.
- Draw geodesics as circular arcs orthogonal to the boundary.
- Compare Euclidean straight lines and hyperbolic straight lines.
- Draw hyperbolic triangles.
- Measure angle sums.
- Move points and watch geodesics change.
- Draw the upper half-plane model.
- Map the upper half-plane to the disk.
- Compare geodesics in both models.

**Patterns to discover:**

- Hyperbolic lines in the disk are circular arcs orthogonal to the boundary.
- Hyperbolic triangles have angle sum less than \(\pi\).
- Many lines can pass through a point without meeting a given line.
- The disk boundary is infinitely far away.
- The Poincaré disk preserves angles but distorts distances.

---

## 14. Hyperbolic tessellations

**Central question:**  
Why are there so many regular tessellations in hyperbolic geometry?

**Experiments:**

- Draw regular tessellations \(\{p,q\}\) in the Poincaré disk.
- Compare spherical, Euclidean, and hyperbolic cases.
- Explore the condition:

\[
\frac1p+\frac1q
\begin{cases}
> \frac12 & \text{spherical},\\
= \frac12 & \text{Euclidean},\\
< \frac12 & \text{hyperbolic}.
\end{cases}
\]

- Draw triangle-group tilings.
- Visualize how tiles shrink near the boundary in the disk model.

**Patterns to discover:**

- Negative curvature allows more polygons around a vertex.
- Hyperbolic space has exponentially more room.
- The Poincaré disk makes infinite tilings visible inside a finite circle.

---

## 15. Simplicial complexes

**Central question:**  
How can we build spaces out of vertices, edges, triangles, and tetrahedra?

**Experiments:**

- Build graphs as 1-dimensional complexes.
- Add triangles to fill cycles.
- Add tetrahedra to fill voids.
- Compute \(f\)-vectors:

\[
(f_0,f_1,f_2,\dots).
\]

- Compute Euler characteristic:

\[
\chi=f_0-f_1+f_2-f_3+\cdots.
\]

- Visualize small complexes.
- Compare a cycle graph with a filled disk.

**Patterns to discover:**

- Filling a loop changes topology.
- Euler characteristic generalizes beyond surfaces.
- Simplicial complexes are combinatorial models of spaces.

---

## 16. Homology as counting holes

**Central question:**  
How many holes does a space have?

**Experiments:**

- Compute connected components.
- Detect cycles in graphs.
- Fill cycles with triangles and see \(H_1\) disappear.
- Build a hollow tetrahedron and compare with a filled tetrahedron.
- Compute or infer Betti numbers:

\[
\beta_0,\beta_1,\beta_2.
\]

- Visualize examples:
  - points,
  - circle,
  - disk,
  - sphere,
  - torus,
  - figure eight,
  - simplicial complexes.

**Patterns to discover:**

- \(\beta_0\): number of connected components.
- \(\beta_1\): number of independent loops.
- \(\beta_2\): number of voids.
- Homology turns shape into numbers.

---

## 17. Euler characteristic from Betti numbers

**Central question:**  
How do holes explain Euler characteristic?

**Experiments:**

- Compute \(f\)-vector Euler characteristic.
- Compute Betti numbers.
- Compare:

\[
\chi=\beta_0-\beta_1+\beta_2-\cdots.
\]

- Try graphs, surfaces, and small complexes.
- Watch what changes when adding an edge, triangle, or tetrahedron.

**Patterns to discover:**

- Euler characteristic can be computed combinatorially or homologically.
- Homology explains what Euler characteristic measures.
- Topological invariants are robust under triangulation.

---

## 18. Holomorphic functions as geometric maps

**Central question:**  
What do complex functions do to the plane?

**Experiments:**

- Plot grids in the complex plane.
- Apply maps such as:

\[
z\mapsto z^2,\qquad
z\mapsto z^3,\qquad
z\mapsto e^z,\qquad
z\mapsto \frac{1}{z},\qquad
z\mapsto \frac{z-i}{z+i}.
\]

- Draw images of horizontal and vertical grid lines.
- Color the complex plane by argument and modulus.
- Observe where angles are preserved.
- Compare holomorphic and non-holomorphic maps, for example:

\[
z\mapsto \bar z,\qquad z\mapsto |z|.
\]

**Patterns to discover:**

- Holomorphic maps preserve angles where the derivative is nonzero.
- Multiplication by complex numbers rotates and scales.
- The map \(z\mapsto z^n\) multiplies angles by \(n\).
- Complex functions are geometric transformations.

---

## 19. Conformal maps

**Central question:**  
How can one shape be transformed into another while preserving angles?

**Experiments:**

- Visualize Möbius transformations.
- Map the upper half-plane to the disk:

\[
z\mapsto \frac{z-i}{z+i}.
\]

- Map circles and lines under Möbius transformations.
- Experiment with maps from strips to disks.
- Use grid deformation to see conformality.
- Compare conformal maps with area-preserving or distance-preserving maps.

**Patterns to discover:**

- Möbius transformations send generalized circles to generalized circles.
- The Poincaré disk and upper half-plane are conformally equivalent.
- Conformal maps preserve angles but distort lengths and areas.
- Complex analysis is geometry.

---

## 20. Winding number

**Central question:**  
How many times does a curve wind around a point?

**Experiments:**

- Draw closed curves around points.
- Numerically compute winding number.
- Deform curves without crossing the point.
- Compare winding numbers.
- Visualize angle accumulation.
- Study complex maps \(z\mapsto z^n\).
- Plot images of circles under complex maps.

**Patterns to discover:**

- Winding number is invariant under deformation.
- It detects whether a point is inside a loop.
- It connects topology, complex numbers, and vector fields.

---

## 21. Fundamental Theorem of Algebra via winding number

**Central question:**  
Can topology prove that polynomials have roots?

**Experiments:**

- Draw a large circle in the complex plane.
- Apply a polynomial map \(p(z)\).
- Plot the image curve \(p(Re^{it})\).
- Compute how many times the image winds around \(0\).
- Vary \(R\).
- Observe that for large \(R\), \(p(z)\approx z^n\), so the image winds \(n\) times.
- If \(p\) had no roots, deform the large circle to a point without crossing \(0\).
- Observe the contradiction in winding number.

**Pattern to discover:**

A nonconstant complex polynomial must have a zero.

**Experimental proof idea:**

For large \(R\), the curve

\[
p(Re^{it})
\]

winds around \(0\) exactly \(\deg p\) times. But if \(p\) had no root, this curve could be contracted through nonzero values to the constant curve \(p(0)\), whose winding number is \(0\). Since winding number cannot change without crossing \(0\), this is impossible.

---

## 22. Argument principle

**Central question:**  
Can roots be counted by how a curve winds?

**Experiments:**

- Choose a polynomial \(p(z)\).
- Draw a contour \(C\).
- Plot the image curve \(p(C)\).
- Compute its winding number around \(0\).
- Compare with the number of roots of \(p\) inside \(C\).
- Move the contour and observe how the count changes.
- Try functions with poles, such as rational functions.

**Patterns to discover:**

For a polynomial \(p\),

\[
\operatorname{wind}(p(C),0)
=
\#\{\text{zeros of }p\text{ inside }C\}.
\]

More generally,

\[
\frac{1}{2\pi i}\int_C \frac{f'(z)}{f(z)}\,dz
=
N-P.
\]

This connects complex analysis, topology, and computation.

---

## 23. Curves on surfaces

**Central question:**  
Which loops can be shrunk to a point?

**Experiments:**

- Draw loops on a sphere.
- Draw loops on a torus.
- Draw meridians and longitudes.
- Try to contract loops visually.
- Study loops on punctured planes.
- Simulate homotopies.

**Patterns to discover:**

- On a sphere, every loop contracts.
- On a torus, many loops do not.
- Holes are detected by noncontractible loops.

---

## 24. Fundamental group experiments

**Central question:**  
Can loops detect holes algebraically?

**Experiments:**

- Study loops in:
  - circle,
  - plane minus one point,
  - plane minus two points,
  - torus,
  - wedge of circles.
- Represent loops as words.
- Reduce words in free groups.
- Animate loop concatenation.
- Explore commutativity on the torus versus noncommutativity in the punctured plane.

**Patterns to discover:**

- \(\pi_1(S^1)=\mathbb Z\).
- The plane minus \(n\) points gives free groups.
- The torus has two commuting generators.
- Loops encode topology algebraically.

---

## 25. Circle packing

**Central question:**  
How can geometry be encoded by tangent circles?

**Experiments:**

- Generate circle packings for triangulated planar graphs.
- Visualize Apollonian gaskets.
- Explore Descartes circle theorem.
- Approximate conformal maps via circle packing.
- Compare random and regular packings.

**Patterns to discover:**

- Tangency graphs encode geometry.
- Circle packings connect combinatorics and conformal geometry.
- Fractal patterns arise naturally.

---

## 26. Fractals and dimension

**Central question:**  
Can dimension be non-integer?

**Experiments:**

- Generate:
  - Cantor set,
  - Sierpiński triangle,
  - Koch curve.
- Estimate box-counting dimension.
- Compare length, area, and scaling.
- Add random fractals.
- Explore coastlines and Brownian paths.

**Patterns to discover:**

- Scaling behavior defines dimension.
- Fractals are self-similar.
- Topological dimension and fractal dimension differ.

---

## 27. Knot diagrams

**Central question:**  
How can a closed curve in space be knotted?

**Experiments:**

- Draw knot diagrams.
- Compute crossing number.
- Apply Reidemeister moves.
- Color knots.
- Compute simple invariants:
  - tricolorability,
  - linking number,
  - bracket polynomial for simple examples.
- Compare unknot, trefoil, and figure-eight knot.

**Patterns to discover:**

- Diagrams change, but knots may not.
- Reidemeister moves preserve knot type.
- Invariants help distinguish knots.

---

## 28. Configuration spaces and braids

**Central question:**  
What is the shape of the space of possible positions?

**Experiments:**

- Study two points moving on a line without collision.
- Study points moving on a circle.
- Animate moving points in the plane.
- Track braids.
- Compose braids.
- Compare braids with permutations.
- Visualize braid relations.

**Patterns to discover:**

- A configuration space can have nontrivial topology.
- Paths of configurations form algebraic objects.
- Braids remember more than permutations.

---

## 29. Convex hulls and computational geometry

**Central question:**  
What shape is determined by a finite set of points?

**Experiments:**

- Generate random point clouds.
- Compute convex hulls.
- Visualize Graham scan or gift-wrapping algorithm.
- Count hull vertices.
- Compare random distributions.
- Study higher-dimensional hulls if possible.

**Patterns to discover:**

- Random point sets have typical convex hulls.
- Algorithms reveal geometric structure.
- Convexity is computationally accessible.

---

## 30. Minimal surfaces and soap films

**Central question:**  
What shapes minimize area?

**Experiments:**

- Simulate soap films using mesh relaxation.
- Explore catenoid versus two disks.
- Study minimal surfaces spanning wireframes.
- Compare area under perturbations.
- Visualize mean curvature.

**Patterns to discover:**

- Minimal surfaces have zero mean curvature.
- Topology and boundary conditions constrain minimizers.
- Some minimizers become unstable.

---

## 31. Shape classification with invariants

**Central question:**  
How can we tell whether two shapes are the same?

**Experiments:**

- Compare shapes using:
  - Euler characteristic,
  - Betti numbers,
  - orientability,
  - genus,
  - curvature integrals,
  - fundamental group clues.
- Build a small shape classifier.
- Test it on meshes and complexes.

**Patterns to discover:**

- Different invariants detect different features.
- Some shapes require stronger invariants.
- Classification is experimental before it is theoretical.
