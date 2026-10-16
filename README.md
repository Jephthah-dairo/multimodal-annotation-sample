# Multimodal Annotation Sample

> Portfolio demonstration only. All records below are synthetic examples. This repository contains no real people, private media, client data, or employer work.

This sample outlines a consistent approach to labeling image, video, and audio content for machine-learning datasets. The examples use text descriptions instead of media files.

## Example annotations

| ID | Modality | Synthetic content description | Labels | Notes |
| --- | --- | --- | --- | --- |
| IMG-001 | Image | A red ball resting on short grass. | object: ball; color: red; setting: outdoors | Label only visible attributes. |
| VID-001 | Video | A person opens a door and walks into a room. | action: opening door; action: entering room | Record timestamps when working from actual footage; do not infer identity. |
| AUD-001 | Audio | One speaker says, “Turn left at the next street.” | speech: present; speakers: 1; transcript: provided sentence | Mark unclear words as uncertain instead of guessing. |

## Suggested annotation fields

- `sample_id`: stable ID for the record
- `modality`: image, video, or audio
- `description`: concise, observable content description
- `labels`: controlled tags for objects, actions, or events
- `timestamp`: required for time-based video or audio events when available
- `confidence`: annotator confidence using a project-defined scale
- `notes`: ambiguity, missing context, or guideline questions

## Quality checks

1. Follow the project label definitions and examples consistently.
2. Describe what is observable; avoid guessing identity, intent, or context.
3. Check video events at the required frame or timestamp granularity.
4. Replay unclear audio and preserve uncertainty in the transcript.
5. Review labels for omissions, duplicates, and inconsistent naming.
6. Escalate ambiguous cases instead of silently forcing a label.

## Scope

These examples illustrate a documentation and quality-review approach. They are not a real annotation dataset and make no claim about production accuracy or volume.
