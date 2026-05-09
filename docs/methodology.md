# Methodology

Canonical product page: <https://justlay.me/grey-mirror/methodology>

This repository publishes a high-level public methodology summary for Grey Mirror. It intentionally does not include private model code, production prompts, proprietary classifiers, customer uploads, internal configuration, or training data.

## Method Overview

Grey Mirror analyzes exported relationship-message histories as full threads rather than isolated excerpts. The pipeline is designed to preserve conversation order, participant roles, and timing context before producing metrics or narrative summaries.

## Pipeline Stages

1. The user selects a relationship route such as romantic, platonic, or family.
2. The user uploads an exported message history.
3. The system parses and normalizes messages into a consistent internal shape.
4. Participant resolution maps sender labels to the people in the thread.
5. The timeline is segmented into windows so change can be measured.
6. Relationship metrics are calculated from the normalized thread.
7. Evidence references are attached where the product has enough support.
8. Confidence language is used to avoid overstating weak or missing evidence.
9. A report/dashboard is generated for the user.

## Route-Aware Interpretation

The relationship route changes the interpretive lens. A romantic thread, friendship thread, and family thread can use the same normalized text representation, but the meaning of silence, repair, obligation, planning, and emotional labor may differ by route.

## Evidence Philosophy

Grey Mirror should connect claims to measurable signals. A metric is stronger when it can point to:

- The relevant time window.
- The participant behavior being counted.
- The comparison baseline.
- The supporting evidence window.
- The confidence or limitation label.

## Boundaries

Grey Mirror cannot know everything that happened outside the text thread. It cannot diagnose people, replace therapy, provide emergency guidance, or prove private intent. Missing messages, deleted exchanges, sarcasm, screenshots without context, and off-platform events can change the interpretation.
