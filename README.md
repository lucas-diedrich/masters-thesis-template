# README
Latex template for master's thesis/short dissertations.


## Directory structure
main.tex <br>
├── bibliography <br>
├── figures <br>
├── .github <br>
│   └── workflows <br>
├── sections <br>
└── submitted-version <br>


- `main.tex` - Run pdflatex/miketex on this file. It will include all subsections, the front matter, abstract, acknowledgments, table of contents/list of figures/list of tables, and the bibliography. You can add/remove sections by adding/removing `.tex` files in the `./sections` directory. 


- `./sections`
It is recommended that all content is added to the respective `.tex` files in this subdirectory. **If you reference figures/import data, the paths are relative to the `main.tex` file.** 

- `./bibliography/`
Add an arbitrary number of `.bib` files. Per default, `biblatex` will try to import a `bibliography.bib` file from this directory. 

- `./figures`/
Add figures here (potentially in subdirectories). Can be included in the subsections with paths relative to the `main.tex` file. 

- `./submitted-version` 
For reproducibility etc. it is recommended to store the final .pdf file or important checkpoints in another directory.

- `.github`
Implements a GitHub workflow so that by going to `> Actions > LaTeX Compile/Build > Run Workflow` builds and compiles `.tex` document via a GitHub Actions Runner to a downloadable `.pdf` artifact. The name can be customized while starting the workflow. 


## Contributing 
Feel free to raise [issues](https://github.com/lucas-diedrich/masters-thesis-template/issues) or add pull requests to improve this template! 
