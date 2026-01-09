# TubeTest Tracker Transfer Archive

This repository is a lightweight archive of the assets that were provided for the TubeTest Tracker handoff. It currently contains the raw uploads that were supplied (several `.docx` documents with instructions and a large `video_details` CSV export). No application source code lives here.

## Contents
- `Prompt ultime Script.docx` and `Prompt ultime Script Prépa.docx`: documentation provided during the handoff.
- `ListeInstructionsPourPrompt.docx`: additional written instructions.
- `video_details - 2023-07-31T174006.771.csv`: exported video metadata.

## Usage notes
- Treat the files in this repository as reference material only; they may contain sensitive operational details that should not be redistributed.
- If you need to extract text from the `.docx` files, convert them locally (for example with `pandoc` or LibreOffice) rather than editing the originals in place.
- Avoid committing secrets or environment values. If credentials are discovered in the documents, move them to a secure secrets store and redact them from version control.
- Should application code be added later, consider creating a fresh Next.js/Firebase project directory (`/home/ubuntu/app`) rather than mixing it with these artifacts.

## Next steps
1. Review the documents for any sensitive information and ensure it is managed securely.
2. Decide whether to keep this repository solely for documentation or migrate the relevant guidance into the actual application repository.
3. If the CSV is needed for analytics, import it into your preferred data tooling and add a short data dictionary in this repository.
