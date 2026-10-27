# Lei Gong — Job-specific LaTeX resumes

One GitHub repository and **one Overleaf project** can hold all job-specific resumes. Each company/role has **one independent `.tex` file**, rather than its own project or subfolder.

## Files
- `main.tex` — Overleaf default entrypoint that selects which resume to preview.
- `resumes/{Company}_{Role}_resume.tex` — 20 independent, complete, pdfLaTeX-compilable resume sources. All stored together in **one directory**.
- `Lei_Resume_Ortet.tex` — unchanged original/master resume.
- `tracking/jobs_2026-10-27.csv` — list of employers, roles, required qualifications, missing qualifications, salary, application URLs, and review status.
- `tracking/job_details/{Company}_{Role}_resume.json` — expanded job metadata.
- `tracking/archived_original_main.tex` — saved copy of the previous blank `main.tex`.

## One Overleaf project: selecting a resume
1. Import or sync this **entire repository** to a single Overleaf project, or upload the source ZIP once.
2. Set the root `main.tex` as **Main document** and select **pdfLaTeX**.
3. To compile a particular company's version, edit **only the \input path** in root `main.tex`:
   ```tex
   \input{resumes/Dandelion_Health_NLP_LLM_Data_Scientist_resume.tex}
   ```
   Change the path to any other `resumes/*_resume.tex` file and recompile.
4. You can also use Overleaf's **Set as Main File** feature on a particular standalone `.tex` file instead of editing `main.tex`.

This repository structure does **not** resolve Overleaf's `GitAPI Error` if the underlying issue is OAuth authorization or the Git integration itself. You can import a source ZIP into Overleaf as an alternative.

## Workflow
The GitHub Actions workflow `.github/workflows/build-tailored-resumes.yml` independently compiles all `resumes/*_resume.tex` files and uploads PDFs as one artifact. These drafts are **not submitted job applications**. Review all facts and employer criteria before applying.

## Privacy
The repository is currently public and includes contact details and job preferences. Consider making it private in GitHub Settings.
