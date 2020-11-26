<details>
<summary>Click here to see the changelog of Omega 1.21 (beta)</summary>

* [1.21.0] New: Real-time clock
* [1.21.0] Change: Chrome Popup: workshop.numworks.com to getomega.dev
* [1.21.0] Change: Doxygen with an Omega theme
* [1.21.0] Change: Merge omega-themes submodule in the main repository

</details>

### Omega 1.20 `LATEST RELEASE`

* [1.20.0] Update: Updated to Epsilon 14.4.1!
* [1.20.0] New: Added 67 constants
* [1.20.0] New: New units
* [1.20.0] New: 3DS Simulator
* [1.20.0] New: External apps are displayed on the Home Screen
* [1.20.0] New: Python: `open` method (and derivatives)
* [1.20.0] New: Physics constants are now using the Epsilon units
* [1.20.0] New: Added message when the compilation starts
* [1.20.0] New: Undef is hidden during symbolic calculation
* [1.20.0] New: Display the scripts size
* [1.20.0] New: Community themes: Download a community theme with `THEME_REPO=git-url` and `THEME_NAME=theme_name`.
* ~~[1.20.0] New: Compact display mode enabled by default~~ Compact display now available on Epsilon
* [1.20.0] New: Shift + Home is now a shortcut to go to calculation (or the first app)
* [1.20.0] New: Support for RGB files without alpha channel.
* [1.20.0] New: Add root and log settings
* [1.20.0] New: `\` shortcut (with <kbd>ALPHA</kbd> + <kbd>x10^x</kbd>), `@` shortcut (with <kbd>ALPHA</kbd> + <kbd>ANS</kbd>), `µ` and `Ω`
* [1.20.0] New: Docker!
* [1.20.0] New: Web simulator background
* [1.20.0] Change: Result display setting is now displayed in "Math settings"
* [1.20.0] Change: Simulators are renamed (Epsilon -> Omega)
* [1.20.0] Fix: <kbd>ALPHA lock</kbd> + <kbd>arrow</kbd>
* [1.20.1] Fix crash on append on new file
* [1.20.1] Change color of fractal in `mandelbrot.py`
* [1.20.1] Python `os` module (`uname`, `listdir`, `remove`, `rename`)
* [1.20.2] New: Document os
* [1.20.2] Change: Clean useless files in os
* [1.20.2] New: `\ @ Ω µ` on the simulator keys
* [1.20.2] New: Persistent Simulator storage
* [1.20.3] Change: Constants based on the CODATA 2018
* [1.20.3] Change: Visual keyboard only change state on keydown
* [1.20.3] Change: `USERNAME` to `OMEGA_USERNAME`

---

### Omega 1.19.x
* [1.19.0] Update: Updated to Epsilon 13 (bêta)!
* [1.19.0] New: Omega Icons!
* ~~[1.19.0] New: Option for font size for Python (will be soon reverted, since Epsilon decided to implement it too)~~ Done on Epsilon
* [1.19.0] New: Hungarian language!
* [1.19.0] New: Compact display in the calculation app
* [1.19.0] New: In the Python app, there is a new option to duplicate a script
* [1.19.0] New: Red, purple and orange color choices for the LED
* [1.19.0] New: Url to install apps + infos about External available in the app
* ~~[1.19.0] New: In the Python app, <kbd>shift</kbd> + <kbd>up</kbd> leads to the beginning of the script and <kbd>shift</kbd> + <kbd>down</kbd> allows you to jump to the end.~~ Not working. Fixed in 1.19.1
* [1.19.0] New: RAM usage in the settings
* [1.19.0] New: External is removed of n0100 and the web simulator.
* [1.19.0] New: Code-side system to check if an app is available in a specific exam mode (`NoExaminationLevel`, `BasicExaminationLevel` and `StrictExaminationLevel`)
* [1.19.0] New: Beta testers added in the contributors list
* [1.19.0] Change: Removed static buffers
* [1.19.0] Change: The exam mode icon is now better positioned.
* [1.19.0] Fixed: With `get_keys()` 2 keys were inverted (right and up)
* [1.19.0] Fixed: The input field of the RPN app now reflects the style of the calculation app
* [1.19.0] Fixed: Apps dependency in ion
* [1.19.0] Fixed: The sign of *10^
* [1.19.0] Fixed: Remove static buffers
* [1.19.0] Fixed: "Activate exam mode" button stayed highlighted
* [1.19.0] Fixed: The Onboarding logo is now better
* [1.19.0] Fixed: <kbd>Shift</kbd> + <kbd>÷</kbd> displays `%` instead of nothing
* [1.19.0] Fixed: In French, the description of "monotonic function" is fixed
* ~~[1.19.0] Fixed: Some problems with alpha(lock)+backspace~~ Feature done on Epsilon
* [1.19.1] Update: Epsilon updated (especially `Allow interruption of infinite print loops`)
* [1.19.1] Change: Free 1776 bytes of heap
* [1.19.1] Change: Disable the LED choice
* [1.19.1] Change: In the Python app, <kbd>alpha</kbd> + <kbd>up</kbd> leads to the beginning of the script and <kbd>alpha</kbd> + <kbd>down</kbd> allows you to jump to the end. Same for <kbd>alpha</kbd> + <kbd>left</kbd> and <kbd>alpha</kbd> + <kbd>right</kbd>. Before, it was with the <kbd>shift</kbd> key, but it's now used to select the text.
* [1.19.1] Fixed: Some problems with the Compact Display
* [1.19.1] Fixed: Some Hungarian translations
* [1.19.1] Fixed: Crash while compiling the official software
* [1.19.1] Fixed: Allow simulator to be loaded with multiple scripts
* [1.19.2] Update: Epsilon (especially `Fix input(), that did not return the input` and `matplotlib`)
* [1.19.2] Fixed: Some problems with the Compact Display

---

### Omega 1.18.x
* [1.18.0] New: Theming engine with a Dark Theme of Omega 😱 Usage: `OMEGA_THEME=name_of_the_theme`
* [1.18.0] New: MicroPython version is now displayed in the settings
* [1.18.0] New: <kbd>shift</kbd> + <kbd>+/-</kbd> increase/decrease the brightness
* [1.18.0] New: <kbd>shift</kbd> + <kbd>(</kbd> writes `()`
* [1.18.0] New: Exam mode: you can now choose between 3 modes: "standard", "no symbolic" and "Dutch"
* [1.18.0] New: Symbolic calculation indicator displayed in the toolbar
* ~~[1.18.0] New: Keep backspace operation in alpha lock mode~~ Done on Epsilon
* [1.18.0] New: External app (v2) ; allows you to install GIAC and Nofrendo from https://zardam.github.io/nw-external-apps/
* [1.18.0] New: Various improvements to the build system
* [1.18.0] New: The contributors usernames (@...) are now displayed
* [1.18.0] New: Doxygen added (to document the source code)
* [1.18.0] Change: Convert symbol_controller into preferences_controller
* [1.18.0] Change: Reorganized storage
* [1.18.0] Fix: Some labels are fixed in the settings. They were too long
* [1.18.0] Fix: Background of the exam mode logo was wrong
* [1.18.1] Fix: External is now disabled in NoSym exam mode, to disable KhiCAS.
* [1.18.2] Fix: All contributors were not shown
* [1.18.2] Removed: Telemetry in the android app
* [1.18.2] New: Omega icon in the android app
* [1.18.2] Change: changed app id in the android app
* [1.18.3] Fix: <kbd>shift</kbd> + <kbd>-</kbd> no longer writes `\\`
* [1.18.4] Fix: Crash with e^(i*pi) or cos(0)
* [1.18.5] New: Red LED in exam mode

---

### From 1.0.x to 1.17.x

* [1.0.0] New: Symbolic Calculation
* [1.0.0] New: Lava OS version in settings > about
* [1.1.0] New: Blue Led in exam mode. Now, teachers can know when a student uses LavaOS
* [1.2.0] New: 'Lava OS' instead of 'APPLICATIONS' at the top of the home screen
* [1.3.0] New: Increase Brightness steps (from 5 to 16)
* [1.4.0] New: Chemistry constants sorted by atomic number or in alphabetical order (120 molar masses!)
* [1.5.0] New: Change Led color in settings (white/green/blue/yellow)
* [1.6.0] New: Lava OS version tag (public/dev) in settings > about
* [1.7.0] New: Lava OS Contributors in settings
* [1.8.0] Change: Lava OS becomes Omega!
* [1.8.1] New: Update contributors
* [1.8.2] Fix: German translations
* [1.9.0] New: Epsilon updated to 12.0.0
* [1.9.1] Fix: Chemical constants duplication (code side)
* [1.10.0] New RPN app!
* [1.10.1] New: Update contributors
* [1.10.2] Fix: Contributors duplication (code side)
* ~~[1.10.3] New: 32 KB Python heap instead of a 16 KB~~ Done on Epsilon
* [1.10.4] Fix: Child display in settings
* [1.11.0] New: Physics constants
* [1.12.0] New: A new periodic table app
* [1.12.1] New: get_keys() on Python!
* [1.12.2] Fix: Warnings during compilation
* [1.12.3] New: Update contributors
* [1.13.0] New: Accessibility settings
* [1.13.1] New: Accessibility translations
* [1.13.2] New: Module time in toolbox
* [1.13.3] New: Add command-line arguments support
* [1.13.4] New: Add username in the settings
* [1.13.5] New: Remove username row if N/A
* [1.13.6] Fix: Spaces in username
* [1.13.7] Fix: Multiplication symbols in toolbox
* [1.13.8] New: Atom app updated
* [1.13.9] New: 3 new constants (physics)
* [1.13.10] Fix: Workshop crash!
* [1.14.0] New: Massive refactor of settings
* [1.15.0] New: You can now compile the simulator
* [1.15.1] New: Updated Atom
* [1.15.2] New: Make binpack target work, changed logo
* [1.15.3] New: Updated Atom
* [1.15.4] New: Updated Epsilon
* [1.15.5] New: Updated Epsilon
* [1.15.6] New: Reordered settings
* [1.16.0] New: Add the ability to change the multiplication sign
* [1.16.1] Fix: Hardware test shortcut position in the settings
* [1.16.2] Fix: Math options > Result format crash
* [1.17.0] New: User-friendly settings for the multiplication sign
* [1.17.0] New: RPN app fixed
* [1.17.0] New: The palette is now larger to allow very customizable themes
* [1.17.0] New: Omega Light theme (installed by default)
* [1.17.1] Fix: Fixed an issue with the multiplication symbol
* [1.17.2] Fix: Fixed colors of the exam mode popup
