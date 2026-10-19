# Design Direction

## Experience
- Premium, calm, contemporary wellness interface; avoid a generic template or overly decorative “AI-generated” look.
- Clear information hierarchy, restrained motion, meaningful whitespace, and legible typography.
- Use 3D only for moments where it improves understanding or delight; provide lightweight/static fallbacks.

## Accessibility and localization
- English and Hindi layouts must both be designed and tested.
- Avoid text baked into images.
- Allow for longer translations, scalable text, screen readers, adequate contrast, and large touch targets.
- Use culturally respectful language and avoid presenting traditional concepts as medical certainty.

## Core navigation candidate
- Home / आज का दिन
- Food / आहार
- Routine / दिनचर्या
- Learn / ज्ञान
- Profile / मेरी जानकारी

Validate navigation with user journeys before implementation.

## States to design
- Loading, empty, error, offline, stale content, permission denied, uncertain assessment result, unavailable translation, and unavailable weather.
- Every recommendation should explain why it is shown and where its information came from.
