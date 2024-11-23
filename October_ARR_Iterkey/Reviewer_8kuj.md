
> **The method lacks novelty and significant technical contribution. The proposed method is a series of prompts that simply extract keywords from user query based on previous error.**
>> 新規性や重要な技術的貢献の欠如：提案手法は、一連のプロンプトによってユーザーのクエリから単純にキーワードを抽出し、以前のエラーに基づいて再生成するものであり、新規性や重要な技術的貢献が不足しています。


> **The proposed method contains some flaws. It does not make sense to regenerate the keyword without any references on the previously retrieved documents. And it is hard to verify the correctness of the answer especially when the model hallucinates heavily.**
>> 提案手法の欠陥：提案された手法にはいくつかの欠陥があります。特に、以前に取得された文書を参照せずにキーワードを再生成することは意味をなさず、モデルが大きく幻覚を起こす場合には、回答の正確性を検証するのが難しいです。


 
> **i understand that the paper only supports sparse retrievers, but they might not be the optimal choice in all circumstances. Therefore, it is also important to include dense retrieval or others.**
>> スパースリトリーバーのみに対応：本論文がスパースリトリーバーのみをサポートしている点は理解していますが、それがすべての状況で最適な選択肢であるとは限りません。そのため、密なリトリーバーや他の手法を含めることも重要です。











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
