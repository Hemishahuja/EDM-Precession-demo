# Electron Electric Dipole Moment (eEDM) Visualization

This interactive visualization demonstrates the behavior of an electron in the presence of electric and magnetic fields, with a focus on detecting the electron's electric dipole moment (EDM).

## Overview

The visualization shows how an electron's spin precesses in magnetic and electric fields. In the Standard Model of particle physics, the electron's EDM is predicted to be extremely small and currently unmeasurable. However, many extensions to the Standard Model predict larger EDM values that could be detected with sufficiently sensitive experiments.

The key signature of an electron EDM is a change in the precession rate when the electric field is reversed. This visualization demonstrates this effect.

## Features

- **Interactive Controls**: Toggle magnetic field, electric field, and EDM on/off
- **Field Reversal**: Flip the electric field direction to observe precession rate changes
- **Real-time Visualization**: See the electron spin precession in real-time
- **Precession Cones**: Visualize the precession cones for both magnetic moment and EDM
- **Rate Display**: Shows the current precession rate in radians per second

## How to Use

1. Open `eedm7.html` in a web browser
2. Use the control buttons to:
   - **Apply B-field**: Turn on the magnetic field to initiate Larmor precession
   - **Apply E-field**: Apply an electric field (only affects precession if EDM is enabled)
   - **Flip E-field**: Reverse the direction of the electric field
   - **Toggle EDM**: Enable/disable the electron's electric dipole moment
   - **Pause/Resume**: Pause or resume the animation
   - **Reset**: Reset all fields and clear the visualization

## Physics Explanation

### Larmor Precession
When an electron is placed in a magnetic field (B), its magnetic moment (μ) precesses around the field direction at the Larmor frequency:
ω_L = -γB

Where γ is the gyromagnetic ratio.

### EDM Effect
If an electron has an electric dipole moment (d), it will interact with an electric field (E) and contribute an additional precession term:
ω_EDM = ηE

Where η is a coupling constant. The key signature of the EDM is that this term changes sign when the electric field is reversed.

### Combined Precession
With both fields present and an EDM:
ω_total = -γB + ηE

When the electric field is flipped (E → -E):
ω_flipped = -γB - ηE

The difference between these rates (2ηE) is the EDM signature.

## Visualization Elements

- **Red Vector**: Electron's magnetic moment (μ)
- **Yellow Vector**: Electron's electric dipole moment (d) - only visible when EDM is enabled
- **Blue Arrow**: Magnetic field (B) - always vertical
- **Purple Arrow**: Electric field (E) - can be flipped
- **Red Cone**: Precession cone for magnetic moment
- **Yellow Cone**: Precession cone for EDM (when enabled)
- **White Trace**: Path of the spin tip over time

## Educational Value

This visualization helps understand:
1. How particle spins behave in electromagnetic fields
2. The concept of Larmor precession
3. How EDM searches work in particle physics experiments
4. Why field reversal is crucial in EDM measurements

## Implementation Details

- Pure HTML/CSS/JavaScript - no external dependencies
- Uses HTML5 Canvas for rendering
- Responsive design that works on most modern browsers
- Physics parameters are scaled for clear visualization

## Files in this Repository

- `eedm7.html`: Main visualization file
- `README.md`: This file
- `implementation_plan.md`: Development plan for future enhancements
- `electron_edm_precession.gif`: Animated demonstration
- Video files: Source recordings of the animation

## Future Enhancements

See `implementation_plan.md` for planned features including a time-based precession rate visualization.

## License

This project is open source and available under the MIT License.
