# CausalBank

In our IJCAI 2020 paper "Guided Generation of Cause and Effect", we released two causal resources:

+ CausalBank: A very large-scale, open domain, sentence-level, parallel causal corpus. It's divided into two parts according to the order of cause and effect appeared in the sentence: because\_mode (effect, then cause), and therefore\_mode (cause, then effect). This corpus was used in our paper for training a seq2seq causal generation model, see the paper and our [online causal generation demo](http://openeg.8wss.com/generate/) for reference.

+ Cause Effect Graph: A lexical cause effect graph from causal contexts, with frequencies. This corpus was a refinement over [this previous work](http://www.cs.sjtu.edu.cn/~kzhu/papers/kzhu-copa.pdf), and used in our paper for looking up the guided causal keywords.

These two resources were both obtained using fine-grained causal template matching from the preprocessed [English Common Crawl corpus (5.14 TB)](http://www.lrec-conf.org/proceedings/lrec2014/pdf/1097_Paper.pdf), totally automatically without any human annotation. There is noise inside it, more or less. So adapt it to your research cases.

In our assumption, the above causal resources may benefit such future studies like: constructing causal eventic graphs, causal relations extraction, sentiment causal discovery, training neural causal generation models, explanable text inference, causal reading comprehension like CosmosQA, or just used as an external causal commonsense knowledge base.

## Download

You can download them either from Google Drive: [CausalBank](https://drive.google.com/drive/u/1/folders/1VYHcTUrQmw0ub9j14eGMOfNttKtryv87) and [Cause Effect Graph](https://drive.google.com/drive/folders/14iTAacR2wd5MO3PgQYp2pETbOOtZklCG), or from Baidu Yun: [CausalBank and Cause Effect Graph](https://pan.baidu.com/s/1TPmWVy0YdQIurqUdf3ayOA), with the access code: wjqw

## Statistics

#### CausalBank: 314 million sentence-level cause-effect pairs

+ because mode: 133 million
+ therefore mode: 181 million

#### Cause Effect Graph (CEG): 89.1 million word-level cause-effect pairs

The three numbers for each cause-effect pair in CEG are: the number of occurrences of the pair, necessity causality score, and sufficiency causality score.


## Citation
If you find our causal resources benifit your research, please cite the following paper:

+ [Guided Generation of Cause and effect](https://www.ijcai.org/Proceedings/2020/502). Zhongyang Li, Xiao Ding, Ting Liu, J. Edward Hu, Benjamin Van Durme. Proceedings of the Twenty-Ninth International Joint Conference on Artiﬁcial Intelligence (IJCAI 2020).

```
@inproceedings{ijcai2020-guided,
  title     = {Guided Generation of Cause and Effect},
  author    = {Li, Zhongyang and Ding, Xiao and Liu, Ting and Hu, J. Edward and Van Durme, Benjamin},
  booktitle = {Proceedings of the Twenty-Ninth International Joint Conference on
               Artificial Intelligence, {IJCAI-20}},
  publisher = {International Joint Conferences on Artificial Intelligence Organization},             
  editor    = {Christian Bessiere},	
  pages     = {3629--3636},
  year      = {2020},
  month     = {7},
  note      = {Main track}
  doi       = {10.24963/ijcai.2020/502},
  url       = {https://doi.org/10.24963/ijcai.2020/502},
}

```
## Contact
Please feel free to contact anyone of the authors!
