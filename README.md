# transformers-getting-started
A beginner-friendly project using Hugging Face Transformers to generate text with GPT-2. Includes basic usage of the text-generation pipeline and seed-controlled outputs.
# 🤗 Hugging Face Text Generation with GPT-2

This project demonstrates how to generate text using the `text-generation` pipeline from the Hugging Face `transformers` library. It uses the popular GPT-2 model and is perfect for anyone starting out with natural language processing (NLP).

## 🚀 What It Does

- Loads the GPT-2 model using Hugging Face’s pipeline interface
- Sets a random seed for reproducible results
- Generates multiple variations of text based on a starting prompt

## 📜 Example Code

```python
from transformers import pipeline, set_seed

generator = pipeline('text-generation', model='gpt2')

set_seed(42)
generator("Hello, I want you to know", max_length=30, num_return_sequences=5)
```

## 🧠 Concepts Learned

- Using `pipeline()` to simplify model usage
- Setting a seed with `set_seed()` for repeatable results
- Generating multiple text continuations with `num_return_sequences`
- Controlling output length using `max_length`

## 📦 Requirements

Install the required library with:

```bash
pip install transformers
```

## 📝 Sample Output

```
Hello, I want you to know what’s going on with you and what you need to do to fix it. I’m not going to let this go.
Hello, I want you to know what it’s like to be a parent. And I want you to be part of that.
Hello, I want you to know that you’ve been doing it right. You’re doing it right now.
Hello, I want you to know I’m not the only one who has to be a bit careful with this one.
Hello, I want you to know that I’ve been there before. You’re not alone.
```

## 🔖 Tags

huggingface • transformers • gpt2 • text-generation • nlp • python • ai

## 📚 References

- https://huggingface.co/docs/transformers/index
- https://huggingface.co/gpt2

## 💡 Next Steps

- Try different prompts
- Use `gpt2-medium` or `gpt2-large` for richer results
- Explore adding temperature and top-k sampling to influence creativity

## 🧑‍💻 Author

Created by **Jill Sharp** while learning Applied Generative AI  
GitHub: [https://github.com/jmsdevworks](https://github.com/jmsdevworks)
