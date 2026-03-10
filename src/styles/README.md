# Styles Source Structure

This folder is the Phase 1 SCSS source architecture.

Order of inclusion from `main.scss`:
1. `00-tokens.scss`
2. `01-base.scss`
3. `02-utilities.scss`
4. `03-layout.scss`
5. `components/*`
6. `course/*`

Guidelines:
- Keep token variables, maps, mixins, and functions in `00-tokens.scss`.
- Keep global element defaults in `01-base.scss`.
- Keep reusable helper classes in `02-utilities.scss`.
- Keep structural layout patterns in `03-layout.scss`.
- Keep semantic component styles in `components/`.
- Keep legacy and module-specific compatibility in `course/`.
