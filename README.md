# Vinci World Pixel Art

Team skill for creating and editing Vinci World illustrations with the approved chunky pixel style, recurring characters and complete brand logo.

## Install

From your project folder, clone this repository into its skills directory:

```sh
mkdir -p .agents/skills
git clone https://github.com/pphc-harry/vinci-world-pixel-art.git .agents/skills/vinci-world-pixel-art
```

This is a private repository. Your GitHub account must have repository access before cloning or downloading it. The owner can grant access in GitHub Settings → Collaborators. If Git is unavailable, download the repository ZIP, extract it and place the folder at `.agents/skills/vinci-world-pixel-art` in your project. Do not overwrite an existing installation without checking local edits.

Start a new agent session in the project so it can discover the skill. For other agents, load `SKILL.md` and attach the referenced images using that agent's supported workflow.

## Use

```text
Use $vinci-world-pixel-art to create 5 Vinci World festival images.
Use varied camera angles, chunky pixels and no extra copy.
```

Requires an agent with image viewing and image generation/editing that accepts reference images. This repo supplies instructions and assets, not an image model, API credentials or generation credits. Availability and output dimensions depend on the image tool.

The skill loads the approved rainy-tram style reference, character reference and full logo. The default logo appears at bottom right at about 26% visible canvas width, including “INCUBATED BY renaiss”. “No text” excludes extra copy; an explicit “no logo” request overrides the logo default.

## Included

- `SKILL.md`: workflow, style constraints, editing and quality checks.
- `agents/openai.yaml`: skill display metadata.
- `assets/`: approved style, characters, full transparent logo and two scene contact sheets.
- `references/prompt.md`: prompt backbone and optional modules.
- `references/sources.md`: portable asset roles and provenance.
- `references/asset-manifest.json`: asset dimensions and SHA-256 hashes.

The contact sheets contain 50 scene concepts; individual full-resolution scene files are not bundled. Generated concepts are not official game screenshots or verified product claims. Brand assets are provided for authorized Vinci World team work; no open-source or third-party redistribution license is granted by this repository.

## Update

```sh
git -C .agents/skills/vinci-world-pixel-art pull --ff-only
```

Check and preserve your local edits before updating.
