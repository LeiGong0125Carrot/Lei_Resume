# Job-specific resumes (LaTeX / Overleaf)

This repository keeps the original resume sources unchanged and stores separate, **editable LaTeX** resumes for individual job applications.

## Master resume
- `Lei_Resume_Ortet.tex` — source template and reference for the 2026 job-specific versions.
- `Lei_Resume.tex` and other original sources have not been overwritten.

## Tailored applications
- `applications/2026-10-27/{Company}_{Role}_resume/main.tex` — one self-contained LaTeX source per job.
- `applications/2026-10-27/{Company}_{Role}_resume/job.json` — job requirements, fit/gaps, salary when known, official application URL, and status.
- `tracking/jobs_2026-10-27.csv` — daily review tracker.

## Open any version in Overleaf
1. Open the desired job folder under `applications/2026-10-27/`.
2. Download its `main.tex` file. The template uses standard TeX Live/Overleaf packages.
3. In Overleaf choose **New Project → Blank Project**, then upload `main.tex` to the project root (replacing its default file). Set `main.tex` as the main document.
4. Compile using **pdfLaTeX**; inspect the PDF and edit the LaTeX source before applying.

Alternatively, download the job folder as a ZIP and choose **New Project → Upload Project**, with `main.tex` as the root/main file. If the ZIP contains parent directories, adjust the main document path or repackage the contents of the selected job folder.

## PDFs and quality status
20/20 LaTeX resumes in the 2026-10-27 batch compiled to one-page PDFs in GitHub Actions. The generated PDFs can be downloaded as the `tailored-resumes-2026-10-27` artifact at:
https://github.com/LeiGong0125Carrot/Lei_Resume/actions/runs/40545098627

Compiled PDFs are build artifacts, not necessarily committed to this repository. Visual and factual review is still required.

## Important
- These are drafts for human review, **not submitted applications**.
- Position requirements and application URLs may change. Always re-check the employer's live posting.
- Do not interpret work under a coauthored project as solely the user's contribution.
- The repository currently is public. Review whether personal contact details and application history should be stored in a private repository.
