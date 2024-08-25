1.  wizard-math: https://drive.google.com/file/d/1MrrsXhSTXlLqrZhTVkjQaW_pRjn58Tm_/view?usp=drive_link
    starcoder2: https://drive.google.com/file/d/1KTqgE5qLA5xs_ll2K0V4zPtjmJaRi2u0/view?usp=drive_link
    starcoder: https://drive.google.com/file/d/1TSTfOr-fIGT1YoStUG46_30GY_MLbvvR/view?usp=drive_link
    qwen2: https://drive.google.com/file/d/1AgpgOTe4dT71fQb1lpkNsTwuPhw4o0Or/view?usp=drive_link
    phi3*14b: https://drive.google.com/file/d/1sKz0v2xcVAElkvtAy4VdNaTzAI0k8kOU/view?usp=drive_link
    moondream: https://drive.google.com/file/d/1PsO5c8rp8DXFxFIowo4iNR7hcZYN6wBS/view?usp=drive_link
    mistral: https://drive.google.com/file/d/1IdTVYh9dme1soXciZm-TrnH_Rdeu7t6m/view?usp=drive_link
    mistral-nemo: https://drive.google.com/file/d/1qk-WfCrtnbI0EM9JxBBD42lXXTxWmnV0/view?usp=drive_link
    meditron: https://drive.google.com/file/d/1dTV1PBBtpbofFBzz8wgQuF9noNW7v8Kn/view?usp=drive_link
    mathstral: https://drive.google.com/file/d/1kB1obPhhpcKu5p_IYrGWT-o_c2EXDhF2/view?usp=drive_link
    llava: https://drive.google.com/file/d/1XV2uQNyGzIPdqPQnYrwA9DrXYBjquef*/view?usp=drive_link
    llava-llama3: https://drive.google.com/file/d/1DqV1tt9l9TGF73_2HM0yx56ijRVg9Otm/view?usp=drive_link
    llama3-chatqa: https://drive.google.com/file/d/1-Ieww2X-sCFswMOr0CGXWG5nk7iMMECF/view?usp=drive_link
    gemma2: https://drive.google.com/file/d/1TiPkbXcjtmS62lTh8I5lfQYWs4CfbqVj/view?usp=drive_link
    codestral: https://drive.google.com/file/d/1EJGGW_HEzHPvHQF7l5WCJtmE5sIOFmf8/view?usp=drive_link
    codegemma: https://drive.google.com/file/d/19AHS0n0Cz-rmwQY3a3fHTAMr8YrGvRFg/view?usp=drive_link
    solar: https://drive.google.com/file/d/1WIKT0hWw64BWcc0SF6t0m1p7nHN2jadz/view?usp=drive_link

2.  all-minilm: https://drive.google.com/file/d/10QsspRGHs-D5HO8mF4Bhc5-AqHP4BJko/view?usp=drive_link
    bge-large: https://drive.google.com/file/d/1FhogmYTuzUY3nMbGbJ72BGP1Tk7Q2eol/view?usp=drive_link
    codellama: https://drive.google.com/file/d/1WOTTqKhNGEHm61zk3NIGoS75PWNqurOA/view?usp=drive_link
    llama3.1: https://drive.google.com/file/d/1kUzXecg2t_CorIStHQLN-E4v6-eUGQUO/view?usp=drive_link
    nomic-embed-text: https://drive.google.com/file/d/1ZIP-8pZdWngl-HQiQaIAzaJUscwUztMW/view?usp=drive_link
    paraphrase-multilingual: https://drive.google.com/file/d/1hI9XyVCnSXHweO2up8CPsKRoBEeNjPR6/view?usp=drive_link

3.  how to use embedding model

https://ollama.com/library/nomic-embed-text

nomic-embed-text is a large context length text encoder that surpasses OpenAI text-embedding-ada-002 and text-embedding-3-small performance on short and long context tasks.

Usage
This model is an embedding model, meaning it can only be used to generate embeddings.

REST API
curl http://localhost:11434/api/embeddings -d '{
"model": "nomic-embed-text",
"prompt": "The sky is blue because of Rayleigh scattering"
}'
Python library
ollama.embeddings(model='nomic-embed-text', prompt='The sky is blue because of rayleigh scattering')
Javascript library
ollama.embeddings({ model: 'nomic-embed-text', prompt: 'The sky is blue because of rayleigh scattering' })

4. https://github.com/vikhyat/moondream
   a tiny vision language model that kicks ass and runs anywhere
