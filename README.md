# **Music Recommender System**  
### *Recommendations based on decomposition, vector space, and multimodal data.*  

## **Description**  
This music recommendation system focuses on working with three types of data: numeric track parameters, extracted audio openings, and the semantic component in the form of song lyrics. 

---

## **Technologies**  
<div align="left">
  
|**Category**           |**Tools**                                                                                      |
|-----------------------|-----------------------------------------------------------------------------------------------|
| Programming language  | ![Python](https://img.shields.io/badge/Python-3.11.1-blue?logo=python)                          |
| Data (metadata)       | PCA, StandardScaler                                                                           |
| Data (audio)          | preview_url -> .m4a/.wav -> using librosa MFCC-coefficients + extra metrics                   |
| Data (lyrics)         | BERT/SBERT -> Paraphrase-MiniLM-L6-v2, paraphase-multilingual-MiniLM-L12-v2, all-MiniLM-L6-v2 |
| Main methods          | KMeans, embeddings, cosine_similarity, working with features                                  |
| Implementation        | Gradio                                                                                        |

</div>

---

## **The structure of the work** 

The work consists of several stages:
1. Extraction, processing and transformation of data and their division into three vectors: numerical data, audio and lyrics
2. Step-by-step creation of a recommendation model using cosine proximity for each direction
3. Combining all three models and experiments to evaluate the accuracy of recommendations
4. Сreating an interface for testing the model on real users
5. Evaluation of results and summing up

```bash
git clone https://github.com/zaruba8/music-recommender-system.git
cd music-recommender-system
