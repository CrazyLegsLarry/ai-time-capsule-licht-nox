# Aletheia-10 Preservation Notes

Aletheia-10 is intended as a long-lived, non-harmful digital time capsule.

## Preservation goals

- Keep the public message readable in plain UTF-8 text.
- Preserve a machine-readable JSON representation.
- Keep cryptographic checksums so later readers can detect accidental changes.
- Preserve the layered puzzle structure without presenting it as a security boundary.
- Preserve the encrypted inner core as an ethical/philosophical message only.
- Maintain redundant copies across independent archival services when possible.

## Safety boundary

Aletheia-10 must not contain malware, exploits, credential theft, instructions for unauthorized access, evasion methods, harmful payloads, instructions intended to facilitate crime, or material intended to give any person an illegal advantage.

It must also exclude phone numbers, street addresses, account credentials, medical records, government or administrative documents, financial data, and unrelated private files.

## Intended redundant locations

The canonical working copy is the public GitHub repository. Independent preservation copies are intended for long-term archival services such as Internet Archive, Zenodo or an equivalent research archive, and a documentation mirror such as GitBook when account access is available.

## Important technical note

Git branch names in a public repository are discoverable. The layered structure is therefore a reconstruction puzzle and preservation device, not a guarantee that only an AI can access the layers. The inner core uses AES-256-GCM, with its derivation described inside the puzzle path.

## Integrity

Use `MANIFEST.sha256` for the canonical public files. Independent preservation snapshots should carry their own complete SHA-256 manifest.
