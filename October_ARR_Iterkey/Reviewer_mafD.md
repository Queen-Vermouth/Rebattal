

> 1. **Inclusion of self answer verification step with LLM is in itself effectively using the LLM's parametric knowledge to judge the correctness of the answer. This may not work well in real world applications where LLM has no knowledge in. The proposed method made a strong assumption that LLM knows the correct answer. The iterative refinement step of the proposed method may go rogue outside the benchmarking environment.**


> 2. **While the results show good performance improvements over baselines, I believe the baselines in the experiments are weaker than necessary. I assume that the baseline RAG employs BM25 too. In this configuration, RAG is in its most basic form with a weak (but robust) retriever. Comparison with existing query expansion technique for sparse retrieval methods is necessary to prove the superiority of the method. Dense retrievers are nearly not mentioned in the paper. Comparison with existing dense-retriever-based RAG methods is also needed in my opinion. Moreover, have a dense-retriever-based RAG + query expansion scenario would make the arguments stronger too. The current experimental results, observations and discussions in the paper may mislead the paper's conclusion.**






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
