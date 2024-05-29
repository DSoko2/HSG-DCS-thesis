# A Thesis Template used by an HSG-DCS Student

This is a content-removed version of my dissertation from the DCS program at the University of St. Gallen (HSG), which ideally helps fellow and future HSG PhD students compile their thesis. Please do whatever you want with it. I started from [Gian-Luca Savino's](https://www.gianlucasavino.com/) thesis (thanks for sharing!), who started from a [template by Krishna Kumar for theses at Cambridge](https://github.com/kks32/PhDThesisLyX/) (thanks Krishna!). However, like Gian-Luca, I adapted the template very goal-driven, adding and changing what I needed and wanted and breaking some stuff that I deemed not to need. So, please do not expect the template to be fully functional or idiomatic :)

The template implements the [HSG printing regulations for doctoral theses](https://universitaetstgallen.sharepoint.com/sites/phdoffice/Freigegebene%20Dokumente/Druck%20und%20Publikation/6Printing%20Regulations%20EN.pdf?web=1) and is opinionated on the freedom the regulations provide.

The main file is [thesis.tex](./thesis.tex). [thesis-info.tex](./thesis-info.tex) is the central place for the metadata, from which the cover, spine, etc. get the information. [definitions.tex](./definitions.tex) contains all kinds of definitions, including the list of bibtex source files to read.

## Submission and Publication

Submission and publication are not the same. You will be assessed after submission. Once you are accepted, you may (have to) make some (minor) changes. Then you publish.

For submission, you technically do not have to comply with the printing regulations (yet). For submission, you have to provide a "Statutory Declaration" and potentially also a "Declaration of Auxiliary Aids." Note that the [Statutory Declaration](overhead/statutory-declaration) is a text HSG provides (this is the up-to-date version from January 2024). The [Declaration of Auxiliary Aids](./overhead/auxiliary-aids) is something I came up with after looking a bit at other theses. It may be completely off or unnecessary; however, the current regulations in January 2024 were quite weird and driven by ChatGPT/AI worries at the University, and I never received any feedback regarding this version, which I submitted (no feedback means neither good nor bad feedback – so I guess it was fine). [example-submission.pdf](./example-submission.pdf) is an example of my thesis in the configuration I submitted (however, content-wise, it is identical to the published version).

For publication, you *do not* have to include the statutory declaration and the declaration of auxiliary aids, as the PhD office responded to me via mail on May 28, 2024. However, you must include the preisdent sign at the beginning, and a CV. [example-publication.pdf](./example-publication.pdf) is the final, published version of my thesis.

## PDF-A Compliance

The publication PDF must be PDF-A-compliant, which requires a little bit of care. I used verapdf to check whether my PDF complies (cf. [check-pdf-a.sh](./check-pdf-a.sh)). The template and everything I did in it technically compiles to a PDF-A-compliant PDF. If you have issues, consider that an embedded PDF (e.g., an included PDF graphic) may be the culprit. Converting non-PDF-A graphics into PDF-A-compliant ones with weird tools did the trick for me...

## Printing Procedure

You can print with whatever company you want. The HSG PhD office recommended to me on May 7, 2024, [Copy Blitz AG](https://www.copy-blitz.ch/) and Niedermann Druck AG. I went with Copy Blitz because I knew them, they are next to OLMA, and they are super friendly people with great service. They also know the publication procedure with HSG. This is a brief trace of the interaction I had:

1. May 29, 2024: Provided Copy Blitz my thesis PDF (compiled from [thesis.tex](./thesis.tex)) and the spine (compiled from [spine.tex](spine.tex)) to be printed as DIN-A5 HSG-compliant dissertation. (The Uni wants you to submit 7 copies; if you want some yourself, ask for more copies...)
2. May 29, 2024: Copy Blitz contacted the PhD office with the print PDF, asking for the'Gut zum Druck' (ready for printing).
3. May 30, 2024: Copy Blitz asked me via mail to confirm their draft of the outside cover sheet (front and back with spine).
4. May 30, 2024: The PhD office confirmed the 'Gut zum Druck' with small requests for changes, which Copy Blitz forwarded to me. I performed the tweaks (all of them are applied to this repo, of course) and sent the new PDF to Copy Blitz. Even though it was not required, Copy Blitz forwarded the new version to the PhD office for confirmation.
5. May 31, 2024: Copy Blitz received the confirmation of the new version and started printing.
   * This is the point where you can submit the final PDF as digital version in Compass (Requests -> Eletronic submission of doctoral thesis).
6. June 3, 2024: Copy Blitz informed me that they printed the theses. I picked them up and submitted 7 of them at the PhD office in person. (If you are not available, Copy Blitz can also mail them.)

## License

The copyright of [./example-submission.pdf](./example-submission.pdf), [./example-publication.pdf](./example-publication.pdf), and [./graphics/example.pdf](./graphics/example.pdf) is retained by the author, Daniel Sokolowski. The use, adaption, and re-distribution of these files are only permitted with explicit consent from the author. All other contents in this repository are licensed under the [MIT license](https://choosealicense.com/licenses/mit/). They can be freely used, adapted, and redistributed.