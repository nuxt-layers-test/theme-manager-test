# Plan

> **In short:** complete and validate the shared application test foundation before creating capability-specific test repositories.

## Current

- Validate the common Theme Manager-integrated dashboard and collapsible sidebar on desktop and mobile.
- Verify homepage navigation and existing Theme Manager routes operate in the same application.
- Confirm keyboard navigation, focus visibility and reduced-motion behaviour.

## Next

- Formalise extensible capability navigation and acceptance-scenario registration, after the shared shell is validated.
- Complete the shared template, then create `nuxt-layers-test/theme-manager-test` from it.
- Preserve a known-good Theme Manager dependency revision in the lockfile.

## Theme Manager acceptance

Initial scenarios:

1. Load the application independently in test mode.
2. Display and navigate the theme library.
3. Create a theme from an available template.
4. Edit and save theme definitions.
5. Select and apply a theme.
6. Delete eligible themes.
7. Verify semantic colours, typography and effects.
8. Verify system, light and dark appearance modes.
9. Verify theme storage and selection persistence.
10. Verify behaviour following application restart.
11. Verify branding, navigation and responsive layout.

Acceptance must not require IAM, an external database
or Docker. Capability implementation remains in
`nuxt-layers/theme-manager`.
