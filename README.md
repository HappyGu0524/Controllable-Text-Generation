# Controllable-Generation

![](https://img.shields.io/badge/Status-building-brightgreen)

## VAE
1. **Extracting and composing robust features with denoising autoencoders** *Pascal Vincent, Hugo Larochelle, Yoshua Bengio, Pierre-Antoine Manzagol* `ICML08` [[PDF]](https://www.cs.toronto.edu/~larocheh/publications/icml-2008-denoising-autoencoders.pdf) ![](https://img.shields.io/badge/DAE-MLP-red)
2. **Auto-Encoding Variational Bayes** *Diederik P Kingma, Max Welling* `ICLR14` [[PDF]](https://arxiv.org/pdf/1312.6114.pdf) ![](https://img.shields.io/badge/VAE-RNN-red)
3. **Generating Sentences from a Continuous Space** *Samuel R. Bowman, Luke Vilnis* `CONLL16` [[PDF]](https://arxiv.org/pdf/1511.06349.pdf) ![](https://img.shields.io/badge/VAE-RNN-red)
4. **Adversarial Autoencoders** *Alireza Makhzani, Jonathon Shlens, Navdeep Jaitly, Ian Goodfellow, Brendan Frey* `ICLR16` [[PDF]](https://arxiv.org/pdf/1511.05644.pdf) ![](https://img.shields.io/badge/AAE-RNN-red)
5. **Learning Structured Output Representation using Deep Conditional Generative Models** *Kihyuk Sohn, Xinchen Yan, Honglak Lee* `NIPS15` [[PDF]](https://papers.nips.cc/paper/2015/file/8d55a249e6baa5c06772297520da2051-Paper.pdf) ![](https://img.shields.io/badge/CVAE-CNN-red)
6. **Deep Unsupervised Clustering with Gaussian Mixture Variational Auotoencoders** *Nat Dilokthanakul, Pedro A. M. Mediano, Marta Garnelo, Matthew C. H. Lee, Hugh Salimbeni, Kai Arulkumaran, Murray Shanahan* `ICLR17` [[PDF]](https://arxiv.org/pdf/1611.02648.pdf) ![](https://img.shields.io/badge/VAEGMM-RNN-red)
7. **Wasserstein Auto-Encoders** *Ilya Tolstikhin, Olivier Bousquet, Sylvain Gelly, Bernhard Sch¨olkopf* `ICLR18` [[PDF]](https://arxiv.org/pdf/1711.01558.pdf) [[code]](https://github.com/KyleGoyette/WassersteinAutoEncoder) ![](https://img.shields.io/badge/WAE-CNN-red)
8. **Adversarially Regularized Autoencoders** *Jake Zhao, Yoon Kim, Kelly Zhang, Alexander M. Rush, Yann LeCun* `ICML18` [[PDF]](https://arxiv.org/pdf/1706.04223v3.pdf) [[code]](https://github.com/jakezhaojb/ARAE) ![](https://img.shields.io/badge/ARAE-RNN-red) <details> <summary><mark>model</mark></summary> <img src="https://github.com/HappyGu0524/pic/blob/master/img/20210318194000.png" width="60%" title="Replace KL divergence with adversarial classifier" align="middle" /> </details> <details> <summary><mark>algorithm</mark></summary> <img src="https://github.com/HappyGu0524/pic/blob/master/img/20210318194045.png" width="60%" align="middle" title="1.Reconstruction Loss; 2.Train Classifier; 3.Train Generator" /> </details>
9. **T-CVAE: Transformer-Based Conditioned Variational Autoencoder for Story Completion** *Tianming Wang, Xiaojun Wan* `IJCAI19` [[PDF]](https://www.ijcai.org/proceedings/2019/0727.pdf) [[code]](https://github.com/sodawater/T-CVAE) ![](https://img.shields.io/badge/CVAE-Transformer-red)<details> <summary><mark>abstract</mark></summary> Story completion is a very challenging task of generating the missing plot for an incomplete story, which requires not only understanding but also inference of the given contextual clues. In this paper, we present a novel conditional variational autoencoder based on Transformer for missing plot generation. Our model uses shared attention layers for encoder and decoder, which make the most of the contextual clues, and a latent variable for learning the distribution of coherent story plots. Through drawing samples from the learned distribution, diverse reasonable plots can be generated. Both automatic and manual evaluations show that our model generates better story plots than stateof-the-art models in terms of readability, diversity and coherence.</details> <details> <summary><mark>model</mark></summary> <img src="https://github.com/HappyGu0524/pic/blob/master/img/20210318194427.png" width="60%" align="middle" /> </details>
10. **Transformer-based Conditional Variational Autoencoder for Controllable Story Generation** *Le Fang, Tao Zeng, Chaochun Liu, Liefeng Bo, Wen Dong, Changyou Chen* `arXiv` [[PDF]](https://arxiv.org/pdf/2101.00828v1.pdf) [[code]](https://github.com/fangleai/TransformerCVAE) ![](https://img.shields.io/badge/CVAE-Transformer-red)<details> <summary><mark>abstract</mark></summary> We investigate large-scale latent variable models (LVMs) for neural story generation—an under-explored application for open-domain long text—with objectives in two threads: generation effectiveness and controllability. LVMs, especially the variational autoencoder (VAE), have achieved both effective and controllable generation through exploiting flexible distributional latent representations. Recently, Transformers and its variants have achieved remarkable effectiveness without explicit latent representation learning, thus lack satisfying controllability in generation. In this paper, we advocate to revive latent variable modeling, essentially the power of representation learning, in the era of Transformers to enhance controllability without hurting state-of-the-art generation effectiveness. Specifically, we integrate latent representation vectors with a Transformer-based pre-trained architecture to build conditional variational autoencoder (CVAE). Model components such as encoder, decoder and the variational posterior are all built on top of pre-trained language models—GPT2 specifically in this paper. Experiments demonstrate state-of-the-art conditional generation ability of our model, as well as its excellent representation learning capability and controllability.</details> <details> <summary><mark>model</mark></summary> <img src="https://github.com/HappyGu0524/pic/blob/master/img/20210318194813.png" width="60%" align="middle" /> </details>
11. **APo-VAE: Text Generation in Hyperbolic Space** *Shuyang Dai, Zhe Gan, Yu Cheng, Chenyang Tao, Lawrence Carin, Jingjing Liu* `NAACL21` [[PDF]](https://arxiv.org/pdf/2005.00054.pdf) [code] ![](https://img.shields.io/badge/APoVAE-RNN-red)

## Controlling information
### Text as exemplar
#### Unparallel text
1. **Disentangled Representation Learning for Non-Parallel Text Style Transfer** *Vineet John, Lili Mou, Hareesh Bahuleyan, Olga Vechtomova* `ACL19` [[PDF]](https://arxiv.org/pdf/1808.04339.pdf) [[code]](https://github.com/vineetjohn/linguistic-style-transfer) ![](https://img.shields.io/badge/Yelp&Amazon-Style%20Transfer-orange) <details> <summary><mark>motivation</mark></summary> To tackle the problem of disentangling the latent representations of style and content in language models.</details> <details> <summary><mark>model</mark></summary> <img src="https://github.com/HappyGu0524/pic/blob/master/img/20210411113202.png" width="80%" align="middle" /> </details>
2. **Pre-train and Plug-in: Flexible Conditional Text Generation with Variational Auto-Encoders** *Yu Duan, Canwen Xu, Jiaxin Pei, Jialong Han, Chenliang Li* `ACL20` [[PDF]](https://arxiv.org/pdf/1911.03882.pdf) [[code]](https://github.com/WHUIR/PPVAE) ![](https://img.shields.io/badge/Yelp&NewsTitle-Controllable%20Generation-orange) <details> <summary><mark>motivation</mark></summary> Flexible when new conditions added to a well trained VAE which requires no more retraining.</details> <details> <summary><mark>abstract</mark></summary> Conditional Text Generation has drawn much attention as a topic of Natural Language Generation (NLG) which provides the possibility for humans to control the properties of generated contents. Current conditional generation models cannot handle emerging conditions due to their joint end-to-end learning fashion. When a new condition added, these techniques require full retraining. In this paper, we present a new framework named Pre-train and Plug-in Variational Auto-Encoder (PPVAE) towards flexible conditional text generation. PPVAE decouples the text generation module from the condition representation module to allow “one-to-many” conditional generation. When a fresh condition emerges, only a lightweight network needs to be trained and works as a plug-in for PPVAE, which is efficient and desirable for real-world applications. Extensive experiments demonstrate the superiority of PPVAE against the existing alternatives with better conditionality and diversity but less training effort.</details> <details> <summary><mark>model</mark></summary> <img src="https://github.com/HappyGu0524/pic/blob/master/img/20210408195017.png" width="80%" title="a) PretrainVAE; b) PluginVAE for each style; c) sample and generate" align="middle" /> </details>
3. **Plug and Play Autoencoders for Conditional Text Generation** *Florian Mai, Nikolaos Pappas, Ivan Montero, Noah A. Smith, James Henderson* `EMNLP20`[[PDF]](https://arxiv.org/pdf/2010.02983.pdf) [[code]](https://github.com/florianmai/emb2emb) ![](https://img.shields.io/badge/Yelp-Controllable%20Generation-orange)  <details> <summary><mark>motivation</mark></summary> Reduce the need for labeled training data for the task and makes the training procedure more efficient by learning a mapping within the autoencoder’s embedding space.<br> <img src="https://github.com/HappyGu0524/pic/blob/master/img/20210410153238.png" width="60%" title="The manifold of a text autoencoder is the low-dimensional region of the high-dimensional embedding space where texts are actually embedded." align="middle" /></details> <details> <summary><mark>model</mark></summary> <img src="https://github.com/HappyGu0524/pic/blob/master/img/20210410152622.png" width="80%" title="a) PretrainVAE; b) Training a mapping function; c) Map manifold from input to output" align="middle" /> </details>


3. **Stylized Dialogue Response Generation Using Stylized Unpaired Texts** *Yinhe Zheng, Zikai Chen, Rongsheng Zhang, Shilei Huang, Xiaoxi Mao, Minlie Huang* `AAAI 21` [[PDF]](https://arxiv.org/pdf/2009.12719.pdf) [[code]](https://github.com/silverriver/Stylized_Dialog) ![](https://img.shields.io/badge/TCFC-Dialogue%20Generation-orange) <details> <summary><mark>model</mark></summary> <img src="https://github.com/HappyGu0524/pic/blob/master/img/20210406104923.png" width="60%" title="Transformer incorporating style embedding" align="middle" /> </details> <details> <summary><mark>algorithm</mark></summary> <img src="https://github.com/HappyGu0524/pic/blob/master/img/20210406105228.png" width="60%" align="middle" title="3-5: Train both forward and backward transformers, forward with style while backward without style; 9-12: Back translation to get synthetic data; 13: Style transfer" /> </details>
4. **Plug and Play Language Models: A Simple Approach to Controlled Text Generation** *Sumanth Dathathri, Andrea Madotto, Janice Lan, Jane Hung, Eric Frank, Piero Molino, Jason Yosinski, Rosanne Liu* `ICLR20` [[PDF]](https://arxiv.org/pdf/1912.02164.pdf) [[code]](https://github.com/uber-research/PPLM)
5. **Hooks in the Headline: Learning to Generate Headlines with Controlled Styles** *Di Jin, Zhijing Jin, Joey Tianyi Zhou, Lisa Orii, Peter Szolovits* `ACL20` [[PDF]](https://arxiv.org/pdf/2004.01980v3.pdf) [[code]](https://github.com/jind11/TitleStylist) ![](https://img.shields.io/badge/NYT&CNN&Humor&Romance&Clickbait-Headline%20Generation-orange)  <details> <summary><mark>motivation</mark></summary> Enrich headlines with controlled style options.<br> <img src="https://github.com/HappyGu0524/pic/blob/master/img/20210410160152.png" width="60%" align="middle" /></details> <details> <summary><mark>model</mark></summary> <img src="https://github.com/HappyGu0524/pic/blob/master/img/20210410160246.png" width="60%" title="Entangle latent representation of stylied generation and summarization by partially parameter sharing." align="middle" /> </details>


#### Parallel text

### Text signals
1. **CTRL: A Conditional Transformer Language Model for Controllable Generation** *Nitish Shirish Keskar, Bryan McCann, Lav R. Varshney, Caiming Xiong, Richard Socher* `arXiv` [[PDF]](https://arxiv.org/pdf/1909.05858.pdf) [[code]](https://github.com/salesforce/ctrl) ![](https://img.shields.io/badge/OpenWebText-Generation-orange) <details> <summary><mark>control code type</mark></summary> <p>Style by domain <p>More complex control codes <p>Triggering specific tasks <p>Zero-shot code-mixing </details>
2. **A Controllable Model of Grounded Response Generation** *Zeqiu Wu, Michel Galley, Chris Brockett, Yizhe Zhang, Xiang Gao, Chris Quirk, Rik Koncel-Kedziorski, Jianfeng Gao, Hannaneh Hajishirzi, Mari Ostendorf, Bill Dolan* `AAAI21` [[PDF]](https://arxiv.org/pdf/2005.00613.pdf) [code] ![](https://img.shields.io/badge/Reddit%20conversation-Response%20Generation-orange)  <details> <summary><mark>model</mark></summary> <img src="https://github.com/HappyGu0524/pic/blob/master/img/20210406155858.png" width="60%" title="GPT2 with Inductive Attention" align="middle" /> </details>
3. **Generate Your Counterfactuals: Towards Controlled Counterfactual Generation for Text** *Nishtha Madaan, Inkit Padhi, Naveen Panwar, Diptikalyan Saha* `AAAI21` [[PDF]](https://arxiv.org/pdf/2012.04698.pdf) [code] ![](https://img.shields.io/badge/DBPedia&AgNews&Yelp-Counterfactual%20Generation-orange)
4. **GEDI: GENERATIVE DISCRIMINATOR GUIDED SEQUENCE GENERATION** *Ben Krause, Akhilesh Deepak Gotmare, Bryan McCann, Nitish Shirish Keskar, Shafiq Joty, Richard Socher, Nazneen Fatema Rajani* `arXiv` [[PDF]](https://arxiv.org/pdf/2009.06367.pdf) [[code]](https://github.com/salesforce/GeDi) ![](https://img.shields.io/badge/IMDb-Controlled%20Generation-orange) 

### Syntactic Guidance
1. **Syntax-guided Controlled Generation of Paraphrases** *Ashutosh Kumar, Kabir Ahuja, Raghuram Vadapalli, Partha Talukdar* `TACL20` [[PDF]](https://arxiv.org/pdf/2005.08417v1.pdf) [[code]](https://github.com/malllabiisc/SGCP) ![](https://img.shields.io/badge/ParaNMT&QQP-Syntax%20Guided%20Controlled%20Generation-orange) <details> <summary><mark>model</mark></summary> <img src="https://github.com/HappyGu0524/pic/blob/master/img/20210410162843.png" width="60%" align="middle" /> </details>
2. **Transformer-Based Neural Text Generation with Syntactic Guidance** *Yinghao Li, Rui Feng, Isaac Rehg, Chao Zhang* `arXiv` [[PDF]](https://arxiv.org/pdf/2010.01737v1.pdf) [[code]](https://github.com/Yinghao-Li/GuiGen) ![](https://img.shields.io/badge/ParaNMT-Syntax%20Guided%20Controlled%20Generation-orange) <details><summary><mark>model</mark></summary> <img src="https://github.com/HappyGu0524/pic/blob/master/img/20210414202208.png" width="40%" align="middle" title="" /> </details> 

### Multi-signals
1. **A Distributional Approach To Controlled Text Generation** *Muhammad Khalifa, Hady Elsahar, Marc Dymetman* `ICLR21` [[PDF]](https://arxiv.org/pdf/2012.11635.pdf) [code] ![](https://img.shields.io/badge/Wikipedia-Controllable%20Generation-orange) <details><summary><mark>model</mark></summary> <img src="https://github.com/HappyGu0524/pic/blob/master/img/20210408164750.png" width="40%" align="middle" title="Energy-Based Model" /> </details> <details> <summary><mark>algorithm</mark></summary> <img src="https://github.com/HappyGu0524/pic/blob/master/img/20210408163917.png" width="60%" align="middle" title="Reward = P(x)/q(x); q initialized with pretrained gpt2; from Energy-Based Model to Autoregressive Policy"/> </details>
2. **Plug-and-Blend: A Framework for Controllable Story Generation with Blended Control Codes** *Zhiyu Lin, Mark O. Riedl* `arXiv` [[PDF]](https://arxiv.org/pdf/2104.04039.pdf) [code] (https://img.shields.io/badge/ROCStories-Controlled%20Generation-orange) 

## Evaluation
1. **Evaluating Style Transfer for Text** *Remi Mir, Bjarke Felbo, Nick Obradovich, Iyad Rahwan* `NAACL19` [[PDF]](https://arxiv.org/pdf/1904.02295.pdf) [[code]](https://github.com/passeul/style-transfer-model-evaluation) ![](https://img.shields.io/badge/EMD-Style%20Transfer-blue)

## Benchmark
1. **StylePTB: A Compositional Benchmark for Fine-grained Controllable Text Style Transfer** *Yiwei Lyu, Paul Pu Liang, Hai Pham, Eduard Hovy, Barnabás Póczos, Ruslan Salakhutdinov, Louis-Philippe Morency* `NAACL21` [[PDF]](https://arxiv.org/pdf/2104.05196.pdf) [[code]](https://github.com/lvyiwei1/StylePTB/)
2. **Expertise Style Transfer: A New Task Towards Better Communication between Experts and Laymen** *Yixin Cao, Ruihao Shui, Liangming Pan, Min-Yen Kan, Zhiyuan Liu, Tat-Seng Chua* `ACL20` [[PDF]](https://arxiv.org/pdf/2005.00701.pdf) [[code]](https://srhthu.github.io/expertise-style-transfer/)
