
> 1.　**Lack of Comparison to Other Retrieval Methods:** The paper focuses only on BM25 for retrieval. Comparing the performance of ITERKEY with many other retrieval methods, such as dense retrieval or neural sparse models like SPLADE, would provide a more comprehensive understanding of its strengths and weaknesses.



> 2.**Limited Novelty:** While ITERKEY presents an interesting application of LLMs for RAG optimization, its novelty is limited. The core idea of using LLMs for query expansion and answer verification is not new. Several existing works, such as those mentioned in the Related Work section explore similar concepts. ITERKEY primarily distinguishes itself through its iterative process and specific prompt engineering. However, the paper would benefit from a clearer articulation of its unique contributions and a more in-depth comparison with existing iterative retrieval methods.



> 3. **Computational Cost:** ITERKEY's iterative nature introduces additional computational costs compared to non-iterative RAG methods. The authors should discuss the trade-off between accuracy gains and computational cost in more detail.



> 4. **Potential for Underestimation of Results:** The evaluation process relies heavily on exact pattern matching for answer verification. This may underestimate the model's performance, as semantically correct answers expressed in different formats might be marked as incorrect. The authors should discuss the limitations of their evaluation methodology and consider alternative evaluation metrics that capture semantic similarity.



> **Consider incorporating other evaluation metrics, such as ROUGE, BLEU and BERT-Score, in addition to Exact Match, to address the limitations of pattern matching and provide a more nuanced assessment of answer quality.**







| Language   | En-En | En-{Lang} | {Lang}-En | {Lang}-{Lang} |
|------------|-------|-----------|-----------|---------------|
| English    | 864   | -         | -         | -             |
| French     | -     | 1,780     | 1,180     | 856           |
| Spanish    | -     | 964       | 1,176     | 668           |
| Italian    | -     | 1,092     | 1,244     | 596           |
| Russian    | -     | 668       | 1,184     | 604           |
| Japanese   | -     | 1,012     | 1,244     | 572           |
| German     | -     | 732       | 1,208     | 1,132         |
| Dutch      | -     | 556       | 1,284     | 468           |
| Swedish    | -     | 912       | 1,164     | 444           |
| Chinese    | -     | 1,092     | 1,304     | 612           |
