# Wikidata-Descriptions
Be Concise and Precise: Synthesizing Open-Domain Entity Descriptions from Facts

## Training and Inference
```
run_model.py --model MODEL_NAME --datadir PATH_TO_DATADIR --config PATH_TO_CONFIG_FILE_NAME --mode [training/eval]
```
MODEL_NAME can be NKLM, DGN, Fact2SeqAttn and PointerGenerator. E.g.
```
run_model.py --model NKLM --datadir Data/WikiFacts10k-OpenDomain --config Configs/NKLM-config.json --mode training
run_model.py --model PointerGenerator --datadir Data/WikiFacts10k-OpenDomain --config Configs/PointerGenerator-config.json --mode eval

```
## Evaluation
We used the automatic evaluation script developed by [Sharma et al., 2017](https://arxiv.org/pdf/1706.09799.pdf) 
To run the evaluation script, use

```
python evaluatation.py <model_name>.csv
```

## Authors

* **Rajarshi Bhowmik**  - [website](https://kingsaint.github.io)
* **Gerard de Melo** - [website](http://gerard.demelo.org)

## Citation

If you use this code, please cite our paper.

```
@inproceedings{BhowmikDeMelo2019EntityDescriptionsCopyModel,
  title = {Be Concise and Precise: Synthesizing Open-Domain Entity Descriptions from Facts},
  author = {Bhowmik, Rajarshi and {de Melo}, Gerard},
  booktitle = {Proceedings of The Web Conference 2019},
  year = {2019},
  location = {San Francisco},
}
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
