# duchadeau_project
Brainhack-school 2024 repository of Romain DUCHADEAU

This project aims to develop an algorithm to detect sleep states using fMRI data thanks to machine learning algorithm.

## Who am I ?
<a href="https://github.com/romainDCHD ">
   <img src="https://avatars.githubusercontent.com/romainDCHD?v=4?s=100" width="100px;" alt=""/>
   <br /><sub><b>Romain DUCHADEAU</b></sub>
</a>

I am a microelectronics engineering student at Polytechnique Montréal who wishes to specialize in biomedical

## Setup Instructions

### Step 1: Create a Virtual Environment

Create a virtual environment to install the necessary libraries in an isolated environment:

```
python -m venv fmri_env
```

### Step 2: Activate the Virtual Environment

Activate the virtual environment:

- **Windows:**
  ```bash
  .\fmri_env\Scripts\activate
  ```

- **MacOS/Linux:**
  ```bash
  source fmri_env/bin/activate
  ```
### Step 3: Download FSL
Download flsinstaller.py on [this](https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/FslInstallation) site

### Step 4: Install FSL
Install FSL by tapping:
```
pip install flsinstaller.py
```

### Step 4: Install Required Libraries
Run the following command to install the libraries:
```
pip install -r requirements.txt
```
**Well done it's finish**. The last step is to dowload the dataset used on [openneuro](https://openneuro.org/datasets/ds003768/versions/1.0.11)

## File description

- **Main.ipynb** : the main jupyter notebook with all the workflow
- **Draft_Exploration_datase.ipynb** and **Draft_preprocessinf.ipynb** :  Two draft used to test ideas. Not supposed to be explored but cans be helpfull.
- **requirement.txt** : See the installation module 

## Dataset Description

This dataset includes simultaneous EEG and BOLD signal recordings from 33 healthy participants, collected at Penn State University with their informed consent.

### Dataset Contents

#### Participants
- 33 healthy participants.

#### Recording Sessions
- Anatomical sessions for structural imaging.
- Two 10-minute resting-state sessions.
- Multiple 15-minute sleep sessions.
- The first resting session was conducted before a visuomotor adaptation task (Albouy et al., Journal of Sleep Research, 2013) and the second after the task.

#### Sleep Stage Data
- Sleep stages for these 33 subjects are organized in the 'sourcedata' folder.
- Each TSV file contains sleep stages for every 30-second interval across different sessions for each subject.
- Notations include: "w" for wake, "1" for NREM1, "2" for NREM2, "3" for NREM3, "uncertain" for uncertain periods, and "unscorable" for periods with too much artifact to be reliably scored.

#### Magnetic Resonance Imaging (MRI)
- Data collected on a Siemens Prisma Fit 3 Tesla scanner using a 20-channel Siemens receive coil.
- Anatomical images acquired with an MPRAGE sequence (TR: 2300 ms, TE: 2.28 ms, isotropic spatial resolution of 1 mm, FOV: 256 mm, flip angle: 8 degrees, matrix size: 256×256×192, acceleration factor: 2).
- BOLD fMRI data acquired with an EPI sequence (TR: 2100 ms, TE: 25 ms, slice thickness: 4 mm, 35 slices, FOV: 240 mm, in-plane resolution: 3 mm×3 mm).

#### EEG Data
- Collected with a 32-channel MRI-compatible EEG system from Brain Products, Germany.
- Electrodes placed according to the international 10-20 system.
- Recorded eye activity (EOG) and cardiac signal (ECG).
- EEG data collected at a sampling rate of 5000 Hz with a bandpass filter of 0-250 Hz.
- R128 in EEG signals corresponds to the BOLD fMRI volume trigger.
- S1 markers in EEG during sleep sessions indicate the participant's wakefulness state. S2 and S3 markers represent no button press and can be ignored.

### Dataset Application

This dataset is ideal for developing algorithms to detect whether a participant is in a state of sleep or wakefulness using EEG and fMRI recordings. You can use the annotated sleep stages to train a machine learning model capable of distinguishing between sleep and wake states.

For more information or questions about this dataset, please refer to the articles mentioned in the "References and Links" section of the dataset or contact Dr. Yameng Gu (ymgu95@gmail.com).

  