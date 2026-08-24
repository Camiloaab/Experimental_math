# Suggested 8-Session Plan: Experimental Geometry, Topology, and Complex Geometry

## Module title

**Shapes, Curvature, Tessellations, and Complex Maps**

## Guiding theme

Geometry studies measurements that change with shape; topology studies properties that survive deformation. Computation lets us draw, deform, count, tile, map, and wind curves around points in order to experimentally discover invariants.

---

## Overview of the 8-session arc

1. Count pieces of polyhedra.
2. Build and classify surfaces.
3. Discover that curvature detects topology.
4. Use random tessellations to recover Euler characteristic.
5. Count holes with simplicial complexes and homology.
6. Explore hyperbolic straight lines and negative curvature.
7. Study holomorphic functions as conformal maps.
8. Use winding number to prove the Fundamental Theorem of Algebra.

In one sentence:

> Shapes can be decomposed, counted, curved, tiled, mapped, and wound around points — and all these experiments reveal invariants.

---

# Session 1 — Polyhedra and Euler characteristic

## Central question

What remains unchanged when we decompose a surface into pieces?

## Experiments

- Build or load Platonic solids:
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

- Subdivide faces and check that \(\chi\) stays constant.
- Compare different triangulations of the sphere.
- Compare sphere-like and torus-like meshes.

## Main discoveries

- Sphere-like polyhedra satisfy

\[
V-E+F=2.
\]

- Subdivision does not change Euler characteristic.
- Euler characteristic is topological, not metric.

## Mathematical shadows

- Euler characteristic.
- Cell decompositions.
- Topological invariance.
- Platonic solids and duality.

## Suggested notebook outputs

- Tables of \(V,E,F,\chi\) for different polyhedra.
- 3D plots of polyhedra.
- Subdivision experiments showing invariant \(\chi\).

---

# Session 2 — Surfaces, genus, and polygon gluings

## Central question

How can we build and classify surfaces?

## Experiments

- Generate or load triangulated surfaces:
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

- Use polygon gluing diagrams to build:
  - cylinder,
  - torus,
  - Möbius strip,
  - Klein bottle,
  - projective plane.
- Test orientability visually.

## Main discoveries

- For a closed orientable surface of genus \(g\),

\[
\chi=2-2g.
\]

- Adding a handle lowers Euler characteristic by \(2\).
- Topology can be encoded by polygon edge identifications.
- Orientability is a global property.

## Mathematical shadows

- Genus.
- Orientability.
- Classification of surfaces.
- Polygon gluings.

## Suggested notebook outputs

- Mesh visualizations of genus \(0,1,2,3\) surfaces.
- Tables of Euler characteristic and genus.
- Edge-gluing diagrams.

---

# Session 3 — Discrete curvature and Gauss-Bonnet

## Central question

How does curvature know topology?

## Experiments

- On a triangulated surface, compute angle defect at each vertex:

\[
K(v)=2\pi-\sum_{\text{faces at }v}\theta_f(v).
\]

- Color vertices by curvature.
- Sum total curvature.
- Try:
  - sphere,
  - torus,
  - double torus.
- Deform the mesh and observe local changes.
- Check that total curvature remains constant.
- Compare polyhedral curvature with smooth Gaussian curvature.

## Main discoveries

- Curvature can be concentrated at vertices in a polyhedral surface.
- Local curvature changes under deformation.
- Total curvature remains topological.
- Discrete Gauss-Bonnet gives:

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

## Mathematical shadows

- Angle defect.
- Discrete curvature.
- Gauss-Bonnet theorem.
- Euler characteristic.

## Suggested notebook outputs

- Curvature-colored meshes.
- Tables comparing total curvature and \(2\pi\chi\).
- Deformation experiments.

---

# Session 4 — Voronoi and Delaunay tessellations on surfaces

## Central question

Can random cell decompositions recover topology?

## Experiments

- Generate random points on a sphere.
- Construct the spherical Voronoi diagram.
- Count:
  - Voronoi vertices \(V\),
  - Voronoi edges \(E\),
  - Voronoi cells \(F\).
- Check

\[
V-E+F=2.
\]

- Construct the Delaunay triangulation dual to the Voronoi diagram.
- Compare Euler characteristic in both decompositions.
- Repeat with more points.
- If feasible, repeat on a flat torus and check

\[
V-E+F=0.
\]

## Main discoveries

- Voronoi diagrams give random cell decompositions of a surface.
- Delaunay triangulations are dual to Voronoi decompositions.
- Euler characteristic is independent of the chosen decomposition.
- Random geometry still recovers topology.

## Mathematical shadows

- Voronoi diagrams.
- Delaunay triangulations.
- Dual cell decompositions.
- Euler characteristic on surfaces.

## Suggested notebook outputs

- Spherical Voronoi diagrams.
- Delaunay triangulations.
- Tables of \(V,E,F,\chi\) for random decompositions.
- Visual primal-dual overlays.

---

# Session 5 — Simplicial complexes and homology

## Central question

How can we count holes?

## Experiments

- Build spaces from vertices, edges, triangles, and tetrahedra.
- Compare:
  - isolated points,
  - graph cycles,
  - filled triangles,
  - hollow tetrahedra,
  - filled tetrahedra,
  - triangulated sphere,
  - triangulated torus.
- Compute \(f\)-vectors:

\[
(f_0,f_1,f_2,f_3,\dots).
\]

- Compute Euler characteristic:

\[
\chi=f_0-f_1+f_2-f_3+\cdots.
\]

- Compute or experimentally infer Betti numbers:

\[
\beta_0,\beta_1,\beta_2.
\]

- Compare

\[
\chi=\beta_0-\beta_1+\beta_2-\cdots.
\]

## Main discoveries

- Filling a loop changes topology.
- \(\beta_0\) counts components.
- \(\beta_1\) counts independent loops.
- \(\beta_2\) counts voids.
- Euler characteristic is the alternating count of holes.

## Mathematical shadows

- Simplicial complexes.
- Homology.
- Betti numbers.
- Euler-Poincaré formula.

## Suggested notebook outputs

- Visual examples of small complexes.
- Boundary matrices for small examples.
- Tables comparing \(f\)-vectors, Betti numbers, and Euler characteristic.

---

# Session 6 — Hyperbolic geometry: disk, plane, and straight lines

## Central question

What does straightness look like in negative curvature?

## Experiments

- Draw the Poincaré disk model.
- Draw geodesics in the disk as arcs orthogonal to the boundary.
- Draw the upper half-plane model.
- Draw geodesics in the upper half-plane.
- Map the upper half-plane to the disk using

\[
z\mapsto \frac{z-i}{z+i}.
\]

- Compare geodesics in both models.
- Draw hyperbolic triangles.
- Measure angle sums.
- Compare Euclidean, spherical, and hyperbolic tessellations.
- Draw simple hyperbolic tessellations \(\{p,q\}\).

## Main discoveries

- Hyperbolic lines depend on the model.
- In the Poincaré disk, geodesics are circular arcs orthogonal to the boundary.
- Hyperbolic triangles have angle sum less than \(\pi\).
- The Poincaré disk is conformal: it preserves angles but distorts distances.
- Negative curvature allows many regular tessellations.

## Mathematical shadows

- Hyperbolic geometry.
- Poincaré disk.
- Upper half-plane.
- Geodesics.
- Hyperbolic tessellations.
- Conformal models.

## Suggested notebook outputs

- Interactive Poincaré disk with geodesics.
- Hyperbolic triangle angle experiments.
- Disk/half-plane map visualizations.
- Hyperbolic tessellation plots.

---

# Session 7 — Holomorphic functions and conformal maps

## Central question

How do complex functions transform geometry?

## Experiments

- Draw grids in the complex plane.
- Apply maps:

\[
z\mapsto z^2,\qquad
z\mapsto z^3,\qquad
z\mapsto e^z,\qquad
z\mapsto \frac{1}{z},\qquad
z\mapsto \frac{z-i}{z+i}.
\]

- Visualize image grids.
- Check angle preservation.
- Compare holomorphic maps with non-holomorphic maps such as:

\[
z\mapsto \bar z,\qquad z\mapsto |z|.
\]

- Study Möbius transformations.
- Observe how generalized circles are mapped.

## Main discoveries

- Holomorphic maps are locally scaling plus rotation where \(f'(z)\neq0\).
- They preserve angles at noncritical points.
- The map \(z\mapsto z^n\) multiplies angles by \(n\).
- Möbius transformations send generalized circles to generalized circles.
- The disk and half-plane models of hyperbolic geometry are conformally equivalent.

## Mathematical shadows

- Holomorphic functions.
- Conformal maps.
- Möbius transformations.
- Complex geometry.
- Critical points.

## Suggested notebook outputs

- Grid-deformation plots.
- Domain coloring plots.
- Möbius transformation animations.
- Comparisons of holomorphic and non-holomorphic maps.

---

# Session 8 — Winding number and the Fundamental Theorem of Algebra

## Central question

Can topology prove that polynomials have roots?

## Experiments

- Draw closed curves in the complex plane.
- Compute winding number around a point.
- Deform curves without crossing the chosen point.
- Apply polynomial maps to circles.
- Plot

\[
p(Re^{it})
\]

for large \(R\).
- Count how many times the image winds around \(0\).
- Vary \(R\).
- Watch roots appear as obstructions to contraction.
- Compare with the argument principle.

## Main discoveries

- Winding number is invariant under deformation.
- A polynomial of degree \(n\) sends a large circle to a curve winding \(n\) times around \(0\).
- If a polynomial had no roots, this winding could be deformed to \(0\), which is impossible.
- Therefore every nonconstant complex polynomial has a root.

## Experimental proof idea

For large \(R\), the curve

\[
p(Re^{it})
\]

winds around \(0\) exactly \(\deg p\) times. But if \(p\) had no root, this curve could be contracted through nonzero values to the constant curve \(p(0)\), whose winding number is \(0\). Since winding number cannot change without crossing \(0\), this is impossible.

## Mathematical shadows

- Winding number.
- Homotopy.
- Argument principle.
- Fundamental Theorem of Algebra.
- Topology of the complex plane.

## Suggested notebook outputs

- Interactive winding number computation.
- Images of circles under polynomial maps.
- Winding number versus number of roots inside a contour.
- Visual proof of the Fundamental Theorem of Algebra.

---

# Optional alternatives and projects

These topics are excellent but probably too much for the core eight sessions.

## Persistent homology

- Sample point clouds from circles, tori, and noisy shapes.
- Build Vietoris-Rips complexes.
- Track components and loops across scale.
- Produce barcode-style plots.

## Knot theory

- Draw knot diagrams.
- Apply Reidemeister moves.
- Compute tricolorability and linking number.
- Compare trefoil, figure-eight knot, and unknot.

## Fundamental group experiments

- Study loops in punctured planes, circles, tori, and wedges of circles.
- Represent loops as words.
- Animate loop concatenation.

## Circle packing

- Generate circle packings.
- Explore Apollonian gaskets.
- Connect tangency graphs with geometry.

## Fractals and dimension

- Generate Cantor set, Sierpiński triangle, and Koch curve.
- Estimate box-counting dimension.

## Minimal surfaces

- Simulate soap films.
- Explore catenoids and minimal surfaces spanning wireframes.

## Configuration spaces and braids

- Animate moving points.
- Track braids.
- Compare braids with permutations.

---

# Summary

The core eight-session plan is:

1. **Polyhedra and Euler characteristic**
2. **Surfaces, genus, and polygon gluings**
3. **Discrete curvature and Gauss-Bonnet**
4. **Voronoi and Delaunay tessellations on surfaces**
5. **Simplicial complexes and homology**
6. **Hyperbolic geometry: disk, plane, and straight lines**
7. **Holomorphic functions and conformal maps**
8. **Winding number and the Fundamental Theorem of Algebra**

This gives a coherent progression from combinatorial topology to curvature, random tessellations, homology, hyperbolic geometry, complex maps, and a topological proof of the Fundamental Theorem of Algebra.
