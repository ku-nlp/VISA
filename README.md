VISA
==========

VISA is a dataset that consists of 40k Japanese-English parallel sentence pairs and corresponding video clips with the following key features: 
  - The parallel sentences are subtitles from movies and TV episodes
  - The source subtitles are ambiguous, which means they have multiple possible translations with different meanings
  - We divide the dataset into Polysemy and Omission according to the cause of ambiguity

Splits:
-------------------

| Split      | Train     | Validation     | test     |
| ---------- | :-----------:  | :-----------: | :-----------: |
|Polysemy      |   18,666      |     1,000        |         1,000 |
|Omission      |   17,214      |     1,000        |         1,000 |
|Combined      |   35,880      |     2,000        |         2,000 |

Usage:
-------------------
You can read json files to find the mapping from videos to parallel subtitle pairs.

Json Files Structure:
-------------------  
video_file_name: {  
&emsp;&emsp;      { "ja": Japanese_subtitle },  
&emsp;&emsp;      { "en": English_subtitle }  
}  

Note:
-------------------
Please, note that by downloading the dataset, you agree to the following conditions:
  - Do not re-distribute the dataset without our permission.
  - We do not officially distribute the video clips. Do not disclose this anywhere, even in your paper.
  - The dataset can only be used for research purposes. Any other use is explicitly prohibited.


Citing:
-------------------
If you find this dataset helpful, please cite our publication "VISA: An Ambiguous Subtitles Dataset for Visual Scene-Aware Machine Translation":  
@misc{li2022visa,  
&emsp;&emsp;      title="VISA: An Ambiguous Subtitles Dataset for Visual Scene-Aware Machine Translation",  
&emsp;&emsp;      author="Yihang Li and Shuichiro Shimizu and Weiqi Gu and Chenhui Chu and Sadao Kurohashi",  
&emsp;&emsp;      year="2022",  
&emsp;&emsp;      eprint="2201.08054",  
&emsp;&emsp;      archivePrefix="arXiv",  
&emsp;&emsp;      primaryClass="cs.CL",  
&emsp;&emsp;      url = "https://arxiv.org/abs/2201.08054"  
}
