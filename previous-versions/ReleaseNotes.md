# PLDO Release Notes

Planar Lattice Defect Ontology (PLDO)

## v0.3.0

Major expansion of stacking fault coverage. This release introduces a detailed hierarchy of stacking fault types and their associated energies, along with new geometric descriptors.

### New Classes (10)

**Stacking Fault Types**
- `IntrinsicStackingFault` — intrinsic stacking fault subtype
- `ExtrinsicStackingFault` — extrinsic stacking fault subtype
- `I1StackingFault` — first intrinsic stacking fault variant
- `I2StackingFault` — second intrinsic stacking fault variant
- `Twin-likeStackingFault` — stacking fault with twin-like character

**Stacking Fault Energies**
- `StackingFaultEnergy` — general stacking fault energy class
- `GeneralizedStackingFaultEnergy` — energy for the generalized (gamma-surface) stacking fault
- `ExtrinsicStackingFaultEnergy`
- `I1StackingFaultEnergy`
- `I2StackingFaultEnergy`

### New Object Properties (1)
- `hasStackingFaultEnergy` — links a stacking fault to its associated energy

### New Datatype Properties (3)
- `hasDisplacementVector` — displacement vector characterising the stacking fault
- `hasSFplane` — crystallographic plane of the stacking fault
- `hasStackingSequence` — atomic layer stacking sequence notation

---

## v0.2.0

This release elevates PLDO from a purely geometric/crystallographic vocabulary to one that also covers computed properties of planar defects.

### New Classes (8)
- `ComputationalSample` — represents a simulated material sample
- `PhysicalQuantity` — top-level class for quantities
- `Energy` — general energy quantity
- `GrainBoundaryEnergy` — energy associated with grain boundaries
- `SurfaceEnergy` — surface or cleavage energy
- `WorkOfSeparation` — energy required to separate two surfaces
- `Gamma-Surface` — generalised stacking fault energy surface
- `CalculatedProperty` — a property obtained from simulation

### New Object Properties (2)
- `hasGrainBoundaryEnergy` — links a grain boundary to its energy
- `hasSurfaceEnergy` — links a surface to its energy

---

## v0.0.1

Initial release of PLDO.

### Classes (11)
Geometric planar defect hierarchy: `PlanarDefect`, `GrainBoundary`, `LowAngleGrainBoundary`, `TiltGrainBoundary`, `TwistGrainBoundary`, `MixedGrainBoundary`, `SymmetricalTiltGrainBoundary`, `TwinBoundary`, `AntiphaseBoundary`, `StackingFault`, `Surface`

### Object Properties (2)
`hasTiltComponent`, `hasTwistComponent`

### Datatype Properties (7)
`geometricalDegreesOfFreedom`, `macroscopicDegreesOfFreedom`, `microscopicDegreesOfFreedom`, `hasGBplane`, `hasMisorientationAngle`, `hasRotationAxis`, `hasSigmaValue`
