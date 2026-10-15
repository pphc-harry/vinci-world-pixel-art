# Prompt backbone

Use with actual attached reference images, not text alone. Name each input's role. For edits, replace the scene request with the user's edit and preservation constraints.

```text
Create a Vinci World pixel-art scene.

REFERENCE ROLES
style-approved.png (latest raw rainy tram) is the strict rendering anchor: match its visibly chunky square clusters, stepped silhouettes, thick dark outlines, simplified surfaces, readable chibi faces, and low-detail finish.
characters-original.png is the identity reference only. Preserve the selected characters' recognizable headwear, hair, clothing identifiers and companion markings. Do not copy poster text, logo, black padding, full cast or layout.
vinci-full-logo.png is the required brand asset for every final image. Preserve the complete supplied VINCI WORLD mark and its INCUBATED BY renaiss line; do not redraw, retype, pixelate or substitute this asset. The character poster is not the logo source.
Any additional environment reference supplies setting and props only; redraw it at the approved chunky pixel quality.

RENDERING
Build characters and environments from broad, deliberate pixel clusters. Keep hair, hands, faces, clothes, stone, wood and foliage at a coherent coarse visual scale. Use a few solid shade clusters per material. Match the approved reference's balance of clear expression and raw pixel simplicity. Prioritize large calm shapes and coarse rendering over decorative polish. Do not add detail when changing scene or colour grading. The reference contains slight tonal softness; avoid expanding it into rendered lighting. Use a bright adventure-game colour language with strong dark contours and controlled warm/cool contrast.
No smooth illustration, 3D shading, hair strands, woodgrain microtexture, fabric noise, fine ornamental detail, bloom, soft-focus painting or dense particles. Do not invent a fixed native grid or palette count.

SCENE MODULE
Selected characters: [0–2 by default, or the requested cast]
One clear action: [action]
Expression per character: [readable expression]
Visible expression cues: [eyes, eyebrows, mouth and supporting gesture; preserve existing emotion for a style-only edit]
Visual story beat: [one specific incident or prop interaction, not a generic pose]
Setting and 3–5 large environmental elements: [setting and props]
Camera and framing: [specific camera angle]
Camera purpose: [how this viewpoint reveals the action; vary viewpoint and crop across a batch]
Composition/aspect: [requested aspect, otherwise landscape 16:9]

BRAND PLACEMENT
Include the complete supplied logo once in the bottom-right corner, preserving its aspect ratio and transparency. Measure the visible logo after excluding transparent outer padding: approximately 26% of canvas width (435 x 172 px on a 1672 x 941 canvas), with approximately 14 px right and bottom margins at that canvas size; scale margins for other sizes. Keep this area clear of faces, hands, cards and the main action. Preserve an existing correct logo without adding a duplicate. For edits, preserve the original scene lighting and composition. A no-text brief excludes additional copy, not this required logo; an explicit user request to omit or change the logo overrides the corresponding default.

No unwanted duplicate characters, extra limbs or fused hands. Apart from the required supplied full logo, no readable text, pseudo-text, other logos, watermark or UI unless explicitly requested. Cards show simple artwork or geometric colour shapes. Do not automatically introduce fairness/proof themes.
```

## Conditional modules

For card-pull briefs, add:

```text
CARD-PULL MOMENT
Stage: [opening / peeking / reveal / duplicate recognition / sorting / sleeving]
Card or pack position and hand interaction: [simple, physically readable]
Character reaction or visual joke: [specific to this incident]
Keep the cards and faces readable at thumbnail size. Avoid repeating the same glowing rare-card reveal. Depict a fictional scene without invented product odds, prices or guaranteed rewards.
```

For edits, replace the new-scene module with:

```text
EDIT CONTRACT
Target image: [actual source image]
Change only: [requested change]
Preserve: [identity, expression unless requested, pose, props, composition, lighting and aspect as applicable]
For a requested smile: use a readable small upturned pixel mouth and relaxed eyes/eyebrows; preserve open/closed eyes unless the brief says otherwise.
For a coarser redraw: enlarge deliberate clusters and simplify materials/background detail without changing the scene's emotion or action. Do not blur the image or introduce fine polish.
```

例子：草帽紅髮收藏家同綠帽冒險者喺木橋中段交換卡片，一個得戚、一個驚訝；卡片高度側面近鏡，背景只有橋柱、河流、遠方浮島。人物圖決定身份，最新雨夜電車標準圖決定像素粗幼；木橋係新場景，唔係宣稱現有遊戲關卡。
