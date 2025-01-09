# LLM-Powered Grapheme-to-Phoneme Conversion

This repository contains the code for the paper **"LLM-Powered Grapheme-to-Phoneme Conversion: Benchmark and Case Study"**.
Grapheme-to-phoneme (G2P) conversion is a critical component of speech processing systems, especially for applications like text-to-speech (TTS). This paper evaluates the potential of large language models (LLMs) in G2P tasks, introducing novel prompting and post-processing techniques that enhance LLM outputs without additional training or labeled data. 

![methods](https://github.com/user-attachments/assets/ca4f2cc9-5989-44fc-9213-8bc01c97a9f0)

We also present:
- **Sentence-Bench**: The first sentence-level benchmarking dataset for G2P in Persian.
- **Kaamel-Dict**: The largest open-licensed G2P Persian dictionary.

Our results demonstrate that LLM-based G2P systems can outperform traditional tools, especially in handling homographs and context-sensitive phonemes, highlighting their potential for underrepresented languages like Persian.

## Code
The code for the experiments and tools described in the paper is provided in this repository. 


## Additional Resources
- **[Sentence-Bench](https://huggingface.co/datasets/MahtaFetrat/SentenceBench)**: Benchmarking dataset for sentence-level G2P evaluation in Persian.
- **[Kaamel-Dict](https://huggingface.co/datasets/MahtaFetrat/KaamelDict)**: Open-source Persian G2P dictionary with over 120,000 entries.

## Paper and Citation (TO BE UPDATED)
You can access the paper [here](https://arxiv.org/abs/2409.08554). If you use this work, please cite it as follows:

```
@article{qharabagh2024llm,
  title={LLM-Powered Grapheme-to-Phoneme Conversion: Benchmark and Case Study},
  author={Qharabagh, Mahta Fetrat and Dehghanian, Zahra and Rabiee, Hamid R},
  journal={arXiv preprint arXiv:2409.08554},
  year={2024}
}
```

## License
The code in this repository is licensed under the MIT License. The datasets associated with this work are licensed under the GNU General Public License (GPL), as they incorporate data from GNU-licensed dictionaries.
