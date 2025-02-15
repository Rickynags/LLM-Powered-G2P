# LLM-Powered Grapheme-to-Phoneme Conversion

This repository contains the code for the paper **"LLM-Powered Grapheme-to-Phoneme Conversion: Benchmark and Case Study"**.
Grapheme-to-phoneme (G2P) conversion is a critical component of speech processing systems, especially for applications like text-to-speech (TTS). This paper evaluates the potential of large language models (LLMs) in G2P tasks, introducing novel prompting and post-processing techniques that enhance LLM outputs without additional training or labeled data. 

![methods](https://github.com/user-attachments/assets/ca4f2cc9-5989-44fc-9213-8bc01c97a9f0)

We also present:
- **Sentence-Bench**: The first sentence-level benchmarking dataset for G2P in Persian.
- **Kaamel-Dict**: The largest open-licensed G2P Persian dictionary.

Our results demonstrate that LLM-based G2P systems can outperform traditional tools, especially in handling homographs and context-sensitive phonemes, highlighting their potential for underrepresented languages like Persian.

## Additional Results

After publishing the paper, we conducted further experiments on two additional models: **GPT-4o** and **O1-Preview**. Below is the full table of results from the paper, now including these two additional models as new columns in bold.

| **Metric**               | **llama-3.1**<br>405b-instruct | **gemma2**<br>9b-it | **mixtral**<br>8x7b | **qwen-2**<br>7b-instruct | **mistral**<br>7b-instruct | **gpt-3.5**<br>turbo-instruct | **gpt-4o**<br>mini | **gpt-4** | **claude-3.5**<br>sonnet | **GPT-4o** | **O1-Preview** |
|--------------------------|-------------------------------|---------------------|---------------------|--------------------------|---------------------------|-------------------------------|-------------------|-----------|--------------------------|------------|----------------|
| **PER (\%) ↓**           | 8.30                          | 21.58               | 26.84               | 59.06                    | 34.68                     | 11.76                         | 10.44             | 8.28      | 5.80                 | **6.43**   | **9.75**       |
| **Homograph Acc. (\%) ↑** | 54.00                         | 21.50               | 15.00               | 3.50                     | 12.50                     | 40.50                         | 45.00             | 48.50     | 78.50                | **64.00**  | **64.50**      |
| **Ezafe F1 (\%) ↑**      | 88.33                         | 61.21               | 44.05               | 27.99                    | 38.93                     | 73.04                         | 70.34             | 87.26     | 93.03                | **89.86**  | **85.15**      |

## Code
The code for the experiments and tools described in the paper is provided in this repository and is accessible in this [colab link](https://colab.research.google.com/drive/1FgWUGkMjnnM4w9jUpZSRuwQlGnqXAhEW?usp=sharing).


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
