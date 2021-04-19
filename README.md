<!--- ## Realistic Image Synthesis with AttnGAN and Transformers
In this work, we implement a unique deep learning design and GAN formulation to bridge these advances in text and image modeling, translating visual ideas from characters to pixels. In this paper, we proposed a new architecture AttnGAN-trans by infusing different transformer networks with AttnGAN [6] and three of its variants AttnBERT, AttnXL, AttnGPT by infusing BERT, XLNet, GPT2 transformer networks respectively. 
Soon, the complete work will be updated in this repo. --->


<h1> Transformer Models for Enhancing AttnGAN based Text to Image
    Generation </h1>
<!-- <p> The detail approach and algorithm of the work will be available here </p> -->
<!-- <i class="fa fa-github"></i> -->

<div>
    <p>
        <b>Abstract:</b> Deep neural networks are capable of producing photographic images that depict given natural language text descriptions. 
        Such models have huge potential in applications such as interior designing, video games, editing and facial sketching for 
        digital forensics. However, only a limited number of methods in the literature have been developed for text to image (TTI) 
        generation. Most of them use generative adversarial networks (GAN) based deep learning methods. Attentional GAN (AttnGAN) 
        is a popular GAN based TTI method that extracts meaningful information from the given text descriptions using attention 
        mechanism. In this paper, we investigate the use of different Transformer models such as BERT, GPT2, XLNet with AttnGAN
         to solve the challenge of extracting semantic information from the text descriptions. Hence, the proposed 
         AttnGAN<sub>TRANS</sub> architecture has three variants AttnGAN<sub>BERT</sub>, AttnGAN<sub>XL</sub> and AttnGAN<sub>GPT</sub>. The proposed method is successful 
          over the conventional AttnGAN and gives a boosted inception score by <b>27.23%</b> and a decline of Frechet inception distance 
          by <b>49.9%</b>. The results in our experiments indicate that the proposed method has the potential to outperform the contemporary 
          state-of-the-art methods and validate the use of Transformer models in improving the performance of TTI generation. <br>
          The code is made publicly available at 
          <a  class="about-link" href="https://github.com/sairamkiran9/AttnGAN-trans" target="_blank">AttnGAN<sub>TRANS</sub></a>
    </p>
</div>
<br>

<div>
    <h3> An Overview of AttnGAN<sub>TRANS</sub></h3>
  <p> We enhanced the AttnGAN model with the Transformers. The existing AttnGAN model generatives word embeddings 
    from the word2vec followed by RNNs. In our approach we introduced Transformer models in between word2vec and RNNs
    for better semantics of text-image. We compared this approach using BERT, GPT2 and XLNet over AttnGAN model. 
    For the comparision of quantitative metrics, we used inception Score (IS) and Frechet inception distance (FID). </p> 
   
   <img class = "myImg1" src="https://github.com/sairamkiran9/AttnGAN-trans/blob/master/imgs/A1.png"  width="600px">
   <h5>Fig.1: Transformer infused text encoder model.</h5>
<br>
        <img class = "myImg2" src="https://github.com/sairamkiran9/AttnGAN-trans/blob/master/imgs/A5.png" width="800px">
        <h5>Fig.2: A Transformer architecture with L encoder blocks and L decoder blocks, along with the encoder block components.</h5>
<br>
   <p>Transformers uses the attention-mechanism which determines the essential parts of the sequence 
    without a chance of losing the information due to external dependencies. The Transformers are made up of 
    an encoder-decoder structure which are stacked up high using attention layers. BERT, GPT2 and XLNet 
    mainly vary each other in the number of attention layer count and embeddings dimensions.
 </p>8
    <img class = "myImg3" src="https://github.com/sairamkiran9/AttnGAN-trans/blob/master/imgs/A4.png" width="800px">
    <h5>Fig.3: The proposed AttnGAN<sub>TRANS</sub> architecture for fine-grained text to image generation.</h5>
<br>
<h3>Experimental Setup</h3>
<p>
Our model is trained on CUB dataset, which contains 200 species of birds, each species has a set of 60 images
and ten respective text descriptions for each image. We have used 8855 images and their respective captions to train the
deep learning model and validate on 2933 images and their respective captions. We trained AttnGAN and its variants
with BERT, GPT2 and XLnet Transformers for 700 epochs on the google colaboratory platform with the support of 
free GPUs provided to test the results. The comparision of model performances is carried out using IS and FID evaluation metrics.
</p>
<br>
<h3>Qualitative Results</h3>
    <img class = "myImg4" src="https://github.com/sairamkiran9/AttnGAN-trans/blob/master/imgs/Birds.jpg" >
    <h5>Fig.4: Example results of different TTI generation models trained on CUB dataset</h5>
<br>
<h3>Quantitative Results</h3>
    <img class = "myImg5" src="https://github.com/sairamkiran9/AttnGAN-trans/blob/master/imgs/table.jpg" width="600px">
    <h5>Table showing the quality comparison of different models with IS and FID scores. Here
        a horizontal line is separating the state-of-the-art methods with
        our proposed models. Blue, purple, red corresponding to the
        first, second, third top results.</h5>
<br>
    <img class = "myImg6" src="https://github.com/sairamkiran9/AttnGAN-trans/blob/master/imgs/A2.jpeg" width="600px">
    <h5>Fig.5: Inception Score (IS) plot of proposed AttnGANTRANS model, taken over 700 epochs on CUB
        dataset.</h5>
<br>
    <img class = "myImg6" src="https://github.com/sairamkiran9/AttnGAN-trans/blob/master/imgs/A3.jpeg" width="600px">
    <h5>Fig.6: FID plot of proposed AttnGANTRANS model, taken
        over 700 epochs on CUB dataset.</h5>
<br>

<h3>Conclusion</h3>
<p> In this work, we introduced a Transformer-based AttnGAN
model for TTI synthesis. The challenge of giving
attention to essential words and deriving meaningful embeddings
is addressed by using powerful Transformers in the
field of NLP. We have conducted a series of experiments on
CUB dataset. For validation, we evaluated the performance
of the proposed method and different existing methods
qualitatively and quantitatively. We found that the proposed
method outperforms state-of-the-art methods and provides
a promising result for TTI generation. In future, we
test a combination of Transformers such as DeBERTa,
GPT3 and GAN architectures like DF-GAN, DMGAN for TTI generation </p>


<p> For more detail approach please do visit our github page 
    <a  class="about-link" href="https://github.com/sairamkiran9/AttnGAN-trans" target="_blank">AttnGAN<sub>TRANS</sub></a><div class=""></div></p>

</div>
  <!-- Footer -->
  <footer class="bg-light text-center text-lg-start ">

    
  
<div class="container-footer">
  © 2021 Copyright:
  <a class="text-dark" href="#">NoOne</a>
</div>

  
  </footer>
  <!-- Footer -->  
