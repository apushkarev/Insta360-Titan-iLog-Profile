# Insta360 Titan iLog Profile
This repo contains custom made log profile for specified camera

Version 0.3.8

### Hardware notes:
- created with [CMP Digital Target Studio Edition](https://www.cmp-color.fr/eng%20digital%20target.html)
- light source used is Aputure Amaran 60x S (set to 5000K) with a modified softbox
- camera WB set to 5000K

### Lut notes:
- using Rec 2020 to interpret data in footage is an educated guess. Insta360 does not specify what color space and gamma is used for iLog, so after checking different options I settled on Rec 2020 and gamma 2.4
- insta360 i-Log is not a true log, since it's tone curve is S-shaped
- this lut does color conversion only, it does not apply S curve (I hope users can do it themself)
- output image looks just flat and needs contrast adjustments

### How to for DaVinci Resolve:
- set first node color space to Rec 2020, gamma to 2.4
- apply lut in this node
- use CST for conversions to working color space

Your feedback is welcome, I'm limited in source footages for extensive testing
