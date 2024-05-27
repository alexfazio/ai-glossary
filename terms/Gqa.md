---
share: true
---

GQA stands for "Grouped Query Attention". This is a training strategy used to reduce the memory footprint of large Transformers by letting multiple queries share keys and values. I don't quite understand the technical details beyond that, but the important element is that it prevents the larger context size from being extremely expensive in terms of memory requirements, with almost no degradation on the end results. Llama 2 70b, Mixtral, Yi 34b, Mistral 7b are all examples of modern models that were trained with GQA.

### Related Articles

### Citations
