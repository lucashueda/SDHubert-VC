# Soft-Discrete Hubert representations for Voice Conversion

This repository is based on official ([github:Soft-VC](https://github.com/bshall/soft-vc)) repository. Here I'm just putting all together and trying new things.

## TODO's

- [X] Aggregate all repositories in one ([hubert](https://github.com/bshall/hubert), [acoustic-model](https://github.com/bshall/acoustic-model) and [hifigan](https://github.com/bshall/hifigan))
- [X] Fix acoustic model checkpoint saving (related to: [acoustic-model:pull request](https://github.com/bshall/acoustic-model/pull/8))
- [ ] Docker image for reproducibility

## Experiments plans

- [ ] Option to extract 22kHz melspectrograms to better quality
- [ ] Option to change the mel dim (default is 128, in TTS is commonly used 80 as default)
- [ ] Non-autoregressive acoustic-model (fastpitch or fastspeech2)
  - [ ] Changing prosody information to be extracted from reference and not predicted (pitch and energy)
- [ ] Direct link between soft-hubert and hifigan, excluding acoustic-model dependency (based on discussion: [acoustic-model:issue](https://github.com/bshall/acoustic-model/issues/6))
  - [ ] Option to augment with pitch countour   
  - [ ] Option to augment with multi-speaker embeddings

## References and credits

- [Hubert code](https://github.com/bshall/hubert)
- [Acoustic model code](https://github.com/bshall/acoustic-model)
- [Hifigan code](https://github.com/bshall/hifigan))
