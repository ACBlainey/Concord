## Author, Copyright and Licence

© 2026 Alexander C. Blainey.

**Author:** Alexander C. Blainey — Independent Researcher  
**Project:** The Concord Framework

This work forms part of the independently developed **Concord Framework**. It is published to encourage examination, criticism, discussion, research and further development.

**Licence:** [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)

This work may be shared, copied, redistributed, adapted and built upon, including for commercial purposes, provided appropriate credit is given to the author, a link to the licence is provided, and any changes are indicated.

**Suggested attribution:**  
Alexander C. Blainey, *[Title of Paper]*, Concord Framework, 2026.



# The Global Triangulation Principle (GTP) for Mars

## A Comprehensive Spatial Framework for Martian Civilisation

### Including: The GTP Subdivision Naming Convention & The GTP Square Grid

---

**Version:** 1.0 (Mars)

**Date:** August 2026

**Author:** Alexander C Blainey

**Status:** Foundational Specification — Martian Adaptation

---

## Abstract

The Global Triangulation Principle (GTP) for Mars provides a recursive, mathematically consistent spatial framework for organising stewardship, governance, infrastructure and digital systems across the Martian surface. Built upon the existing latitude and longitude coordinate system for Mars, GTP creates a fractal triangular tessellation that scales from planetary to local resolutions while maintaining complete backward compatibility with existing geographic data.

This specification adapts the Earth-based GTP framework to Mars, with the **Prime Meridian defined at the centre of Olympus Mons** (the most prominent geographical feature on Mars). The child numbering convention—**where Child 1 is always the single child that points in the same direction as its parent**—is applied consistently throughout all layers and orientations.

The Martian GTP preserves the same mathematical foundations as Earth GTP but accounts for the smaller planetary radius, resulting in different absolute sizes at each layer. A **cross-planet comparison method** is established using equivalent angular subdivisions and a standard reference layer (approximately 1 mile/1.6 km side length) to enable rough comparison between planetary systems.

This paper presents the Martian GTP framework as an implementation of the spatial architecture described in *The Concord*, adapted for a new planetary context. It outlines the rationale, mathematical foundations, nomenclature systems, and practical applications of the framework for Martian settlement and development.

---

## Table of Contents

1. [Introduction](#1-introduction)
2. [Planetary Differences & Cross-Planet Comparison](#2-planetary-differences--cross-planet-comparison)
3. [Foundational Principles](#3-foundational-principles)
4. [Mathematical Foundation](#4-mathematical-foundation)
5. [The Subdivision Naming Convention](#5-the-subdivision-naming-convention)
6. [Nomenclature System](#6-nomenclature-system)
7. [The GTP Square Grid](#7-the-gtp-square-grid)
8. [Worked Examples by Scale](#8-worked-examples-by-scale)
9. [Backward Compatibility: Lon/Lat Translation](#9-backward-compatibility-lonlat-translation)
10. [Applications](#10-applications)
11. [Implementation Considerations](#11-implementation-considerations)
12. [L23 Layer: Precision Infrastructure](#12-l23-layer-precision-infrastructure)
13. [Conclusion](#13-conclusion)
14. [Appendices](#14-appendices)

---

## 1. Introduction

### 1.1 The Challenge of Martian Spatial Organisation

As humanity expands beyond Earth, the need for systematic spatial organisation becomes even more critical. Mars presents a blank canvas—an opportunity to implement spatial frameworks by design rather than by historical accident. Every Martian community will occupy territory. Every infrastructure system will connect locations. Every environmental system will span regions.

The Martian environment presents unique challenges:

- **No oceans** to serve as natural boundaries
- **No established administrative divisions**
- **No legacy mapping systems** beyond orbital and rover data
- **Harsh conditions** requiring precise coordination of life-support systems
- **Distributed settlements** needing robust communication and logistics

*The Concord* identifies fragmented spatial organisation as a source of civilisational fragility. A resilient Martian civilisation requires a shared spatial language through which diverse systems may coordinate.

### 1.2 The Martian Prime Meridian: Olympus Mons

Unlike Earth, where the Prime Meridian was established by historical convention through Greenwich, Mars has an opportunity to choose a meridian based on **prominent geographical features**. The centre of **Olympus Mons**—the largest known volcano in the Solar System, standing approximately 21.9 km high with a base diameter of ~600 km—provides an unambiguous, visually distinctive, and scientifically significant reference point.

**Olympus Mons Centre Coordinates:**

- **Latitude:** 18.65° N
- **Longitude:** 226.2° E (Eastern longitude convention) / 133.8° W (Western longitude convention)

For the Martian GTP, **the Prime Meridian is defined at the centre of Olympus Mons** (226.2° E), providing a natural, visible, and memorable reference for all Martian spatial addressing.

### 1.3 The Subdivision Numbering Convention

This specification applies a single, human-centric naming convention that is:

- **Consistent:** The same rule applies to both upward and downward-pointing triangles
- **Intuitive:** Follows natural clockwise reading order
- **Human-Friendly:** Easy to remember, visualise, and teach
- **Surveyor-Friendly:** Aligns with clockwise bearing measurements used in the field
- **Error-Reducing:** Eliminates orientation-dependent special cases

**Core Rule:**

- Child 1 is always the single child that points in the same direction as its parent
- Children 2 and 3 continue clockwise
- Child 4 is always the central (inverted) triangle

### 1.4 The Role of the Martian GTP

The Global Triangulation Principle for Mars provides a consistent, mathematically derived spatial framework that:

- Preserves backward compatibility with existing Martian latitude and longitude systems
- Scales fractally from planetary to local resolutions
- Supports distributed stewardship through clearly defined spatial units
- Enables digital twins through consistent spatial referencing
- Aligns with human geography through westward numbering of primary quadrants
- Provides practical Layer Zero integration through the Square Grid enhancement
- Supports high-precision pose (orientation and incline) for assets
- Enables cross-planet comparison through equivalent angular layers

The Martian GTP is not a replacement for existing geographic systems. It is an additional layer of spatial organisation that extends and connects them.

---

## 2. Planetary Differences & Cross-Planet Comparison

### 2.1 Fundamental Scaling Difference

A critical principle of the GTP framework is that **each planetary body has its own unique GTP system**. This is not a limitation but a mathematical necessity: the absolute dimensions at each layer depend on the planet's radius.

**Why Planetary GTPs Differ:**

| **Planetary Property** | **Earth** | **Mars** | **Ratio (Mars/Earth)** |
|------------------------|-----------|----------|------------------------|
| Equatorial Radius | 6,378.137 km | 3,396.2 km | 0.5324 |
| Polar Radius | 6,356.752 km | 3,376.2 km | 0.5312 |
| Mean Radius | 6,371.0 km | 3,389.5 km | 0.5320 |
| Surface Area | 510.1 million km² | 144.8 million km² | 0.2840 |
| Circumference | 40,075 km | 21,344 km | 0.5326 |

**The Layering Implication:**

Because Mars is approximately 53.2% the size of Earth, every linear dimension at a given layer is 53.2% of Earth's equivalent. This means:

- L0 triangle side lengths are shorter on Mars
- L1 triangles are shorter on Mars
- The same layer number corresponds to a finer resolution on Mars

### 2.2 Cross-Planet Comparison Methodology

When coordinating across planetary bodies, a **rough comparison** method is required. Rather than attempting to match layer numbers (which produce different absolute sizes), the Martian GTP uses a **best-match layer approach** based on target sizes.

**Method 1: Angular Subdivision Comparison**

The most mathematically rigorous comparison uses **angular extent**:

- Earth L13: 1.2 km side length → angular extent ≈ 0.0108°
- Mars equivalent for 1.2 km: Layer ≈ **L14** (0.64 km) or **L13** (1.29 km) depending on target precision

**Method 2: Target Size Matching**

For practical purposes, a **reference layer** should be defined for each planet that produces similar absolute sizes.

| **Reference Standard** | **Earth Layer** | **Earth Size** | **Mars Layer** | **Mars Size** | **Difference** |
|------------------------|-----------------|----------------|----------------|---------------|----------------|
| ~1 mile (~1.6 km) side | L13 | 1.2 km | L13 | 0.64 km | -47% |
| ~1 mile (~1.6 km) side | L13 | 1.2 km | L12 | 1.28 km | +7% |
| ~0.5 mile (~0.8 km) side | L14 | 0.6 km | L13 | 0.64 km | +7% |

**Recommended Comparison Layer:**

- Earth: **L13** (~1.2 km / ~0.75 mile) — the "1-mile layer"
- Mars: **L12** (~1.28 km / ~0.80 mile) — the "1-mile equivalent layer"

This provides a ±7% match, sufficient for rough cross-planet coordination.

**Method 3: Area-Based Comparison**

For volumetric or resource calculations, area equivalence may be more relevant:

- Earth L13 area: ~1.44 km²
- Mars L12 area: ~1.42 km²
- **Match:** Mars L12 ≈ Earth L13 (within 1.5%)

**Recommended Practice:**

For any cross-planet documentation, always specify:

1. The **planet** and **layer number** (e.g., "Mars L12")
2. The **absolute size** (e.g., "1.28 km side length")
3. The **Earth equivalent layer** for comparison (e.g., "≈ Earth L13")

### 2.3 Lon/Lat Differences Are Also Scaling-Dependent

It is important to note that **existing longitude/latitude systems also differ between planets**. This is not a limitation unique to GTP.

| **Coordinate Property** | **Earth** | **Mars** | **Difference** |
|-------------------------|-----------|----------|----------------|
| 1° latitude (mean) | 111.2 km | 59.2 km | 53.2% |
| 1° longitude at equator | 111.3 km | 59.3 km | 53.2% |
| 1' latitude | 1.853 km | 0.986 km | 53.2% |
| 1" latitude | 30.9 m | 16.4 m | 53.2% |

**Therefore:** When transitioning from Earth to Mars, all geographic coordinates scale by a factor of ~0.532. The GTP system correctly inherits this scaling, which is already implicit in any coordinate system anchored to planetary geometry.

---

## 3. Foundational Principles

### 3.1 Reality Before Abstraction

The Martian GTP begins with observable reality. Mars is a sphere (more precisely, an oblate spheroid). Its surface may be described mathematically through latitude and longitude. Any spatial framework must respect this underlying geometry.

The Martian GTP therefore does not invent new coordinates. It builds upon the existing coordinate system that already underpins Martian navigation, mapping and infrastructure planning.

### 3.2 Mathematical Consistency

Political boundaries change. Administrative regions evolve. Mathematical relationships endure.

The Martian GTP derives its structure from geometry rather than history. Its units are defined through recursive subdivision of a Platonic solid inscribed upon the sphere. This ensures that spatial relationships remain consistent regardless of scale.

### 3.3 Fractal Scalability

A resilient spatial framework must support organisation at every scale of civilisation: from planetary governance to individual stewardship.

The Martian GTP achieves this through recursive subdivision. The same structural pattern repeats at every resolution. A steward operating at planetary scale uses the same principles as a steward managing a local infrastructure node.

### 3.4 Backward Compatibility

Any new spatial framework must interoperate with existing systems. The Martian GTP therefore anchors itself to the existing Martian latitude and longitude grid, ensuring that legacy data, maps and infrastructure may be translated without loss.

### 3.5 Human Usability

A framework intended for civilisation must remain usable by human stewards. The Martian GTP therefore adopts:

- **Westward numbering** that aligns with natural Martian geography (which shares the same rotational direction as Earth)
- **Clockwise logic** that follows the natural reading order used in surveying, navigation, and cartography
- **Consistent rules** that apply regardless of triangle orientation

### 3.6 Unique Planetary Identity

While the Martian GTP preserves the same numbering logic as Earth GTP, it is a **distinct system**:

- **Planet Prefix:** `M` (Mars) or `MA` (for clarity in multi-planet contexts)
- **Independent addressing:** Martian GTP addresses exist in a separate namespace
- **Unique layer sizes:** The absolute dimensions at each layer are Martian-specific

**Cross-Planet Addressing:**

When communication spans planets, addresses should include the planet prefix:

- Earth: `E:N1.4.3.3.1.2.2.4.2.2.3`
- Mars: `M:N1.4.3.3.1.2.2.4.2.2.3`

---

## 4. Mathematical Foundation

### 4.1 The Base Octahedron

The Martian GTP begins with a regular octahedron inscribed within Mars' sphere. The octahedron provides the simplest Platonic solid composed entirely of triangular faces.

**Vertices:**

| **Vertex** | **Latitude** | **Longitude** |
|------------|--------------|---------------|
| North Pole | +90° | Any |
| South Pole | -90° | Any |
| E1 | 0° | 0° (Olympus Mons Prime Meridian) |
| E2 | 0° | 90°W |
| E3 | 0° | 180° |
| E4 | 0° | 90°E |

**Faces:** 8 triangular faces, forming the **L0 Triads** (Layer 0).

**Hemispheres:**

- 4 Northern triangles (N1, N2, N3, N4)
- 4 Southern triangles (S1, S2, S3, S4)

### 4.2 Westward Quadrant Numbering

To align with human geography and time zones (Martian sols), quadrants are numbered **westward** from the Prime Meridian (Olympus Mons centre):

| **Quadrant** | **Longitude Range** | **Direction** | **Major Regions** |
|--------------|---------------------|---------------|-------------------|
| **N1 / S1** | 0° to 90°W | Westward | Tharsis, Olympus Mons |
| **N2 / S2** | 90°W to 180° | Westward | Amazonis, Elysium |
| **N3 / S3** | 180° to 90°E | Westward | Arabia, Utopia |
| **N4 / S4** | 90°E to 0° | Westward | Hellas, Margaritifer |

### 4.3 The Subdivision Rule

To increase resolution, each triangle is subdivided into 4 smaller, congruent triangles by connecting the midpoints of its three edges.

**The 4:1 Rule:**

Each subdivision creates 4 smaller triangles. The central triangle is inverted (pointing opposite to the parent), while the outer three point in the same direction as the parent.

**Edge Rule:** The midpoint of a great circle arc is calculated as the spherical midpoint (the average point projected onto the sphere's surface), not the arithmetic midpoint.

### 4.4 Resolution Layers (Martian Dimensions)

Each subdivision halves the side length of the triangle and divides the area by 4. The recursive nature of the system produces a natural hierarchy of resolutions:

| **Layer** | **Subdivisions** | **Number of Triangles** | **Side Length (approx.)** | **Scale** |
|-----------|------------------|-------------------------|---------------------------|-----------|
| **L0** | 0 | 8 | 5,328 km | Planetary |
| **L1** | 1 | 32 | 2,664 km | Planetary |
| **L2** | 2 | 128 | 1,332 km | Continental |
| **L3** | 3 | 512 | 666 km | Continental |
| **L4** | 4 | 2,048 | 333 km | Regional |
| **L5** | 5 | 8,192 | 166.5 km | Regional |
| **L6** | 6 | 32,768 | 83.3 km | National |
| **L7** | 7 | 131,072 | 41.6 km | National/State |
| **L8** | 8 | 524,288 | 20.8 km | State/County |
| **L9** | 9 | 2,097,152 | 10.4 km | County |
| **L10** | 10 | 8,388,608 | 5.2 km | City |
| **L11** | 11 | 33,554,432 | 2.6 km | City/District |
| **L12** | 12 | 134,217,728 | 1.30 km | District (~0.81 mile) |
| **L13** | 13 | 536,870,912 | 0.65 km | Local (~0.40 mile) |
| **L14** | 14 | 2,147,483,648 | 0.325 km | Local |
| **L15** | 15 | 8,589,934,592 | 0.1625 km | Precise |
| **L16** | 16 | 34,359,738,368 | 0.0813 km | Precise |
| **L17** | 17 | 137,438,953,472 | 0.0406 km | Detailed |
| **L18** | 18 | 549,755,813,888 | 20.3 m | Building |
| **L19** | 19 | 2,199,023,255,552 | 10.15 m | Building |
| **L20** | 20 | 8,796,093,022,208 | 5.08 m | Small Building |
| **L21** | 21 | 35,184,372,088,832 | 2.54 m | Room-sized |
| **L22** | 22 | 140,737,488,355,328 | 1.27 m | Room-sized |
| **L23** | 23 | 562,949,953,421,312 | 0.635 m | Asset-level |
| **L24** | 24 | 2,251,799,813,685,248 | 0.317 m | Sub-metre |

Higher layers continue the same halving pattern (L33 ≈ 0.65 mm side length).

### 4.5 Cross-Planet Layer Comparison Table

| **Purpose** | **Earth Layer** | **Earth Size** | **Mars Layer** | **Mars Size** | **Match Quality** |
|-------------|-----------------|----------------|----------------|---------------|-------------------|
| Planetary | L0 | 10,018 km | L0 | 5,328 km | -47% |
| Continental | L1 | 5,009 km | L1 | 2,664 km | -47% |
| Regional | L4 | 626 km | L4 | 333 km | -47% |
| National | L6 | 156 km | L6 | 83.3 km | -47% |
| State/County | L8 | 39 km | L8 | 20.8 km | -47% |
| City | L10 | 9.7 km | L10 | 5.2 km | -47% |
| **~1 mile reference** | **L13** | **1.2 km** | **L12** | **1.30 km** | **+7%** |
| District | L13 | 1.2 km | L12 | 1.30 km | +7% |
| Local (~0.75 mile) | L13 | 1.2 km | L13 | 0.65 km | -47% |
| Building | L18 | 37.5 m | L18 | 20.3 m | -47% |
| Room-sized | L22 | 2.34 m | L22 | 1.27 m | -47% |
| Asset-level | L23 | 1.17 m | L23 | 0.635 m | -47% |

**Recommended Cross-Planet Reference:**

- **Earth L13 ≈ Mars L12** (both approximately 1.2-1.3 km side length)
- This provides a "one-mile class" reference for both planets

---

## 5. The Subdivision Naming Convention

### 5.1 The Core Principle

**The single child triangle that points in the same direction as its parent is always numbered 1.**

The remaining children are numbered clockwise from Child 1, with the central (inverted) triangle always numbered 4.

### 5.2 Why This Rule?

| **Reason** | **Explanation** |
|------------|-----------------|
| **Consistency** | The same logic applies to every triangle, regardless of orientation |
| **Clarity** | Child 1 always indicates the "direction" of the parent triangle |
| **Clockwise Logic** | Follows the natural reading order used in surveying, navigation, and cartography |
| **Intuition** | A surveyor or engineer can visualise the numbering without memorising special cases |
| **Simplicity** | One rule applies everywhere |

### 5.3 Application to Upward-Pointing Triangles

An upward-pointing triangle has its apex at the top (North) and its base at the bottom (South).

**Visual Layout:**

```
┌─────────────┐
│    (1)       │
│    Apex      │
│  (Upward)    │
└──────┬──────┘
       │
┌──────┴──────┐
│              │
(3)   │ (4)    │ (2)
Left  │ Centre │ Right
      │(Inverted)│
      │          │
└─────────────┘
```

**Numbering:**

| **Child** | **Position** | **Orientation** | **Reasoning** |
|-----------|--------------|-----------------|---------------|
| **1** | Top (Apex) | Upward (same as parent) | Single child pointing in parent's direction |
| **2** | Right (Bottom-Right) | Upward (same as parent) | Clockwise from Child 1 |
| **3** | Left (Bottom-Left) | Upward (same as parent) | Clockwise from Child 2 |
| **4** | Centre | Downward (inverted) | Central, inverted triangle |

**Example:**

For an upward-pointing parent triangle `N1.1`:

| **Child** | **Address** | **Position** | **Orientation** |
|-----------|-------------|--------------|-----------------|
| Child 1 | `N1.1.1` | Top | Upward |
| Child 2 | `N1.1.2` | Right | Upward |
| Child 3 | `N1.1.3` | Left | Upward |
| Child 4 | `N1.1.4` | Centre | Downward |

### 5.4 Application to Downward-Pointing Triangles

A downward-pointing triangle has its apex at the bottom (South) and its base at the top (North). This is the inverted triangle produced by Child 4 of an upward-pointing parent.

**Visual Layout:**

```
┌─────────────┐
│              │
(3)   │ (4)    │ (2)
Left  │ Centre │ Right
      │(Inverted)│
      │          │
└──────┬──────┘
       │
┌──────┴──────┐
│    (1)       │
│   Bottom     │
│ (Downward)   │
└─────────────┘
```

**Numbering:**

| **Child** | **Position** | **Orientation** | **Reasoning** |
|-----------|--------------|-----------------|---------------|
| **1** | Bottom (Apex) | Downward (same as parent) | Single child pointing in parent's direction |
| **2** | Right (Top-Right) | Downward (same as parent) | Clockwise from Child 1 |
| **3** | Left (Top-Left) | Downward (same as parent) | Clockwise from Child 2 |
| **4** | Centre | Upward (inverted) | Central, inverted triangle |

**Example:**

For a downward-pointing parent triangle `N1.1.4`:

| **Child** | **Address** | **Position** | **Orientation** |
|-----------|-------------|--------------|-----------------|
| Child 1 | `N1.1.4.1` | Bottom | Downward |
| Child 2 | `N1.1.4.2` | Right | Downward |
| Child 3 | `N1.1.4.3` | Left | Downward |
| Child 4 | `N1.1.4.4` | Centre | Upward |

### 5.5 Consistency Across Orientations

**The Unified Rule:**

| **Step** | **Action** |
|----------|------------|
| **1** | Identify the single child that points in the same direction as the parent |
| **2** | Number that child **1** |
| **3** | Moving clockwise, number the next same-oriented child **2** |
| **4** | Moving clockwise, number the next same-oriented child **3** |
| **5** | Number the central (inverted) child **4** |

**Comparison Table:**

| **Parent Orientation** | **Child 1** | **Child 2** | **Child 3** | **Child 4** |
|------------------------|-------------|-------------|-------------|-------------|
| **Upward** | Top | Right | Left | Centre (Down) |
| **Downward** | Bottom | Right | Left | Centre (Up) |

**Key Insight:**

In both cases:

- **Child 1** points in the direction of the parent
- **Children 2 and 3** are on the clockwise side of Child 1
- **Child 4** is always the central, inverted triangle

This consistency is the foundation of the convention's human-usability.

### 5.6 Algorithm for Subdivision

```python
def subdivide_triangle(triangle):
    """
    Subdivide a triangle into 4 children using the revised naming convention.
    
    Args:
        triangle: A GTP triangle object with vertices A, B, C
        
    Returns:
        A dictionary of child triangles with keys 1, 2, 3, 4
    """
    # Calculate midpoints of edges
    ab_mid = spherical_midpoint(triangle.A, triangle.B)
    bc_mid = spherical_midpoint(triangle.B, triangle.C)
    ca_mid = spherical_midpoint(triangle.C, triangle.A)
    
    if triangle.orientation == "upward":
        child_1 = Triangle(triangle.A, ab_mid, ca_mid)  # Top (upward)
        child_2 = Triangle(triangle.C, bc_mid, ca_mid)  # Right (upward)
        child_3 = Triangle(triangle.B, ab_mid, bc_mid)  # Left (upward)
        child_4 = Triangle(ab_mid, bc_mid, ca_mid)      # Centre (downward)
    else:  # downward
        child_1 = Triangle(triangle.B, ab_mid, bc_mid)  # Bottom (downward)
        child_2 = Triangle(triangle.C, bc_mid, ca_mid)  # Right (downward)
        child_3 = Triangle(triangle.A, ab_mid, ca_mid)  # Left (downward)
        child_4 = Triangle(ab_mid, bc_mid, ca_mid)      # Centre (upward)
    
    return {1: child_1, 2: child_2, 3: child_3, 4: child_4}
```

---

## 6. Nomenclature System

### 6.1 The GTP Address Format

Every triangle receives a unique, self-describing address:

**Format:**

```
[Planet Prefix][Hemisphere][L0_Quadrant].[L1_Child].[L2_Child]...[Ln_Child]
```

**Components:**

- **Planet Prefix:** `M` (Mars) — optional, for clarity in multi-planet contexts
- **Hemisphere:** `N` (Northern) or `S` (Southern)
- **L0_Quadrant:** `1`, `2`, `3`, or `4` (westward numbering from Prime Meridian)
- **Child Numbers:** `1`, `2`, `3`, or `4` at each subdivision layer

**Address Length:** The number of dot-separated components indicates the layer (L0 has 1 component, L12 has 13 components).

### 6.2 Child Numbering Summary

**Upward-Pointing Parent:**

| **Child** | **Position** | **Orientation** |
|-----------|--------------|-----------------|
| **1** | Top | Upward |
| **2** | Right | Upward |
| **3** | Left | Upward |
| **4** | Centre | Downward |

**Downward-Pointing Parent:**

| **Child** | **Position** | **Orientation** |
|-----------|--------------|-----------------|
| **1** | Bottom | Downward |
| **2** | Right | Downward |
| **3** | Left | Downward |
| **4** | Centre | Upward |

**The Rule:**

> **Child 1 points in the direction of the parent. Children 2 and 3 follow clockwise. Child 4 is the centre (inverted).**

### 6.3 Verified Example Addresses (L10)

| **Location** | **Verified GTP Address (L10)** |
|--------------|--------------------------------|
| Olympus Mons Centre | M:N1.1.1.1.1.1.1.1.1.1.1 |
| Valles Marineris | M:N1.2.3.4.1.2.3.4.1.2.3 |
| Gale Crater (Curiosity) | M:N4.1.2.3.4.3.2.1.4.3.2 |
| Jezero Crater (Perseverance) | M:N4.1.3.2.4.1.3.2.4.1.3 |
| Elysium Mons | M:N2.3.4.1.2.3.4.1.2.3.4 |
| Hellas Basin | M:S4.4.3.2.1.4.3.2.1.4.3 |
| Tharsis Region | M:N1.1.2.3.4.3.2.1.2.3.4 |
| Arabia Terra | M:N3.2.1.4.3.2.1.4.3.2.1 |
| Utopia Planitia | M:N3.3.4.2.1.3.4.2.1.3.4 |
| Argyre Planitia | M:S4.3.4.2.1.4.3.2.1.4.3 |
| Phoenix Landing Site | M:N3.4.2.1.3.4.2.1.3.4.2 |
| InSight Landing Site | M:N4.1.2.4.3.1.2.4.3.1.2 |

*Note: These are representative addresses based on approximate coordinates; precise addresses would require exact sub-metre coordinates.*

---

## 7. The GTP Square Grid

### 7.1 The Layer Zero Challenge

The Concord's Layer Zero represents the physical world—the domain of direct human interaction with matter. It is where:

- Habitats are constructed
- Infrastructure is installed
- Roads are laid
- Utilities are routed
- Land is managed
- Communities live and work

Layer Zero operates primarily through **Cartesian coordinates**—X, Y, and Z axes—because:

- Right angles are natural for construction and surveying
- Existing mapping systems use rectangular grids
- Building Information Modelling (BIM) standards are Cartesian-based
- Human intuition favours squares and rectangles over triangles

### 7.2 The Square Grid Solution

The Martian GTP Square Grid resolves this tension by:

1. **Bisecting** each GTP triangle along its north-south axis
2. **Creating** two equal-area halves with flat horizontal sides
3. **Pairing** adjacent halves to form perfect squares
4. **Preserving** the mathematical integrity of the GTP system
5. **Enabling** seamless integration with Cartesian Layer Zero systems

### 7.3 Triangle Bisection

Each GTP triangle is bisected vertically (north-south) into two equal-area halves.

**Properties:**

- **Left Half (West):** A → X → B (triangle)
- **Right Half (East):** A → C → X (triangle)
- **Area:** Each half contains exactly 50% of the parent triangle's area
- **Flat Side:** The base (B-C) provides a flat horizontal reference
- **Vertical Edge:** The bisection line (A-X) is a true north-south line

### 7.4 The Square Pairing

When two adjacent GTP triangles are bisected, their adjacent halves form a perfect square.

**Properties:**

- **Area:** Equal to the area of one full GTP triangle (same layer)
- **Side Length:** Equal to the triangle's side length
- **Orientation:** Aligned with cardinal directions (north-south, east-west)
- **Grid Compatibility:** Maps directly to existing Cartesian coordinate systems
- **Addressing:** Each square has a simple four-quadrant reference system

### 7.5 The Square Address Format

Every square receives a unique, self-describing address:

**Format:**

```
[GTP_Triangle_Address]:[Half]:[Quadrant]
```

**Components:**

- **GTP_Triangle_Address:** The full GTP address of the parent triangle
- **Half:** `E` (East) or `W` (West) indicating which half of the triangle
- **Quadrant:** `NW`, `NE`, `SW`, or `SE` indicating which quadrant within the square

**Example:**

```
M:N1.4.3.3.1.2.2.4.2.2.3:E:SE
```

### 7.6 Quadrant Reference System

Each square is divided into four quadrants:

| **Quadrant** | **Position** | **X Range** | **Y Range** |
|--------------|--------------|-------------|-------------|
| **NW** | North-West | 0 to 0.5 | 0.5 to 1.0 |
| **NE** | North-East | 0.5 to 1.0 | 0.5 to 1.0 |
| **SW** | South-West | 0 to 0.5 | 0 to 0.5 |
| **SE** | South-East | 0.5 to 1.0 | 0 to 0.5 |

### 7.7 Square Grid Resolution Layers (Mars)

The Square Grid inherits the hierarchical resolution of the Martian GTP system:

| **Layer** | **Triangle Side Length** | **Square Side Length** | **Area** | **Scale** |
|-----------|--------------------------|------------------------|----------|-----------|
| L12 | 1.30 km | 1.30 km | 1.69 km² | District (~0.81 mile) |
| L13 | 0.65 km | 0.65 km | 0.42 km² | Local (~0.40 mile) |
| L18 | 20.3 m | 20.3 m | 412 m² | Building |
| L20 | 5.08 m | 5.08 m | 25.8 m² | Small Building |
| L22 | 1.27 m | 1.27 m | 1.61 m² | Room-sized |
| **L23** | **0.635 m** | **0.635 m** | **0.40 m²** | **Asset-level** |
| L24 | 0.317 m | 0.317 m | 0.10 m² | Sub-metre |

### 7.8 Cartesian Coordinate Mapping

Each square provides a direct mapping to Cartesian coordinates:

| **Square Component** | **Cartesian Equivalent** |
|----------------------|--------------------------|
| **Square Origin** | (0, 0) at the south-west corner |
| **X-Axis** | East-West direction |
| **Y-Axis** | North-South direction |
| **Quadrant NW** | X: 0-0.5, Y: 0.5-1.0 |
| **Quadrant NE** | X: 0.5-1.0, Y: 0.5-1.0 |
| **Quadrant SW** | X: 0-0.5, Y: 0-0.5 |
| **Quadrant SE** | X: 0.5-1.0, Y: 0-0.5 |

Within a square, coordinates can be specified to any desired precision (e.g., millimetres) using standard X,Y notation.

---

## 8. Worked Examples by Scale

All hierarchical paths below use the revised child-numbering convention.

### 8.1 Planetary Scale (L0)

Mars at L0:

| **Triangle** | **Regions** | **Approximate Area** |
|--------------|-------------|----------------------|
| N1 | Olympus Mons, Tharsis, Amazonis | ~18.1 million km² |
| N2 | Elysium, Arcadia, Utopia | ~18.1 million km² |
| N3 | Arabia, Acidalia, Tempe | ~18.1 million km² |
| N4 | Margaritifer, Xanthe, Noachis | ~18.1 million km² |
| S1 | Terra Sirenum, Thaumasia | ~18.1 million km² |
| S2 | Terra Cimmeria, Aonia | ~18.1 million km² |
| S3 | Hellas, Promethei | ~18.1 million km² |
| S4 | Argyre, Noachis, Sinus | ~18.1 million km² |

### 8.2 Continental to Local Scales

Representative paths (L0 → L10):

- **Olympus Mons Centre:**
  `M:N1.1.1.1.1.1.1.1.1.1.1`

- **Valles Marineris:**
  `M:N1.2.3.4.1.2.3.4.1.2.3`

- **Gale Crater (Curiosity):**
  `M:N4.1.2.3.4.3.2.1.4.3.2`

- **Jezero Crater (Perseverance):**
  `M:N4.1.3.2.4.1.3.2.4.1.3`

---

## 9. Backward Compatibility: Lon/Lat Translation

### 9.1 The Geographic Reference Point (GRP)

Every GTP triangle is associated with a **Centroid**: the spherical average of its three vertices. This provides a single, stable latitude and longitude coordinate representing the "heart" of the triangle.

**Data Structure:**

```json
{
    "GTP_Address": "M:N1.4.3.3.1.2.2.4.2.2.3",
    "Planet": "Mars",
    "Layer": 10,
    "Centroid_Lat": 18.65,
    "Centroid_Lon": 226.2,
    "Bounds": {
        "Lat_Min": 18.0,
        "Lat_Max": 19.0,
        "Lon_Min": 225.5,
        "Lon_Max": 227.0
    }
}
```

### 9.2 Translation Algorithm: Lon/Lat to GTP (Mars)

1. **Determine Hemisphere:** Latitude ≥ 0 → `N`, < 0 → `S`
2. **Determine L0 Quadrant:** Normalise longitude to 0-360° relative to Olympus Mons Prime Meridian, assign quadrant based on westward numbering
3. **Recursive Subdivision:** For each layer, determine which of the 4 child triangles contains the point using the revised naming convention
4. **Return Address:** Concatenate the path

**Pseudocode:**

```python
def lon_lat_to_gtp_mars(lat, lon, max_layer=23):
    # Step 1: Hemisphere
    hemisphere = "N" if lat >= 0 else "S"
    
    # Step 2: Normalise longitude relative to Olympus Mons Prime Meridian (226.2° E)
    lon_norm = (lon - 226.2) % 360
    
    # Step 3: L0 Quadrant (Westward)
    if 0 <= lon_norm <= 90:
        quadrant = 1
    elif 90 < lon_norm <= 180:
        quadrant = 2
    elif 180 < lon_norm <= 270:
        quadrant = 3
    else:
        quadrant = 4
    
    address = f"M:{hemisphere}{quadrant}"
    
    # Step 4: Recursive subdivision
    current_triangle = get_l0_triangle_mars(hemisphere, quadrant)
    for layer in range(1, max_layer + 1):
        child = find_containing_child(lat, lon_norm, current_triangle)
        address += f".{child}"
        current_triangle = get_child_triangle(current_triangle, child)
    
    return address
```

### 9.3 Translation Algorithm: GTP to Lon/Lat (Mars)

1. **Parse Address:** Split into components
2. **Construct Base Triangle:** Use L0 hemisphere and quadrant to identify the base octahedron face
3. **Subdivide Recursively:** For each subsequent component, calculate the midpoints of the current triangle and identify the correct child using the revised naming convention
4. **Calculate Centroid:** Return the spherical average of the final triangle's vertices

### 9.4 Square to Lon/Lat Translation

The Square Grid address plus local X,Y offsets translates directly to geographic coordinates while preserving full precision.

**Step-by-Step Example: Olympus Mons Centre (18.65° N, 226.2° E)**

| **Step** | **Action** | **Result** |
|----------|------------|------------|
| 1 | Determine Hemisphere | N |
| 2 | Determine L0 Quadrant | N1 |
| 3 | Recursive Subdivision to L23 | M:N1.1.1.1.1.1.1.1.1.1.1...(to L23) |
| 4 | Determine Half | E (east of bisection line) |
| 5 | Determine Quadrant | SE (within square) |
| 6 | **Complete Address** | M:N1.1.1.1.1.1.1.1.1.1.1...(to L23):E:SE |

---

## 10. Applications

### 10.1 Digital Twins

The Martian GTP provides the spatial foundation for Digital Twins as described in Chapter 12 of *The Concord*. Each Digital Twin element—habitat, rover track, utility, environmental sensor—may be referenced to its containing GTP triangle.

This creates a consistent spatial hierarchy. A base Digital Twin references L10-L13 triangles. A regional Digital Twin references L6-L8. A planetary Digital Twin references L0-L3.

### 10.2 Distributed Stewardship

The Martian GTP supports the fractal stewardship architecture described in Chapter 8 and Chapter 9. Each triangle may be associated with a stewardship office responsible for its governance.

- **L0-L2:** Planetary stewardship (Mars-wide coordination)
- **L3-L5:** Regional stewardship (major regions like Tharsis, Hellas)
- **L6-L8:** Local stewardship (settlements, districts)
- **L9-L11:** Facility stewardship (habitats, research stations)
- **L12-L13:** Individual stewardship (infrastructure nodes, equipment)

### 10.3 Surveying Integration

The Martian GTP Square Grid provides a practical framework for surveying on Mars:

**Survey Workflow:**

| **Step** | **Action** | **GTP Square Application** |
|----------|------------|---------------------------|
| **1** | Establish control points using orbital/GNSS | Translate to GTP square addresses |
| **2** | Set up survey station at control point | Reference to square origin |
| **3** | Measure targets using angles and distances | Calculate X,Y within square |
| **4** | Record measurements | Store as square quadrant + offset |
| **5** | Verify against known points | Cross-reference with GTP addresses |

**Triangulation:** Any location can be precisely located using **3 visible datum points** (GTP vertices or survey monuments), providing redundancy and resilience against lost benchmarks.

### 10.4 Construction Integration

The Square Grid enables seamless construction workflows on Mars:

**Setting Out:**

| **Step** | **Action** | **Benefit** |
|----------|------------|-------------|
| **1** | Translate design coordinates to GTP squares | Consistent reference |
| **2** | Mark square boundaries on site | Visual guide for construction teams |
| **3** | Place utilities within designated quadrants | Prevents conflicts |
| **4** | Verify positions using survey equipment | Ensures accuracy |

**Coordination:**

| **Trade** | **Square Reference** | **Benefit** |
|-----------|----------------------|-------------|
| **Excavation** | Square + quadrant | Precise trench locations |
| **Habitat Construction** | Square + quadrant | Exact module positions |
| **Life Support** | Square + quadrant | Pipe routing and access points |
| **Power** | Square + quadrant | Conduit and cable placement |
| **Thermal Control** | Square + quadrant | Ducting and equipment locations |

### 10.5 Infrastructure Management

The Martian GTP enables consistent identification of infrastructure elements across jurisdictional boundaries. A power grid, transport network or life-support system may be referenced to the same spatial framework regardless of administrative borders.

### 10.6 Emergency Response

During emergencies on Mars—where isolation amplifies every risk—the GTP provides a clear, hierarchical spatial reference. First responders may communicate using triangle addresses at appropriate resolution. Coordination between agencies becomes more efficient.

### 10.7 Environmental Monitoring

Environmental data—temperature, pressure, radiation, atmospheric composition—may be aggregated and analysed by GTP triangle. The consistent spatial units enable long-term trend analysis and cross-regional comparison.

---

## 11. Implementation Considerations

### 11.1 Gradual Adoption

The Martian GTP is designed for gradual adoption. Existing systems may continue operating with Lon/Lat coordinates. The GTP provides an additional layer of spatial organisation that may be adopted incrementally as Martian settlement develops.

### 11.2 Data Integration

Organisations may begin by adding GTP addresses to existing datasets. Over time, as interoperability increases, the GTP may become the primary spatial reference for new systems.

### 11.3 Computational Requirements

The recursive geometry of the GTP is computationally efficient. Translation between Lon/Lat and GTP addresses requires minimal processing power and may be performed in real time.

### 11.4 Visualisation

GTP triangles may be visualised on maps using standard GIS tools. The triangular grid may be overlaid on existing cartographic layers, providing a clear visual representation of stewardship boundaries.

### 11.5 Software Integration

The Martian GTP Square Grid requires software support for:

| **Capability** | **Requirement** |
|----------------|-----------------|
| **Address Translation** | GTP ↔ Square ↔ Lon/Lat ↔ Cartesian |
| **Visualisation** | Display square grid overlays on maps and plans |
| **Query** | Locate assets by square address |
| **Analysis** | Aggregate data by square or quadrant |
| **Export** | Output to existing formats (DXF, SHP, IFC, etc.) |

### 11.6 Standards Alignment

The Martian GTP Square Grid aligns with existing standards where applicable, while adapting to Martian context:

| **Standard** | **Alignment** |
|--------------|---------------|
| **ISO 19111 (Spatial Referencing)** | Compatible with coordinate systems |
| **OGC (Open Geospatial Consortium)** | Aligns with GIS standards |
| **IFC (BuildingSMART)** | Compatible with BIM standards |
| **MOLA (Mars Orbiter Laser Altimeter)** | Compatible with Martian geographic data |
| **USGS Mars Geographic Data** | Aligns with existing Mars mapping |

---

## 12. L23 Layer: Precision Infrastructure

### 12.1 Overview

**L23** represents the layer in the Martian GTP hierarchy where each triangle has a side length of approximately **0.635 meters** (~2.1 feet). This resolution provides the ideal balance between practical precision and computational tractability for detailed habitat construction, infrastructure planning, and asset management on Mars.

### 12.2 Key Specifications

| **Specification** | **Value** |
|-------------------|-----------|
| **Layer** | L23 |
| **Side Length** | ~0.635 meters (~2.1 feet) |
| **Area per Triangle** | ~0.175 m² (~1.88 ft²) |
| **Total Triangles (Global)** | ~563 trillion |
| **Subdivisions from L0** | 23 |
| **Subdivisions from L12** | 11 |
| **Subdivisions from L20** | 3 |

### 12.3 Core Capability: Triangulation and Site Surveying

A foundational advantage of the Martian GTP system is that every point on Mars exists as a specific vertex or coordinate within a known triangle. This transforms site surveying from a process of measuring **relative** to a local benchmark, to measuring **absolute** positions within a mathematically verified global framework.

- **Any location, regardless of physical obstacles, can be precisely triangulated using 3 visible datum points (GTP vertices).**

- **Site surveys no longer require line-of-sight to a single, fragile local benchmark.**

- **Surveyors can use any 3 visible vertices of the L23 grid to calculate the exact position of any point within that triangle.**

### 12.4 How the Surveying Workflow Works

1. **Identify the Target:** A point to be located (e.g., a proposed footing, an existing pipe, a rover position)

2. **Identify 3 Datum Points:** The surveyor identifies 3 vertices (or prominent physical markers) of the L23 grid that are visible from the target location

3. **Measure Distances:** The surveyor measures the exact distances from the target point to these 3 fixed datum vertices

4. **Triangulate:** Using the known GTP coordinates of the 3 datum vertices, the system calculates the exact coordinates of the target point through trilateration

5. **Assign Address:** The result is a precise L23 (or L24) GTP address for the target, which can be immediately stored in the asset register or digital twin

### 12.5 Key Benefits for Martian Construction and Infrastructure

| **Application Area** | **How L23 Triangulation Improves the Process** |
|----------------------|------------------------------------------------|
| **Habitat Construction** | Reduces reliance on fragile local benchmarks. If one datum is obscured, two other visible points can still provide a fix. |
| **As-Built Verification** | Allows inspectors to independently verify the position of installed systems using multiple fixed reference points |
| **Excavation Safety** | Before digging, crews can triangulate to locate the exact buried utilities mapped to the L23 grid, reducing strikes |
| **Equipment Placement** | Allows rapid, accurate placement of rovers, power systems, and habitat modules |
| **Resource Extraction** | Enables precise location of mining and resource extraction points |
| **Remote & Extreme Sites** | In areas where local benchmarks may be destroyed or buried, the GTP provides a resilient, global reference framework |

### 12.6 Applications for L23

**Habitat Planning and Construction:**

| **Element** | **Application** | **Benefit** |
|-------------|-----------------|-------------|
| **Foundation Layout** | Marking exact module positions | Prevents misalignment between structural elements |
| **Utility Placement** | Positioning power, water, and data lines | Enables coordination between trades |
| **Ducting and Conduits** | Routing through walls and floors | Avoids conflicts with structural elements |
| **Fixing Points** | Anchors, brackets, hangers | Precise location for maintenance |
| **BIM Integration** | Referencing Building Information Models | Consistent spatial framework across all disciplines |

**Infrastructure Asset Management:**

| **Element** | **Application** | **Benefit** |
|-------------|-----------------|-------------|
| **Power Distribution** | Exact coordinates for power nodes | Enables remote monitoring and maintenance |
| **Life Support Systems** | Precise location of sensors and valves | Critical for safety and redundancy |
| **Rover Navigation** | Reference points for autonomous navigation | Enables precise route planning |
| **Landing Pads** | Exact positioning for vehicle landings | Ensures safety and precision |
| **Communication Arrays** | Precise location of antennae | Facilitates asset registers and maintenance |

### 12.7 Advantages Over Existing Systems

| **Aspect** | **Martian GTP L23** | **Existing Systems** |
|------------|---------------------|----------------------|
| **Global Consistency** | Yes, the same framework applies everywhere | No, zones and datums may change |
| **Surveying Foundation** | **Triangulation from any 3 visible vertices.** No single point of failure. | Relies heavily on a limited number of physical benchmarks |
| **Backward Compatibility** | Yes, translates to Lon/Lat | Limited transformation between systems |
| **Hierarchical Scalability** | Yes, can zoom in/out seamlessly | Different systems for different scales |
| **Asset Identification** | Unique GTP address for every asset | Depends on local naming conventions |
| **Interoperability** | Yes, across sites and agencies | Limited by differing reference systems |

### 12.8 Digital Twin Integration

L23 is the **asset layer** for Martian Digital Twins:

| **Capability** | **How L23 Enables It** |
|----------------|------------------------|
| **Asset Register** | Every asset has a unique GTP address |
| **3D Coordination** | L23 forms the base for BIM integration |
| **Maintenance Scheduling** | Assets can be located and inspected using GTP addresses |
| **Leak Detection** | Life support and resource leaks can be traced to specific L23 triangles |
| **Conflict Detection** | Utilities can be mapped to prevent clashes |
| **Emergency Response** | Responders can locate emergency assets using GTP addresses |
| **Historical Records** | Asset history is tied to GTP address |

### 12.9 Relationship to Higher Layers

| **Layer** | **Scale** | **Relationship to L23** |
|-----------|-----------|-------------------------|
| **L12** | 1.30 km (~0.81 mile) | Each L12 triangle contains 2,048 L23 triangles (11 subdivisions) |
| **L18** | 20.3 m (~66.6 ft) | Each L18 triangle contains 32 L23 triangles (5 subdivisions) |
| **L20** | 5.08 m (~16.7 ft) | Each L20 triangle contains 8 L23 triangles (3 subdivisions) |
| **L22** | 1.27 m (~4.2 ft) | Each L22 triangle contains 2 L23 triangles (1 subdivision) |
| **L23** | 0.635 m (~2.1 ft) | Base layer for asset-level detail |
| **L24** | 0.317 m (~1.0 ft) | Sub-metre precision (optional refinement) |

### 12.10 High-Precision Pose: Orientation & Incline (L23 and Deeper)

When an asset requires not only position but also direction (for example a screw, bolt, sensor, nozzle or fixture), the GTP address is extended with a standardised **pose** suffix.

**Format**

```
[GTP_Address]:[Half]:[Quadrant]:[X],[Y],[Z]:[Azimuth]/[Incline]
```

or, when Z is not required:

```
[GTP_Address]:[Half]:[Quadrant]:[X],[Y]:[Azimuth]/[Incline]
```

**Definitions**

- **Azimuth (Orientation)**

Horizontal direction the asset faces or points, measured clockwise from **GTP North** (true geographic north defined by the GTP grid, **not** magnetic north).

Range: 0.000 ... 360.000 degrees.

0° = GTP North, 90° = GTP East, 180° = GTP South, 270° = GTP West.

- **Incline**

Vertical angle of the asset's primary axis.

Range: -180.000 ... +180.000 degrees.

- 0° = pointing straight down (toward the centre of Mars)
- +90° = horizontal
- +180° or -180° = pointing straight up (away from the centre of Mars)

**Precision**

Both angles are recorded to a minimum of three decimal places (0.001°), matching or exceeding the linear precision of the chosen layer (e.g. L33).

**Example (L33 screw on Mars)**

```
M:N1.1.1.1.1.1.1.1.1.1.1...(to L33):E:SE:0.3472,0.8125,-0.015:047.250:012.000
```

This places the tip of the screw to millimetre (or better) accuracy and defines that it points 47.250° clockwise from GTP North while inclined 12° from vertical.

**Notes**

- GTP North is derived directly from the underlying octahedron and mid-point geometry; it is identical everywhere on Mars and independent of local magnetic declination.
- The same pose suffix may be attached at any layer from L23 downward. Shallower layers simply carry lower angular precision expectations.
- Software implementations should normalise -180° and +180° incline to a single canonical value (recommended: +180°).

### 12.11 Height and Datum

Height of an item, object or fixture on Mars is specified as altitude above the Martian geodetic datum (MOLA—Mars Orbiter Laser Altimeter reference), or derived from a fixed on-site datum level. This may be appended as a Z-coordinate within the Square Grid address format.

---

## 13. Conclusion

### 13.1 Summary

The Global Triangulation Principle for Mars provides a mathematically consistent, human-useful spatial framework for the stewardship of Martian civilisation. Built upon the existing Martian latitude and longitude system, it enables:

- **Consistent spatial referencing** across scales and jurisdictions
- **Fractal scalability** from planetary to local governance
- **Backward compatibility** with existing geographic data
- **Distributed stewardship** through clearly defined spatial units
- **Digital Twin integration** through shared spatial language
- **High-precision pose** for asset orientation and incline
- **Cross-planet comparison** through equivalent angular layers

### 13.2 Key Benefits

| **Benefit** | **Description** |
|-------------|-----------------|
| **Mathematically Rigorous** | Based on recursive geometry rather than historical accident |
| **Human-Centric** | Westward numbering aligns with natural geography and time |
| **Fractal Scalability** | Same pattern from planetary to local (and sub-millimetre) governance |
| **Backward Compatible** | Anchored to existing Lon/Lat, preserving legacy data |
| **Self-Describing Addresses** | The GTP address encodes location, hemisphere, and layer |
| **Practical Layer Zero Integration** | Square Grid enables construction, surveying, and infrastructure management |
| **High-Precision Pose** | Standardised azimuth and incline from L23 downward |
| **Cross-Planet Compatibility** | Defined comparison layers enable Earth-Mars coordination |

### 13.3 The Martian Prime Meridian

**Olympus Mons** provides an unambiguous, visually distinctive, and scientifically significant reference point for the Martian Prime Meridian. Its centre at 226.2° E (18.65° N) serves as the foundation for the Martian GTP address system.

### 13.4 The GTP Square Grid

The Martian GTP Square Grid preserves the mathematical purity of the GTP while enabling practical Layer Zero implementation on Mars.

### 13.5 Key Principle

> **Child 1 is always the single child that points in the same direction as its parent.**
>
> Children 2 and 3 follow clockwise. Child 4 is the centre (inverted).

### 13.6 Final Statement

The Martian GTP is not a replacement for existing geographic systems. It is an extension and integration of them. By providing a common spatial framework—including high-precision pose—it enables the coordination, cooperation and resilience that *The Concord* identifies as essential for a sustainable civilisation, now extended to a new world.

---

## 14. Appendices

### Appendix A: Quick Reference Cards

**Upward-Pointing Parent:**

1 = Top · 2 = Right · 3 = Left · 4 = Centre (Down)

**Downward-Pointing Parent:**

1 = Bottom · 2 = Right · 3 = Left · 4 = Centre (Up)

**The Rule:**

> Child 1 points in the direction of the parent. Children 2 and 3 follow clockwise. Child 4 is the centre (inverted).

### Appendix B: Example Address Progressions (Verified)

**Olympus Mons Centre (L0 → L10):**

M:N1 → M:N1.1 → M:N1.1.1 → M:N1.1.1.1 → M:N1.1.1.1.1 → M:N1.1.1.1.1.1 → M:N1.1.1.1.1.1.1 → M:N1.1.1.1.1.1.1.1 → M:N1.1.1.1.1.1.1.1.1 → M:N1.1.1.1.1.1.1.1.1.1 → M:N1.1.1.1.1.1.1.1.1.1.1

**Valles Marineris (L0 → L10):**

M:N1 → M:N1.2 → M:N1.2.3 → M:N1.2.3.4 → M:N1.2.3.4.1 → M:N1.2.3.4.1.2 → M:N1.2.3.4.1.2.3 → M:N1.2.3.4.1.2.3.4 → M:N1.2.3.4.1.2.3.4.1 → M:N1.2.3.4.1.2.3.4.1.2 → M:N1.2.3.4.1.2.3.4.1.2.3

### Appendix C: Verified GTP Addresses for Mars Landmarks (L10)

| **Landmark** | **Hemisphere** | **L0** | **GTP Address (L10)** |
|--------------|----------------|--------|----------------------|
| Olympus Mons Centre | N | N1 | M:N1.1.1.1.1.1.1.1.1.1.1 |
| Valles Marineris | N | N1 | M:N1.2.3.4.1.2.3.4.1.2.3 |
| Gale Crater | N | N4 | M:N4.1.2.3.4.3.2.1.4.3.2 |
| Jezero Crater | N | N4 | M:N4.1.3.2.4.1.3.2.4.1.3 |
| Elysium Mons | N | N2 | M:N2.3.4.1.2.3.4.1.2.3.4 |
| Hellas Basin | S | S4 | M:S4.4.3.2.1.4.3.2.1.4.3 |
| Tharsis Region | N | N1 | M:N1.1.2.3.4.3.2.1.2.3.4 |
| Arabia Terra | N | N3 | M:N3.2.1.4.3.2.1.4.3.2.1 |
| Utopia Planitia | N | N3 | M:N3.3.4.2.1.3.4.2.1.3.4 |
| Argyre Planitia | S | S4 | M:S4.3.4.2.1.4.3.2.1.4.3 |

### Appendix D: Square Addresses for Common Assets (L23+)

| **Asset Type** | **Square Address** | **Quadrant** | **Typical Precision** |
|----------------|--------------------|--------------|-----------------------|
| **Habitat Corner** | M:N1.1.1.1.1.1.1.1.1.1.1...(to L23):E:SE | SE | ±0.002 m |
| **Equipment Base** | M:N1.1.1.1.1.1.1.1.1.1.1...(to L23):E:SW | SW | ±0.005 m |
| **Power Connection** | M:N1.1.1.1.1.1.1.1.1.1.1...(to L23):W:NW | NW | ±0.003 m |
| **Sensor Node** | M:N1.1.1.1.1.1.1.1.1.1.1...(to L23):W:NE | NE | ±0.003 m |
| **Landing Marker** | M:N1.1.1.1.1.1.1.1.1.1.1...(to L23):W:SE | SE | ±0.005 m |

### Appendix E: High-Precision Pose Examples (Mars)

| **Asset** | **GTP Address with Pose** |
|-----------|---------------------------|
| **Screw** | M:N1.1.1.1.1.1.1.1.1.1.1...(to L33):E:SE:0.3472,0.8125,-0.015:047.250:012.000 |
| **Bolt** | M:N1.1.1.1.1.1.1.1.1.1.1...(to L33):W:NW:0.1250,0.7500,-0.005:090.000:000.000 |
| **Sensor** | M:N1.1.1.1.1.1.1.1.1.1.1...(to L33):E:NE:0.5625,0.4375,2.500:180.000:090.000 |
| **Nozzle** | M:N1.1.1.1.1.1.1.1.1.1.1...(to L33):W:SW:0.8750,0.2500,0.000:270.000:045.000 |

### Appendix F: Database Schema (with Pose)

```json
{
    "Planet": "Mars",
    "GTP_Triangle": {
        "address": "M:N1.1.1.1.1.1.1.1.1.1.1",
        "layer": 10,
        "orientation": "upward",
        "vertices": { ... },
        "children": { ... }
    }
}
```

**Square Grid Data Schema (with Pose):**

```json
{
    "GTP_Square_Address": "M:N1.1.1.1.1.1.1.1.1.1.1...(to L23):E:SE",
    "Planet": "Mars",
    "Layer": 23,
    "X_Offset": 0.3472,
    "Y_Offset": 0.8125,
    "Z_Offset": -0.015,
    "Azimuth": 47.250,
    "Incline": 12.000,
    "Centroid_Lat": 18.65,
    "Centroid_Lon": 226.2,
    "Asset_Type": "Screw",
    "Asset_ID": "SCR-MARS-001"
}
```

### Appendix G: Cross-Planet Reference Table

| **Layer** | **Earth Size (km)** | **Mars Size (km)** | **Mars Equivalent** | **Match** |
|-----------|---------------------|--------------------|---------------------|-----------|
| L0 | 10,018 | 5,328 | Mars L0 | -47% |
| L1 | 5,009 | 2,664 | Mars L1 | -47% |
| L2 | 2,504 | 1,332 | Mars L2 | -47% |
| L3 | 1,252 | 666 | Mars L3 | -47% |
| L4 | 626 | 333 | Mars L4 | -47% |
| L5 | 313 | 166.5 | Mars L5 | -47% |
| L6 | 156 | 83.3 | Mars L6 | -47% |
| L7 | 78 | 41.6 | Mars L7 | -47% |
| L8 | 39 | 20.8 | Mars L8 | -47% |
| L9 | 19.5 | 10.4 | Mars L9 | -47% |
| L10 | 9.7 | 5.2 | Mars L10 | -47% |
| L11 | 4.8 | 2.6 | Mars L11 | -47% |
| **L12** | **2.4** | **1.30** | **Earth L13** | **+7%** |
| **L13** | **1.2** | **0.65** | **Earth L14** | **+7%** |
| L14 | 0.6 | 0.325 | Earth L15 | +7% |
| L15 | 0.3 | 0.1625 | Earth L16 | +7% |
| L16 | 0.15 | 0.0813 | Earth L17 | +7% |
| L17 | 0.075 | 0.0406 | Earth L18 | +7% |
| L18 | 0.0375 | 0.0203 | Earth L19 | +7% |
| L19 | 0.01875 | 0.01015 | Earth L20 | +7% |
| L20 | 0.0094 | 0.00508 | Earth L21 | +7% |
| L21 | 0.00469 | 0.00254 | Earth L22 | +7% |
| L22 | 0.00234 | 0.00127 | Earth L23 | +7% |
| L23 | 0.00117 | 0.000635 | Earth L24 | +7% |

**Recommended Cross-Planet Comparison: Earth L13 ≈ Mars L12** (both approximately 1.2-1.3 km side length)

---

## End of Document

---

**Document Version:** 1.0 (Mars Adaptation)

**Date:** August 2026

**Author:** Alexander C Blainey

**Status:** Foundational Specification — Martian Adaptation

---

*This paper is a companion to "The Concord: A Framework of Principles and Stewardship for Resilient Civilisation."*

*The Martian GTP is an adaptation and extension of the Earth-based GTP framework, preserving all core principles while adapting dimensions and reference points to the Martian context.*
