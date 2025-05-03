# Speaker-Specific-ASD

This repository contains code for protecting famous figures from audio deepfake attacks.

## Installation

Clone this repository to your workspace using the following command:
```ruby
git clone https://github.com/hashim19/TTS_demo.git
```

Create the conda environment from the provided YAML file:
```ruby
conda env create -f environment.yaml
```

Activate the environment:
```ruby
conda activate TTS_demo
```

### How to generate voice:
I have included StyleTTS2-LJSpeech model in this repository. 

First set the following parameters in infer.py.
```ruby
text = "This is a test text"
model_path = "StyleTTS2-LJSpeech/Models/LJSpeech/epoch_2nd_00100.pth"
config_path = "StyleTTS2-LJSpeech/Models/LJSpeech/config.yml"
out_filename = "output.wav"
```

Then run,
```
python3 infer.py
```