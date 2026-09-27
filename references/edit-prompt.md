# 单张编辑提示词

替换方括号为实际观察。核实输入编号，只保留一个配色分支及适用的高光分支，不把占位符送入工具。

```text
Use case: style-transfer. Produce one independent finished image.

INPUT ROLES
Input 1 is the only source of subject, scene and composition: [actual photo].
Input 2 is the bundled water print, used for texture and treatment of existing specular highlights only.
Inputs [actual indices] are supporting style references: [roles]. Never copy their objects or layouts.

CONTENT LOCK
Preserve [identity, count, pose, camera angle, proportions, position, specific markings and image-side orientation, key background and framing]. Preserve the source aspect ratio and orientation, without stretching or cropping the subject. Simplify tiny photographic textures into gentle tonal forms, retaining recognition-critical details. [Important existing lettering.] No new objects, captions or signatures.

COLOR STRATEGY — retain exactly one branch
[A: The source already has compatible blue/cool tones: identify them. Match the references' nuanced cobalt/ocean/teal relationships, deep blue shadows, creamy ivory lights and restrained warm coral/olive accents where these are present in the source. Preserve the original illumination and relative color identities. No uniform blue overlay, fluorescent colors or gray washout.]
[B: The source palette is substantially different: identify its main hues and approximate visual proportions. Retain those source hues, warm/cool balance, colored shadows and subject colors. Borrow only the references' print texture, gentle tonal simplification and applicable highlight shapes. Do not inject cobalt, teal or peach into unrelated areas. Use a quiet neutral ivory support and highlight colors compatible with the original light.]

MEDIUM AND CLEANLINESS
A matte, finely grained paper print with softly simplified photographic forms. Dense but subtle random ink granules and paper pinholes, slightly varied in size and coverage, integrated into the color areas. At a 1024px viewing scale, most visible grains feel about 1–3px, not coarse snow. Maintain clean coherent color fields, comfortable color harmony and clear subject edges. Keep texture quieter on faces, eyes, markings and product details. No muddy color mixing, heavy colored noise, regular halftone grids, scratches, stains, impasto, cartoon outlines or slick vector surfaces.

HIGHLIGHTS — retain applicable directions
[Existing specular highlights at: actual locations. Preserve their distribution, direction and perspective. Render irregular discontinuous soft-white/cream glints, a few larger fragments among small flecks, subtly broken paper-print edges and minimal bloom. For palette A, allow very pale peach edging like the water reference. For palette B, adapt warmth to the source light. No starbursts, crosses, lens flares, neon halos or invented reflections.]
[Diffuse bright areas at: actual locations. Keep them coherent, with gentle light planes and fine grain; never shatter white fur, skin, clothes, walls or clouds into glitter.]
[No strong highlights: do not add sparkles, water glints or a new light source.]

FRAME
[Default: retain the overall source aspect ratio, fitting the complete composition within a quiet ivory paper margin approximately 5–8% of the short side as a visual guide; slightly irregular ink edges. No square-forcing or crop.]
[If borderless requested: full bleed, no outer paper border; keep internal paper-print texture.]

RESULT
One finished artwork, no comparison grid or mockup. Keep the source unmistakably recognizable. Prioritize a clean, comfortable image over stronger texture. Series consistency comes from print material, not forcing unrelated source palettes to become blue.
```
