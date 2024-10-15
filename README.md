# Personal Curriculum Vitae in LaTeX

This repository contains the LaTeX source code for my personal Curriculum Vitae (CV). The purpose of this project is to maintain a version-controlled configuration of my CV.

## Repository Structure

- `main.tex`: The main file of the CV, located in the root directory. This file includes the necessary sections from the `sections` folder and compiles the full CV.
- `sections/`: This folder contains all the individual sections and subsections of the CV, organized into separate files for modular editing and compilation. Below is a list of the files inside this folder:
    - `0_contact_info.tex`: Contains personal contact information.
    - `1_experience.tex`: Describes professional experience.
    - `2_education.tex`: Provides an overview of education.
    - `2a_education_courses.tex`: Lists the relevant courses completed.
    - `2b_education_conferences.tex`: Details the conferences attended.
    - `3_skills.tex`: Summarizes key skills.
    - `3a_skills_technical.tex`: Describes technical skills.
    - `3b_skills_competencies.tex`: Lists competencies and soft skills.
    - `4_academic_publications.tex`: Includes a list of academic publications.
    - `5_presentations_recognitions.tex`: Contains presentations and recognitions.
    - `5a_presentations.tex`: Lists the presentations given.
    - `5b_competitions.tex`: Details the competitions participated in.
    - `5c_recognitions.tex`: Describes recognitions received.
    - `6_personal_projects.tex`: Describes personal projects worked on.
    - `7_languages.tex`: Lists the languages spoken.
    - `8_additional_information.tex`: Includes any additional relevant information.

## Configuring the Language

To change the language of the generated CV, modify the following line in `main.tex`:
```latex

\newcommand{\idioma}{english} % Options: 'espanol', 'english'
```
- Set `\idioma` to `english` for an English version.
- Set `\idioma` to `espanol` for a Spanish version.

## Precompiled PDFs

For convenience, precompiled versions of the CV in both English and Spanish are provided in the root directory. Although it's not ideal to keep binary files in version control, in this case, they are provided for ease of access:
- `cv_english.pdf`
- `cv_espanol.pdf`

## Branches

The `main` branch of this repository contains the general version of the CV. Additionally, separate branches exist for specific roles, allowing for easy adaptation of the CV depending on the target position:
- `role-management`: Tailored CV for management roles.
- `role-technical`: Tailored CV for technical roles.

## How to Compile

To compile the LaTeX source code, the following programs must be installed:
- `pdflatex`
- `latexmk`
- Other LaTeX packages specified in `main.tex`

Alternatively, the CV can be compiled online using Overleaf: [Overleaf](https://www.overleaf.com/)

To compile locally, simply run the following command:

```bash
pdflatex main.tex
```

This will generate a PDF version of the CV based on the sections included and the language configuration.