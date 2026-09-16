# From tennis video to explainable form

The goal is to start from ordinary video—especially professional footage—recover one stroke in a body-local frame, and turn it into a free-camera teaching animation inspired by [Learn Table Tennis](https://learntabletennis.com/academy/3d-viewer-demo/).

Research prototype. No standalone public demo is currently available.

## Research position

- Modern monocular methods make any-video pose recovery a reasonable starting point, but tennis benchmarks still show unreliable depth and foot contact.
- Bath motion capture is a validation ruler, not the product input: it tests whether known metric motion and racket geometry survive the pipeline.
- The first deliverable is one honest, body-local teaching stroke with measured, inferred, and authored quantities clearly separated—not an athlete-specific digital twin or a full rally simulation.

## Current evidence

- **Rejected:** a smooth orbitable broadcast reconstruction that failed its geometry gate: 48.33 px median reprojection error, 2.36 m position error, and 108.1° orientation error.
- **Retained:** a fixed-camera Alcaraz review with 61/61 inspected joint frames, 54/61 visible or uncertainty-labelled racket silhouettes, and a 2.20 px median 2D ball-fit residual over eight reviewed observations.
- **Next test:** recover one short professional stroke with a current monocular model, validate the same pipeline on known 3D, then require a held-out camera before claiming accurate any-angle form.

The research distinguishes the product goal from its benchmarks; the results above do not establish a usable video-to-animation product.
