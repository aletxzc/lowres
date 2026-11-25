# Lowres

An app that turns the phone's camera into retro cameras: handheld consoles, early digicams, film and instant cameras. Each one makes photos look the way that kind of device would have.

## Language

### Models and their look

**Model**:
A fictional retro camera the app emulates, inspired by (but never named after) a real device. It is made of an ordered list of Effects, each with its own settings, and it determines how a Photo comes out.
_Avoid_: Camera, filter, preset, profile, skin

**Effect**:
One building block of a Model's look, such as grain, vignette, a color curve or a date stamp. There is a fixed set of Effects shared by all Models.
_Avoid_: Filter, pass, stage, layer, step

### Shooting

**Photo**:
The finished image a Model produces when the user shoots. Only the finished image exists: no unprocessed original is kept, so a Photo can never be switched to another Model.
_Avoid_: Picture, image, capture, snapshot

**Viewfinder**:
The live view of what the Device camera sees, shown through the selected Model before shooting. It matches the Photo except for compression artifacts, which only appear when shooting.
_Avoid_: Preview, camera view, live feed

**Device camera**:
The physical camera of the phone or computer running the app.
_Avoid_: Camera (on its own), lens, sensor

**Facing**:
Which side of the device the Device camera points to: front or back.
_Avoid_: Orientation (that means portrait vs landscape), selfie mode
