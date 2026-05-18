# 🐉 Chinese Dragon Automaton

Final project for 3D Printing — a hand-cranked mechanical automaton that brings a
Chinese dragon to life through a system of phase-offset cams. The dragon's body
is segmented into ten individually moving parts that rise and fall sequentially,
creating the iconic undulating wave motion of the Chinese dragon in flight.

---

## 🎯 How It Works

A horizontal **camshaft** runs through the housing, fitted with ten eccentric cam
profiles, each rotated to a different angle relative to the others (phase-offset).
A **gear-driven hand crank** transfers rotation from the user to this shaft, with
a small gear reduction that slows the motion down for smoother, more controlled
operation.

As the shaft turns, each cam pushes a **vertical follower rod** up and down.
Because the cams are offset in phase, the followers rise and fall at slightly
different moments — producing a **wave of vertical motion** that travels from
one end of the housing to the other.

Each follower is connected to one of the **ten body segments of the dragon**, so
the wave is transferred directly to the dragon's body. The result is a fluid,
undulating motion that travels from head to tail — the characteristic movement
of the Chinese dragon in traditional parades and folklore.

The faster the user cranks, the more dynamic the wave becomes, evoking the
dragon "flying" through clouds.

---

## 📐 Dimensions

Overall footprint of the assembled automaton: approximately **120 × 40 × 80 mm**
(length × width × height).

| Measurement | Value |
|---|---|
| Housing length | ~120 mm |
| Housing width | ~40 mm |
| Total height (with dragon) | ~80 mm |
| Main shaft diameter | ~5 mm |
| Number of cams | 10 |
| Number of body segments | 10 |

---

## 🧩 Components

The project mirrors the structure of the reference dolphin automaton, with all
mechanism parts reused and only the body segments redesigned. Each component
exists as both a Fusion 360 source file (`.f3d`) and an exported mesh (`.stl`)
for printing.

### Mechanism parts (reused from reference)

| File | Quantity printed | Role |
|---|---|---|
| `Housing_frame.f3d / .stl` | 1 | Housing — outer frame with side windows, supports the shaft and follower guides |
| `Housing_top.f3d / .stl` | 1 | Housing — top cover with ten vertical slots for the follower rods |
| `Camshaft.f3d / .stl` | 1 | Main camshaft — horizontal axle with all ten phase-offset cam profiles integrated as a single printed piece |
| `Camshaft_endcap.f3d / .stl` | 1 | Small cylindrical end cap with a square hole that slides onto the far end of the camshaft, acting as a retainer to keep the shaft seated in the housing |
| `Gear_small.f3d / .stl` | 1 | Small driven gear (~14 teeth) with a square hole; mounted on the gear-end of the camshaft and meshes with `Crank_handle` to receive rotation from the user |
| `Crank_handle.f3d / .stl` | 1 | Large drive gear with an integrated cylindrical grip — the user-facing input element; meshes with `Gear_small` to drive the camshaft |
| `Crank_pivot.f3d / .stl` | 1 | Small auxiliary part of the crank assembly with a cylindrical base and square top; functions as the pivot/axle around which `Crank_handle` rotates within the housing |
| `Follower_rod.f3d / .stl` | 10 | Vertical follower rod that sits on top of a cam and transfers motion to a body segment |

### Body parts (new design for the dragon)

| File | Quantity printed | Role |
|---|---|---|
| `dragon_p1.f3d / .stl` | 1 | Dragon head — with horns, eyes, whiskers, and traditional Chinese features |
| `dragon_p2.f3d / .stl` | 1 | Body segment 2 — first segment behind the head |
| `dragon_p3.f3d / .stl` | 1 | Body segment 3 |
| `dragon_p4.f3d / .stl` | 1 | Body segment 4 |
| `dragon_p5.f3d / .stl` | 1 | Body segment 5 — central segment, longest dorsal spine |
| `dragon_p6.f3d / .stl` | 1 | Body segment 6 |
| `dragon_p7.f3d / .stl` | 1 | Body segment 7 |
| `dragon_p8.f3d / .stl` | 1 | Body segment 8 |
| `dragon_p9.f3d / .stl` | 1 | Body segment 9 |
| `dragon_p10.f3d / .stl` | 1 | Dragon tail — tapered, with flame or fin motif |

**Summary: 18 unique designs, 27 printed parts in total** (one each for the
mechanism components except `Follower_rod`, which is printed ten times).

---

## 🎨 Design Decisions & Personal Touches

Going beyond a direct copy of the reference dolphin automaton, the following
intentional design choices make this project original:

- **Theme**: re-interpreting the mechanism in the context of Chinese mythology.
  The dragon traditionally undulates through clouds rather than through water,
  which suits the wave motion of the mechanism perfectly.
- **Body segmentation**: the dragon is split into ten segments along its length,
  matching the structure of the reference dolphin but reshaped into a serpentine
  dragon body with distinct head and tail.
- **Decorative features per segment**: dorsal spines, scaled texture, and a
  central segment with a longer ornamental spine, all referencing traditional
  Chinese dragon iconography.
- **Stylized housing**: the housing is given a Chinese-pavilion aesthetic
  (curved roof line, ornamental side windows shaped as round "coin" motifs).
- **Embossed iconography**: the Chinese character for dragon (龍) is embossed on
  the front of the housing in place of the original "DOLPHIN" lettering.
- **Color palette**: the dragon is hand-painted post-print in red and gold
  acrylic — the traditional colors of celebration and good fortune in Chinese
  culture.
- **Decorative cloud base**: a thin printed base with stylized clouds replaces
  the original wave decoration, supporting the "flying dragon" theme.

---

## 🛠️ Assembly Notes

- The `Camshaft` is printed as a single piece with all ten cam profiles
  integrated. No assembly of individual cams is required.
- Alternatively, the shaft can be replaced with a straight metal rod (Ø 5 mm)
  for reduced friction and improved rotation — in this case the cam profiles
  are printed separately and slid onto the rod at the correct phase angles
  (36° apart for ten cams evenly distributed across one full rotation).
- `Gear_small` slides onto the square section at one end of the `Camshaft`,
  while `Camshaft_endcap` slides onto the square section at the opposite end
  to retain the shaft in place within the housing.
- The ten `Follower_rod` parts rest freely on top of the camshaft. Gravity holds
  them in contact with the cam surface during operation.
- Each dragon segment attaches to its corresponding follower through a friction
  fit (a small cylindrical socket in the underside of the segment receives the
  flat top of the follower). No glue is required.
- `Crank_handle` rotates around the `Crank_pivot`, which is mounted in the side
  wall of the housing. The teeth of `Crank_handle` mesh with `Gear_small` to
  drive the camshaft.
- The two housing halves (`Housing_frame` and `Housing_top`) snap together over
  the assembled mechanism.
- Estimated assembly time: 15–20 minutes once all 27 parts are printed and
  cleaned.

---

## 🚧 Project Status

🟡 **In development** — the repository will be updated throughout the project with:

- [ ] All `.f3d` source files
- [ ] All `.stl` files ready for slicing
- [ ] Photos of the modeling process in Fusion 360
- [ ] Photos and timelapse of the printing process
- [ ] Final demonstration video showing the wave motion
- [ ] Motion study GIF
- [ ] Complete documentation and lessons learned

---

## 📚 References & Inspiration

- Reference automaton: swimming-dolphin cam-driven kinetic sculpture, GrabCAD
  Library (<https://grabcad.com/library/swimming-dolphin-1>)
- Mechanical principles: cam–follower transmission and phase-offset shafts
  (see *507 Mechanical Movements*, Chapter VI)
- Cultural references: traditional Chinese dragon iconography in folk parades,
  temple architecture, and Year of the Dragon celebrations
