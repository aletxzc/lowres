# Models are recipes of shared Effects

A Model is data, not code: an ordered list of Effects from a fixed, shared set (resolution reduction, color curve, noise, grain, vignette, light leak, JPEG compression, date stamp), each with its settings. We chose this so that adding a Model means writing a recipe instead of graphics code, which lowers the bar for contributors, and so that the planned iOS app can reimplement the Effect set once and reuse every Model unchanged.

## Considered Options

- **One hand-written shader per Model**: more freedom for each look, but every Model would have to be ported separately to every platform, and contributing a Model would require graphics programming.

## Consequences

A look that the existing Effects can't express needs a new Effect, implemented on every platform, rather than one-off code inside a single Model.
