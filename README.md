# 診療テキストの構造化に向けた症例報告コーパスからの情報抽出

本リポジトリは2022年度人工知能学会全国大会の医療言語処理の拡張と連携 (OS-13)で発表した「診療テキストの構造化に向けた症例報告コーパスからの情報抽出」の実験コードです。

## Setpu
### Requirements

- Python 3.8+
- pandas 1.2.4
- numpy 1.20.1
- torch 1.10.1+cu113
- scikit-learn 0.24.1
- transformers 4.11.3
- seqeval 1.2.2

## Run

 UTH-BERTを[こちら](https://ai-health.m.u-tokyo.ac.jp/home/research/uth-bert)からダウンロードして任意の場所に置いてください。

Jointモデルの訓練と評価（ファイル内のパスは環境に応じて修正してください）
```
bash run_joint.sh
```

Pipelineモデルの訓練と評価（ファイル内のパスは環境に応じて修正してください）
```
bash run_pipeline.sh
```

# License
CC BY-NC-SA 4.0

## References

- Ma, Y., Hiraoka, T., & Okazaki, N. (2020). Named Entity Recognition and Relation Extraction using Enhanced Table Filling by Contextualized Representations. arXiv preprint arXiv:2010.07522. Software available from https://github.com/YoumiMa/TablERT.
- pytorch-crf. Software available from https://pytorch-crf.readthedocs.io/en/stable/.
- Hiroki Nakayama. seqeval: A python framework for sequence labeling evaluation, 2018. Software available from https://github.com/chakki-works/seqeval.

## Other
実験に使用した症例報告コーパスは[こちら](https://ai-health.m.u-tokyo.ac.jp/home/research/corpus)からダウンロードできます。

## Citation

本リポジトリを参照する場合は以下の文献を文献を引用してください。

```
柴田 大作, 河添 悦昌, 篠原 恵美子, 嶋本 公徳. 診療テキストの構造化に向けた症例報告コーパスからの情報抽出. 第36回人工知能学会全国大会.
```
