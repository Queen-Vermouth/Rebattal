

> 1. **Inclusion of self answer verification step with LLM is in itself effectively using the LLM's parametric knowledge to judge the correctness of the answer. This may not work well in real world applications where LLM has no knowledge in. The proposed method made a strong assumption that LLM knows the correct answer. The iterative refinement step of the proposed method may go rogue outside the benchmarking environment.**
>> LLMによる自己回答検証ステップの問題：LLMを用いた自己回答検証ステップは、LLMのパラメトリック知識を利用して回答の正確性を判断する方法そのものです。しかし、これはLLMが知識を持たない現実の応用場面ではうまく機能しない可能性があります。提案手法は、LLMが正しい答えを知っているという強い仮定を置いています。提案手法の反復的な改善ステップは、ベンチマーク環境外では不適切な挙動を示す可能性があります。


> 2. **While the results show good performance improvements over baselines, I believe the baselines in the experiments are weaker than necessary. I assume that the baseline RAG employs BM25 too. In this configuration, RAG is in its most basic form with a weak (but robust) retriever. Comparison with existing query expansion technique for sparse retrieval methods is necessary to prove the superiority of the method. Dense retrievers are nearly not mentioned in the paper. Comparison with existing dense-retriever-based RAG methods is also needed in my opinion. Moreover, have a dense-retriever-based RAG + query expansion scenario would make the arguments stronger too. The current experimental results, observations and discussions in the paper may mislead the paper's conclusion.**
>>ベースラインの弱さ：結果はベースラインに対して良好な性能向上を示していますが、実験で用いられたベースラインが必要以上に弱いと考えています。ベースラインのRAGもBM25を採用していると仮定しています。この構成では、RAGは最も基本的な形態であり、弱い（ただし堅牢な）リトリーバーに依存しています。提案手法の優位性を証明するには、スパースリトリーバー向けの既存のクエリ拡張技術との比較が必要です。また、論文では密なリトリーバーについてほとんど言及されていません。既存の密なリトリーバーに基づくRAG手法との比較も必要だと思います。さらに、密なリトリーバーを用いたRAG + クエリ拡張のシナリオを含めることで、議論がより説得力を持つでしょう。結論の誤解を招く可能性：現在の実験結果や観察、議論は、論文の結論を誤解させる可能性があります。






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
