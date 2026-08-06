# Boltz Colab Notebook

[Open In Colab]

An interactive, easy-to-use Google Colab notebook for running the **Boltz** biomolecular prediction model. 

Inspired by the highly accessible AlphaFold2/ColabFold notebooks, this tool is designed to generate and analyze biomolecular structures without dealing with complex local setups, dependencies, or advanced coding.


## Key Features

- **Interactive UI Forms:** Seamlessly configure your job names, output directories, and parameters directly through Colab's UI fields—no code editing required.
  
- **Automated Environment Setup:** Built-in commands to clean temporary directories (`~/.boltz/`) ensuring conflict-free, reproducible runs every time.
  
- **Integrated 3D Visualization:** Analyze your predicted structures right in the browser. Features include:
  - Color mapping by confidence scores (pLDDT).
  - Toggle options to display side chains.
  - PAE (Predicted Aligned Error) and PDE plots natively displayed.
    
- **Zero Local Hardware Required:** Run complex biomolecular predictions using Google Colab's cloud GPUs.


## How to Use

1. **Open the Notebook:** Click the "Open in Colab" badge at the top of this README.
2. **Connect to a Runtime:** Ensure you are connected to a GPU runtime in Colab (`Runtime` > `Change runtime type` > Hardware accelerator: `GPU`).
3. **Upload Sequence:** First, upload a `.yaml` file containing your target protein sequence to the Colab environment (using the folder icon on the left sidebar).
4. **Input Parameters:** When prompted by the UI forms, enter your desired job name (e.g., `prot_xxxx.yaml` matching your uploaded file) and output directory.
5. **Run the Cells:** Execute the cells sequentially (or use `Runtime` > `Run all`).
6. **Visualize:** Scroll down to the visualization cells to inspect your generated structures and PAE/PDE plots.


## Acknowledgments

- The original creators and researchers behind the **Boltz** model. Please visit and support the official [Boltz GitHub Repository](https://github.com/jwohlwend/boltz).

- The **ColabFold** team for inspiring the user-friendly UI/UX approach for bioinformatics tools in Google Colab.


@article{passaro2025boltz2,
  author = {Passaro, Saro and Corso, Gabriele and Wohlwend, Jeremy and Reveiz, Mateo and Thaler, Stephan and Somnath, Vignesh Ram and Getz, Noah and Portnoi, Tally and Roy, Julien and Stark, Hannes and Kwabi-Addo, David and Beaini, Dominique and Jaakkola, Tommi and Barzilay, Regina},
  title = {Boltz-2: Towards Accurate and Efficient Binding Affinity Prediction},
  year = {2025},
  doi = {10.1101/2025.06.14.659707},
  journal = {bioRxiv}
}

@article{wohlwend2024boltz1,
  author = {Wohlwend, Jeremy and Corso, Gabriele and Passaro, Saro and Getz, Noah and Reveiz, Mateo and Leidal, Ken and Swiderski, Wojtek and Atkinson, Liam and Portnoi, Tally and Chinn, Itamar and Silterra, Jacob and Jaakkola, Tommi and Barzilay, Regina},
  title = {Boltz-1: Democratizing Biomolecular Interaction Modeling},
  year = {2024},
  doi = {10.1101/2024.11.19.624167},
  journal = {bioRxiv}
}

@article{mirdita2022colabfold,
  title={ColabFold: making protein folding accessible to all},
  author={Mirdita, Milot and Sch{\"u}tze, Konstantin and Moriwaki, Yoshitaka and Heo, Lim and Ovchinnikov, Sergey and Steinegger, Martin},
  journal={Nature methods},
  year={2022},
}
