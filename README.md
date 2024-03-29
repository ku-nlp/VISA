VISA
==========

__VISA__ is a dataset that consists of 40k Japanese-English parallel sentence pairs and corresponding video clips with the following key features: 
  - The parallel sentences are __subtitles__ from movies and TV episodes
  - The source subtitles are __ambiguous__, which means they have multiple possible translations with different meanings
  - We divide the dataset into __Polysemy__ and __Omission__ according to the cause of ambiguity

Examples:
-------------------
Polysemy:  
  
放せ！ --> Let me go!

![let_me_go](https://user-images.githubusercontent.com/38623473/160537899-a5085b99-d3f4-49aa-a5c2-df33c984c2f3.gif)

Omission:  
  
銃を持ってる。 --> I have a gun.

![I_carry_a_gun](https://user-images.githubusercontent.com/38623473/160538132-6e0ab417-41f7-45ca-aef5-c8a540496a69.gif)

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
```
video_file_name: {  
    { "ja": Japanese_subtitle },  
    { "en": English_subtitle }  
}  
```

Note:
-------------------
Please, note that by downloading the dataset, you agree to the following conditions:
  - Do not re-distribute the dataset without our permission.
  - The dataset can only be used for research purposes. Any other use is explicitly prohibited.
<!---  - We do not officially distribute the video clips. Do not disclose this anywhere, even in your paper.--->

Downloadable Features:
-------------------
If you are interested in the video features of VISA, you can download them from the following links:
  - The I3D Features of VISA: http://lotus.kuee.kyoto-u.ac.jp/~yihang/dataset/VISA_i3d.zip
  - The RCNN Features of VISA: http://lotus.kuee.kyoto-u.ac.jp/~yihang/dataset/VISA_rcnn.zip

Citation:
-------------------
If you find this dataset helpful, please cite our publication "[VISA: An Ambiguous Subtitles Dataset for Visual Scene-Aware Machine Translation](https://aclanthology.org/2022.lrec-1.725/)":  

```
@inproceedings{li-etal-2022-visa,
    title = "{VISA}: An Ambiguous Subtitles Dataset for Visual Scene-aware Machine Translation",
    author = "Li, Yihang  and
      Shimizu, Shuichiro  and
      Gu, Weiqi  and
      Chu, Chenhui  and
      Kurohashi, Sadao",
    booktitle = "Proceedings of the Thirteenth Language Resources and Evaluation Conference",
    month = jun,
    year = "2022",
    address = "Marseille, France",
    publisher = "European Language Resources Association",
    url = "https://aclanthology.org/2022.lrec-1.725",
    pages = "6735--6743",
}
```

Contact:
-------------------
If you have any questions about this dataset, please contact liyh@nlp.ist.i.kyoto-u.ac.jp.

License:
-------------------
[GNU General Public License v3.0](LICENSE)
