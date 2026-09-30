# TB2S — Train–Bridge–2 Spans

**A MATLAB desktop application for rapid dynamic screening of continuous two-span railway bridges under moving loads.**

Developed at the **Universitat Politècnica de València (UPV), Spain**, by **Carlos Riascos, Willan Cueva, and Pedro Museros**, within the InBridge4EU project.

[Download releases](https://github.com/carlosriascosUPV/TB2S_desktop/releases) · [Report an issue](https://github.com/carlosriascosUPV/TB2S_desktop/issues) · [Contact the authors](mailto:criascos@upv.es)

## Overview

TB2S implements a simplified Residual Influence Line (LIR) approach for continuous railway bridges with two equal spans. It combines an analytical formulation for the first vertical bending mode with a numerical reference surface for the second mode. Modal contributions can be combined using SRSS or CQC.

The application supports preliminary assessment and parametric studies by identifying train–bridge combinations that may require more detailed analysis.

## Main features

* Automatic or manual input of bridge parameters.
* PT60 and HSLM-A train models, with options to define custom trains.
* Displacement and acceleration response envelopes.
* Accumulated response envelopes for increasing train speed.
* Separate results for the first mode, second mode, and combined response.
* Two-dimensional and three-dimensional response maps over bridge length and train speed.
* Selection of a bridge length to inspect its response curves.
* Bottom Limit thresholds for filtering the displayed results.
* Save and open analysis configurations, and export results to Excel or HTML.

## Download

1. Open the repository's [Releases page](https://github.com/carlosriascosUPV/TB2S_desktop/releases).
2. Select the required release and download its Windows application ZIP from **Assets**.
3. Extract the entire ZIP to a local folder before running the installer or application.

Choose the application ZIP uploaded by the authors. GitHub's automatically generated **Source code (zip)** download is a repository snapshot and may not contain the executable.

## System requirements

* Windows compatible with the supplied executable and its MATLAB Runtime release.
* The **MATLAB Runtime release that matches the MATLAB release used to compile the application**, at the same update level or newer within that release.
* Internet access during installation if the installer downloads MATLAB Runtime.

**A paid MATLAB licence is not required to run the compiled application.** MATLAB Runtime is freely available from MathWorks.

Consult the MATLAB-generated `readme.txt` supplied with the release for the exact Runtime requirement. For example, an application compiled with MATLAB R2024b requires MATLAB Runtime R2024b (24.2); a different, newer MATLAB release is not a substitute.

[Download MATLAB Runtime](https://www.mathworks.com/products/compiler/matlab-runtime.html)

## Installation

Use the instructions that match the package downloaded from the release.

### Package with an installer

1. Extract the complete ZIP.
2. Run the supplied installer, whose filename may include `Installer` or `\_web`.
3. Follow the installation wizard. If the installer offers to install or download MATLAB Runtime, allow it to complete this step.
4. If the installer does not include Runtime installation, install the matching Runtime separately using the requirement in `readme.txt`.
5. Launch TB2S from the shortcut created by the installer or from the installation folder.

### Package with the application executable only

1. Read the supplied MATLAB-generated `readme.txt` and install the matching MATLAB Runtime.
2. Extract the complete package and preserve its folder structure.
3. Run the application executable, normally `TB2S.exe`.

Keep any supplied data files, images, libraries, and support folders in their original locations. Do not move the executable out of its application folder or run it directly from inside the ZIP.

## Quick start

1. Choose **Bridge Response** to inspect a selected bridge or **Response Maps** to explore a range of bridge lengths.
2. Set the bridge length or length range and the other bridge parameters. Use automatic input or enter the available values manually.
3. Select the train model and the trains to analyse. Check the train-speed range.
4. Select acceleration or displacement and choose **SRSS** or **CQC** for modal combination.
5. Click **Run Analysis**.
6. Inspect the individual modal contributions and their combined response. In Response Maps, use the length selector to inspect the curves for a particular bridge.
7. Use accumulated responses, 2D/3D views, and Bottom Limit thresholds as needed. Export the results to Excel or HTML.

Check the units displayed beside each input. When changing analysis inputs, run the analysis again whenever the application indicates that recalculation is required.

## Scope and limitations

The present formulation considers symmetric, prismatic continuous beam bridges with two equal spans under prescribed moving loads. It represents the response using the first two vertical bending modes.

Use the results within these assumptions. TB2S provides a simplified screening model; detailed assessment may require additional modes, a refined bridge model, or time-domain analysis. The accuracy of modal combination depends on the train–bridge configuration.

## How to cite

If you use TB2S in research, teaching materials, reports, or presentations, please cite the software and the associated methodological contribution.

### Software

> Riascos, C., Cueva, W., \& Museros, P. (2026). \*TB2S: Train–Bridge–2 Spans\* \[Computer software]. Universitat Politècnica de València. https://github.com/carlosriascosUPV/TB2S\_desktop

For reproducibility, also state the **release tag or version used** and link to that specific release.

```bibtex
@misc{Riascos2026TB2S,
  author       = {Riascos, Carlos and Cueva, Willan and Museros, Pedro},
  title        = {{TB2S}: Train--Bridge--2 Spans},
  year         = {2026},
  howpublished = {Computer software, Universitat Polit\\`ecnica de Val\\`encia},
  url          = {https://github.com/carlosriascosUPV/TB2S\_desktop}
}
```

### Methodological contribution

> Riascos, C., Cueva, W., \& Museros, P. (2026). \*Screening analysis of continuous beams under moving loads by residual influence line methods: A MATLAB toolbox implementation\*. Conference contribution, EURODYN 2026, Hannover, Germany.

## Authors and contact

**Carlos Riascos, Willan Cueva, and Pedro Museros**  
Universitat Politècnica de València (UPV), Spain

Contact: [criascos@upv.es](mailto:criascos@upv.es)

When reporting a problem, include the TB2S release, Windows version, MATLAB Runtime release and update, the complete error message, and the bridge and train settings needed to reproduce it.

## Troubleshooting

|Problem|What to check|
|-|-|
|MATLAB Runtime is missing or incompatible|Install the release specified in the MATLAB-generated `readme.txt`, at the required update level or newer within that release.|
|A `.mat` file, image, or other resource cannot be found|Extract the complete ZIP and preserve all support folders. If the error remains, report it to the authors so the application package can be corrected.|
|Results do not reflect modified inputs|Check whether the application requests recalculation and run the analysis again.|
|An export cannot be saved|Choose a folder where your Windows account has write permission.|

## Acknowledgements

This work was developed within **InBridge4EU**, funded by **Europe's Rail Joint Undertaking** under the **Horizon Europe** research and innovation programme, **Grant Agreement No. 101121765** (HORIZON-ERJU-2022-ExplR-02).

Views and opinions expressed are those of the authors only and do not necessarily reflect those of the European Union or Europe's Rail Joint Undertaking. Neither the European Union nor the granting authority can be held responsible for them.

## Installation reference

[MathWorks documentation on MATLAB Runtime compatibility](https://www.mathworks.com/help/compiler/about-the-matlab-runtime.html)

