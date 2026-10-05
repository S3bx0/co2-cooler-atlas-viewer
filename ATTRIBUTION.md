# Attribution and model provenance

## Static delivery permission boundary

The portable-model implementation adds local generation, lossless transport
compression, manifest verification and static rendering of the **same** geometry.
On **2026-10-05**, the project owner explicitly attested to rights or the rights
holder's permission for public distribution of the existing eleven `current-2kh-3ar`
derived packets and their inclusion in this private repository and its clone
history. The source-bound `public` and `repository` grants in
[`config/model-publication.json`](config/model-publication.json) record that
attestation, approver, date and scope. This is not independent manufacturer
verification and does not relicense manufacturer-derived geometry under MIT.

The approved release supplies those packets and their manifest under `public/models/`
so a clone of that revision can load the current model without the original CAD.
The original GLB, private drawings, workbooks, detailed source reports and credentials
remain excluded. `authenticated` and `sourceCi` remain null; no separate grant for
the authenticated build target or cloud processing of the original was recorded.
Local preview trees remain ignored and are not public upload artifacts.

Commit/push and application publication were also approved on October 5. Hosting
activation remains blocked by the Pages HTTP 422 plan response and Vercel HTTP 403
team-authentication response; no live deployment is confirmed. See
[delivery and hosting](docs/model-delivery.md) for the prepared root-base alternative.

Historical descriptions below refer to the earlier loopback development stages.
Their statements excluding packets from Git or production describe those stages
before the October 5 attestation. Their manufacturer provenance, distinctions
between source surfaces and reconstruction, and engineering limitations remain
unchanged. The new distribution scope is limited to the existing eleven delivery packets.

The optional 3A-R structural refinement follows the user's visual request for
one V per truss, four purlins and a smaller rear panel-to-column gap. The chosen
40 mm display gap and revised web/purlin layout are not source-certified
dimensions or a structural calculation. Generated concept illustrations are
not evidence for profiles, bolts, materials, no-load/working-load ratings or
compliance; their unsupported annotations are not adopted. Existing cooler CAD,
PIR panels and HEA120/MT40/M10 suspension remain unchanged. See
`docs/structural-refinement.md`; the original 3A comparison remains available.

## Application and interface

CO₂ Cooler Atlas contains original application code and procedural scene construction by the project's contributors, released under the [MIT License](LICENSE), copyright 2026 S3bx0.

The controls in `components/ui/`, together with supporting UI utilities, were generated and adapted from **shadcn/ui**. Their upstream MIT copyright notice is retained in [licenses/shadcn-MIT.txt](licenses/shadcn-MIT.txt). Third-party code is not relicensed as original project work. See [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md) for the installed versions and relevant license texts.

The repository presentation was inspired by [Human Atlas](https://github.com/ashemag/human-atlas). This project's documentation is written for the cooler application; no anatomy dataset or assets are included.

The October 2026 README gallery contains new screenshots of the actual local
application, with captions distinguishing source-surface review, generated
geometry and hidden components. They are not manufacturer drawings, synthetic
concept renders or a distribution of the underlying CAD packets. The gallery
does not imply a production deployment of the private-CAD review or extend the
application's MIT license to manufacturer references. See [docs/gallery.md](docs/gallery.md).

## Equipment reference

| Field | Reference |
| --- | --- |
| Manufacturer named on the source | Kelvion |
| Equipment | CO₂ air cooler / evaporator |
| Model | CSF-632-6KB-CX38 |
| Drawing identifier | 0200700379-010.000-1 |
| Fan identification used in the viewer | Ziehl-Abegg AC-630 |

The model was reconstructed from a supplied engineering drawing and user corrections. The original PDF, page renders and private research attachments are excluded from the repository and website. The drawing remains subject to its owner's rights; this repository does not grant permission to redistribute it.

The blue textile outlet hoods reflect a user-supplied correction to the intended construction. Their mesh, inflation and collapse are procedural interpretations, without a supplied textile pattern or validated material model.

The CAD datum migration additionally uses measurements from the supplied `0200700379-010.000-1-S.glb`. The original GLB remains local and is excluded from the repository and browser build. Development-overlay screenshots in the Phase 1 report document alignment against that reference. The application's MIT license does not grant rights to the underlying manufacturer CAD geometry.

Phase 2A's optional local review additionally renders a checksum-bound subset of 11 independent original bodies: rear inlet hood, drain tray, four suspension brackets and five pipe bodies. Their original vertices, normals, indices and cavity boundaries retain the manufacturer's provenance and are not application-licensed geometry. During that stage, the subset was served only in the loopback development review and was not committed to Git or included in the production bundle. Its illustrative materials are separately owned. Pipe circuit identities and materials remain unverified; their neutral spatial grouping is not a CO₂/glycol identification. Adapted support members and the rear infill clearance remain explicitly procedural interpretations, not extracted or certified manufacturer details. See `docs/cad-phase-2a.md` for scope and source/subset checksums.

Phase 2B adds the two unchanged independent CAD front covers to that same local-only review. Their probable terminal-box function and source materials remain unverified. Their supporting bases are repositioned procedural interpretations, not geometry recovered from the fused core. At that stage, the original and derived CAD assets were excluded from Git and production; the stage's subset hash and limitations are recorded in `docs/cad-phase-2b.md`.

Kelvion, Ziehl-Abegg and related product names identify the equipment being illustrated. This is an independent project with no stated affiliation, sponsorship or endorsement by those companies. No manufacturer trademarks or reference documents are licensed under the project's MIT license.

## Interpretation and uncertainty

The optional Phase 2C roof review retains selected surfaces from the fused source
core and reconstructs missing interface surfaces. The distinction is recorded
per triangle and can be highlighted in the viewer. This is not an independently
exported manufacturer panel or a certified sheet-thickness interpretation.
At that stage, retained CAD surface data and the derived roof packet stayed local
and were excluded from Git and the production bundle. Adjacent flange/bevel clearance
adjustments are procedural illustrations. See `docs/cad-phase-2c.md`.

Phase 2D extends that distinction to separately selected left and right side
envelopes. Their original exterior patches remain unchanged; missing inner and
bottom interfaces are explicitly inferred. Old procedural diagonal stiffeners,
representative side fasteners and conjectural pipe holes are removed rather than
relabelled as source features. Neither side is a certified manufacturer panel or
sheet-thickness model. During Phase 2D, the pair packet remained local and excluded
from Git and production. See `docs/cad-phase-2d.md` for provenance and bounded tests.

Phase 2F-B partitions selected Ziehl-Abegg fan surfaces from the fused `Solid4`
without changing their source vertices/normals. Exact source blade/external-rotor
bell surfaces are animated separately from an exact static central motor/stator
complement. In the 2F-B comparison the outer sleeve and guard remain procedural,
and source material identity is unverified. During that stage, the derived fan
packet stayed local and excluded from Git and production. See `docs/cad-phase-2f.md`.

Phase 2G conservatively adds unchanged source shroud surfaces and the separate
forward square outlet lattices. These are geometry-based surface selections from
the same fused `Solid4`, not independently exported or named manufacturer parts.
The inner wire guards remain procedural because 35,934 nearby source guard/support
faces cannot be assigned without overstating ownership or manually splitting the
source. Two zero-area source facets also remain unresolved. During Phase 2G, source
and generated packets stayed local and excluded from Git and production. See
`docs/cad-phase-2g.md`.

Phase 2H further classifies complete consecutive source-face runs as concentric
guard rings or outer radial ribs. It preserves 27,839 unchanged source triangles
without clipping, while 8,095 mixed central junction/support and outer-web faces
remain unresolved. The resulting logical grille is not an independently exported
or certified detachable manufacturer guard, and its illustrative material is not
a source material claim. During Phase 2H, the packet remained local and excluded
from Git and production. See `docs/cad-phase-2h.md`.

Phase 2I displays all 8,095 remaining non-degenerate fixed fan junction faces as
two explicitly mixed inspection regions. Their original positions/normals are
unchanged, but this does not establish their allocation to detachable motor,
guard or shroud parts. They are hidden during explosion rather than stretched or
assigned by appearance. During Phase 2I, original and derived CAD packets remained local/ignored.
See `docs/cad-phase-2i.md`.

Phase 2J uses section medians from the separate static textile nodes to adapt the
procedural ON silhouette and nominal 1.03 m deployed length. The R326 fabric root
and measured source gap stay unchanged. Raised stitching, clips, material,
inflation, flutter and sag remain illustrative, not manufacturer sewing details,
physical cloth behavior, CFD or an attachment certification. The private textile
meshes are not exported or bundled; the optional fit was development-review only
at Phase 2J. See `docs/cad-phase-2j.md`.

Phase 2K-A is an audit only. It finds no positive-area source surfaces in the
tested exchanger interior, so generated internal fins or tubes must not be
relabeled as original manufacturer CAD. Large source boundary patches are
envelope evidence, not a physically verified flow model. Repeated end-sheet
features are capped recesses in the supplied mesh, not confirmed internal tube
circuits. Spatial candidate selections and negative-winding shells do not imply
new part, material or void-function ownership. All detailed reports and source
projections remain local/ignored; the viewer is unchanged. See
`docs/cad-phase-2k-a.md`.

Phase 2K-B reconstructs an open perforated fin pack from the existing exchanger
datums and retained illustrative tube layout. All new fin triangles are generated;
none is relabeled as original `Solid4` geometry. The 240-fin count and 1.4 mm
display thickness are inherited visual assumptions; 10 mm pitch follows the
existing product-data transcription. The 1 mm aperture expansion is a visual
clearance choice, not a manufacturer contact fit or fabrication tolerance.
The four inherited tube-pattern overlaps are not repaired or certified by this
stage. Source end-sheet candidates remain deferred, and the old generated end
proxies are removed only in the new review. Fans, textiles and older comparisons
retain their prior qualifications. See `docs/cad-phase-2k-b.md`.

Phase 2K-C corrects the generated secondary tube pattern and its fin apertures
together while preserving the primary tube geometry. The two secondary depth
shifts are visualization choices that remove cross-family mesh interference,
not recovered CAD tube paths or manufacturer dimensions. Retained radii, sweeps,
fin thickness and aperture margins remain illustrative; no fluid identity,
complete circuit continuity, thermal contact or fabrication fit is certified.
The source-ownership ledger is unchanged, source end sheets remain deferred,
and the accepted older comparison modes retain their prior interpretation.
See `docs/cad-phase-2k-c.md`.

Phase 2K-D displays 358 unchanged source exchanger/casing interface triangles
as incomplete assembled-only inspection regions. The broad end-sheet candidates
are not recovered detachable plates, and their capped recesses are not tube
routes. Both rear end bands are deferred whole because they intersect existing
procedural supports; neither source nor supports are deformed to conceal that
incompatibility. Source positions and normals are preserved, while material,
mechanical allocation and fastening remain unverified. During Phase 2K-D, the new
source packet stayed local and excluded from Git and production. See `docs/cad-phase-2k-d.md`.

Phase 2K-E moves only a generated rear transverse beam forward by 33 mm to admit
both previously deferred whole source rear bands. The 116 source triangles keep
their original positions, normals and IDs; their mechanical ownership remains
unresolved. The support dimensions/placement, overlapping frame joints and
material finish are illustrative, not manufacturer structural or fabrication
data. Source end interiors/capped recesses remain deferred and all earlier
comparison packets remain unchanged. See `docs/cad-phase-2k-e.md`.

Phase 2K-F is an audit of residual source coverage after 2K-D/E, not a new
geometry import. It reserves the accepted 474 inspection triangles without
upgrading their mechanical ownership and records the remaining capped end
features separately from the illustrative tube layout. Winding, source-edge
adjacency and spatial bins do not identify hardware, materials, fabrication
detail or a fluid circuit. Detailed source-ID maps and geometric witnesses
remain local and ignored. See `docs/cad-phase-2k-f.md`.

Phase 2K-G retains the entire eleven-triangle central source residual without
clipping or deformation. Together with the previous 266 faces it completes the
audited central selection, not a manufacturer-exported detachable divider.
Original edge and lower-fin boundary contacts remain explicit; the finite
numerical checks do not certify fabrication fit, materials, fastening or loads.
The component is assembled-only inspection geometry. During Phase 2K-G, its source
packet remained local and excluded from Git and production. See `docs/cad-phase-2k-g.md`.

Phase 2K-H adds generated operational-core end skins around the existing
illustrative tube sections and return bends. Their rectangular domain, 2 mm
display thickness, capsule apertures and clearances are reconstruction choices,
not source end-plate geometry, measured gauge or manufacturer circuit routing.
The original 485 source inspection faces stay unchanged and the 184 capped
source recesses per end stay uninstalled. The nominal 1 mm aperture margin is
distinct from realized tessellated surface clearance. See `docs/cad-phase-2k-h.md`.

The local structural-context review uses user-supplied drawings 02/03/04 and
building screenshots for arrangement: lower-chord bearing, column seats and
purlins above trusses. New profiles, crop extents, node plates, bearing seats
and fastener patterns are generated display choices. Steel and fastener
schedules do not establish their per-joint assignment. The retained HEA120,
MT40 and M10 suspension is not a verified substitution for the drawing's 2 × U140
designation, and the printed 300 kg hanger note is not a verified model capacity.
Original building references and detailed extraction remain private, not part
of the distributed application. See `docs/structural-context.md`.

Phase 2E applies three explicit provenance classes to the fused front: unchanged
source triangles, source triangles clipped to the audited front domain, and
inferred closures/interfaces. The source front does not provide the R347 mm
operating apertures used by the interactive fan system; it has only much smaller
approximately R80 mm boundary loops and source surfaces otherwise cap those
footprints. The R347 openings are therefore documented as **functional
reconstruction**, not manufacturer bore dimensions. Real source detail in the
approximately 3 mm lateral seam remains unresolved behind shallow generated
front-skin connectors; their 0.3 mm depth is illustrative, not sheet thickness.
During Phase 2E, the generated front packet and retained manufacturer surface data
remained local and excluded from Git and production. See `docs/cad-phase-2e.md`.

- The envelope, nominal fan spacing, materials and listed design data are transcribed from the reference.
- Sheet thickness, fan blade shape, concealed refrigerant and defrost routing, fasteners and disassembly motions include approximations for a readable browser model.
- The airflow path illustrates lower intake, passage through the fin pack and front discharge. Particle speed, thermal colors and textile pressure are explanatory effects, not CFD or measured operating data.
- The listed electrical motor power does not establish whether the value applies per fan or to the full assembly; the application marks this uncertainty.
- Exploded arrangements explain component relationships and are not an approved maintenance sequence.

Use the manufacturer's current documentation for engineering decisions. The viewer provides no independent verification of performance, safety, installation requirements or manufacturing tolerances.

## Fonts and dependencies

**DM Sans** and **IBM Plex Mono** are supplied through Fontsource and remain licensed under the **SIL Open Font License 1.1**. Their complete upstream copyright and license text is retained in [licenses/DM-Sans-OFL.txt](licenses/DM-Sans-OFL.txt) and [licenses/IBM-Plex-Mono-OFL.txt](licenses/IBM-Plex-Mono-OFL.txt).

React, Three.js, React Three Fiber, Drei, Zustand, Base UI, Lucide and the other dependencies retain their own licenses. Preserve applicable notices when redistributing the source or browser build; see [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).
