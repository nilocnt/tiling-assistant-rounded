# Tiling Assistant + Rounded Corners

This package combines Tiling Assistant v55 with the current Rounded Window
Corners Reborn effect.

The rounded-corner effect is enabled and disabled together with the tiling
extension. Window resize notifications refresh the shader after tiling and
untiling, so there is no second custom shader implementation competing with
the tiling code.

Before enabling this package:

- Disable the standalone `Tiling Assistant` extension.
- Disable the standalone `Rounded Window Corners Reborn` extension.
- Keep the Agnus Shell v64 rounded-corners and tiling modules removed.

The existing Rounded Window Corners preferences are preserved through the
`org.gnome.shell.extensions.rounded-window-corners-reborn` settings schema.
The combined package exposes the Tiling Assistant preferences page.

The bundled shader also fixes the upstream `bounds[4]` indexing error in the
maximum-radius calculation.
