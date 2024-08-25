Here are the steps to create custom models.

Make sure you have Ollama installed and running ( no walking 😄 )
Go to huggingface website and download the model ( I have downloaded the GGUF model )
Create a modelfile and input necessary things.
Create a model out of this modelfile and run it locally in the terminal.

Now, you might be wondering what are the necessary things to input in the modelfile, I know your thinking, here it is 🤗 In this example, I am using the TheBloke/CapybaraHermes-2.5-Mistral-7B-GGUF model.

# Modelfile

FROM "./capybarahermes-2.5-mistral-7b.Q4_K_M.gguf"

PARAMETER stop "<|im_start|>"
PARAMETER stop "<|im_end|>"

TEMPLATE """
<|im_start|>system
{{ .System }}<|im_end|>
<|im_start|>user
{{ .Prompt }}<|im_end|>
<|im_start|>assistant
"""

You might also be thinking how to create and run the custom model, for that too, here it is ✌️

ollama create my-own-model -f Modelfile
ollama run my-own-model

Now, you know how to create a custom model from model hosted in Huggingface with Ollama. Give a try and good luck with it. Still, If you prefer a video walkthrough, here is the link.

#### TheBloke/CapybaraHermes-2.5-Mistral-7B-GGUF

.gitattributes
2.45 kB
GGUF model commit (made with llama.cpp commit e0085fd)
7 months ago
README.md
22.7 kB
Upload README.md
7 months ago
capybarahermes-2.5-mistral-7b.Q2_K.gguf

2.72 GB
LFS
GGUF model commit (made with llama.cpp commit e0085fd)
7 months ago
capybarahermes-2.5-mistral-7b.Q3_K_L.gguf

3.82 GB
LFS
GGUF model commit (made with llama.cpp commit e0085fd)
7 months ago
capybarahermes-2.5-mistral-7b.Q3_K_M.gguf

3.52 GB
LFS
GGUF model commit (made with llama.cpp commit e0085fd)
7 months ago
capybarahermes-2.5-mistral-7b.Q3_K_S.gguf

3.16 GB
LFS
GGUF model commit (made with llama.cpp commit e0085fd)
7 months ago
capybarahermes-2.5-mistral-7b.Q4_0.gguf

4.11 GB
LFS
GGUF model commit (made with llama.cpp commit e0085fd)
7 months ago
capybarahermes-2.5-mistral-7b.Q4_K_M.gguf

4.37 GB
LFS
GGUF model commit (made with llama.cpp commit e0085fd)
7 months ago
capybarahermes-2.5-mistral-7b.Q4_K_S.gguf

4.14 GB
LFS
GGUF model commit (made with llama.cpp commit e0085fd)
7 months ago
capybarahermes-2.5-mistral-7b.Q5_0.gguf

5 GB
LFS
GGUF model commit (made with llama.cpp commit e0085fd)
7 months ago
capybarahermes-2.5-mistral-7b.Q5_K_M.gguf

5.13 GB
LFS
GGUF model commit (made with llama.cpp commit e0085fd)
7 months ago
capybarahermes-2.5-mistral-7b.Q5_K_S.gguf

5 GB
LFS
GGUF model commit (made with llama.cpp commit e0085fd)
7 months ago
capybarahermes-2.5-mistral-7b.Q6_K.gguf

5.94 GB
LFS
GGUF model commit (made with llama.cpp commit e0085fd)
7 months ago
capybarahermes-2.5-mistral-7b.Q8_0.gguf

7.7 GB
LFS
GGUF model commit (made with llama.cpp commit e0085fd)
7 months ago
config.json
31 Bytes
GGUF model commit (made with llama.cpp commit e0085fd)
7 months ago
