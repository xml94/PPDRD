# PPDRD
**New contribution is encouraged and appreciated.**

**Collect public plant disease recognition datasets.**

This project aims to **only** collect the public dataset to recognize plant disease because the community can not
verify the performance on the private ones, although they have information and contributions.

* For every dataset, a file is linked to give more description.
* Dataset name: we will give a name if a dataset has no name. Default is fully public and PartPublic means partially public.
* Crop: show the crop if only one or give the number of crops, otherwise.
* Number of classes: include diseased classes and healthy if having.
* Number of images: **Only** those images with public labels are counted, and **only** the original images are counted (augmented images are not).
* Image background: complex (cmpx), medium (med), simple (simp).
* Machine learning (ML) task: image classification (clf), object detection (obj), segmentation (seg).
* Performance (PE): official leaderboard for challenges, or reported results in the dataset publication.
* Reference: default is with publications or official challenges such as in kaggle; otherwise no reference ![](https://img.shields.io/badge/-NoRef-grey).


| Dataset name                                 | Crop      | Class |  Image | Image BG     | ML task & PE     |
|----------------------------------------------|:----------|------:|-------:|:-------------|:-----------------|
| [Apple2020][Apple2020]                       | Apple     |     4 |  1,821 | med          | clf: 0.984 AUROC |
| [Apple2021][Apple2021]                       | Apple     |     6 | 18,632 | med          | clf: 0.883 F1    |
| [PCApple2023][PCApple2023]                   | Apple     |     9 | 10,212 | med+sim      | clf: N.A         |
| [ASDID][ASDID]                               | Soybean   |     8 |  9,648 | med+sim      | clf: 0.968 Acc   |
| [BRACOL][BRACOL]                             | Coffee    |     5 |  1,747 | sim          | clf: 0.956 Acc   |
| [RoCoLe][RoCoLe]                             | Coffee    |     6 |  1,560 | med          | clf: N.A         |
| [iCassava][iCassava]                         | Cassava   |     5 |  5,656 | med          | clf: 0.939 Acc   |
| [CLDCMakerere][CLDCMakerere]                 | Cassava   |     5 | 21,397 | cmpx+med     | clf: 0.913 Acc   |
| [CLDCAmanda][CLDCAmanda]                     | Cassava   |     6 |  2,249 | med          | clf: 0.930 Acc   |
| [CLDD][CLDD]                                 | Cassava   |     3 |    228 | med          | clf: N.A         |
| [CDRD][CDRD]                                 | Cucumber  |     8 |  1,289 | med+sim      | clf: N.A         |
| [CucumberNegm][CucumberNegm]                 | Cucumber  |     2 |    691 | med          | clf: N.A         |
| [PaddyDoctor][PaddyDoctor]                   | Rice      |    10 | 10,407 | cmpx         | clf: 0.990 Acc   |
| [Rice1426][Rice1426]                         | Rice      |     9 |  1,426 | cmpx+med+sim | clf: 0.971 Acc   |
| [Rice5932][Rice5932]                         | Rice      |     4 |  5,932 | med          | clf: 0.984 Acc   |
| [HuyDoRice][HuyDoRice]                       | Rice      |     4 |  3,355 | sim          | clf: 0.984 Acc   |
| [DhanShomadhan](DhanShomadhan)               | Rice      |     5 |  1,106 | cmpx+sim     | clf: N.A         |
| [WheatLong][WheatLong]                       | Wheat     |     5 |    999 | cmpx         | clf: 0.971 Acc   |
| [WheatLeafDataset][WheatLeafDataset]         | Wheat     |     3 |    407 | med+sim      | clf: N.A         |
| [GroundNutLeaf][GroundNutLeaf]               | Groundnut |     5 |  3,058 | med          | clf: N.A         |
| [MaizeCraze][MaizeCraze]                     | Corn      |     6 |  2,355 | sim          | clf: N.A         |
| [BisqueCorn][BisqueCorn]                     | Corn      |     2 |  1,785 | cmpx         | clf: N.A         |
| [CornNLB][CornNLB]                           | Corn      |     1 | 18,222 | cmpx         | clf: N.A         |
| [iBean][iBean]                               | Bean      |     3 |  1,296 | med          | clf: N.A         |
| [SoybeanMignoni][SoybeanMignoni]             | Soybean   |     3 |  6,410 | cmpx         | clf: N.A         |
| [TaiwanTomato][TaiwanTomato]                 | Tomato    |     6 |    622 | med+sim      | clf: N.A         |
| [GLFD][GLFD]                                 | Guava     |     5 |    527 | sim          | clf: N.A         |
| [IDADP][IDADP]                               | Grape     |     7 |  3,596 | cmpx         | clf: N.A         |
| [CitrusRauf][CitrusRauf]                     | Citrus    |    10 |    759 | sim          | clf: N.A         |
| [PlantVillage][PlantVillage]                 | 14        |    38 | 54,305 | sim          | clf: N.A         |
| [FieldPV][FieldPV]                           | 14        |    38 |    665 | med+sim      | clf: 0.720 Acc   |
| [PlantDocCls][PlantDocCls]                   | 13        |    27 |  2,598 | cmpx+med+sim | clf: N.A         |
| [PlantConservation][PlantConservation]       | 12        |    10 |  4,503 | sim          | clf: N.A         |
| [CCMT][CCMT]                                 | 4         |    22 | 24,881 | med+sim      | clf: N.A         |
| [PDD271][PDD271]                             | N.A       |   271 |  2,710 | cmpx+med     | clf: 0.855 Acc   |
| [PlantDocObj][PlantDocCls]                   | 13        |    27 |  2,598 | cmpx+med+sim | obj: N.A         |
| [NZDLPlantDiseaseV1][NZDLPlantDiseaseV1]     | 5         |    20 |  3,337 | med          | obj: 0.745 mAP   |
| [NZDLPlantDiseaseV2][NZDLPlantDiseaseV2]     | 8         |    28 |  3,039 | med          | obj: 0.932 mAP   |
| [FieldPlant][FieldPlant]                     | 4         |    31 |  5,156 | cmpx+med     | obj: 0.144 mAP   |
| [GrapevineDiseaseMalo][GrapevineDiseaseMalo] | Grape     |     3 |    744 | cmpx         | obj: N.A         |
| [GrapevineDiseaseMalo][GrapevineDiseaseMalo] | Grape     |     4 |    128 | cmpx         | seg: N.A         |
| [RoCoLe][RoCoLe]                             | Coffee    |     2 |  1,560 | sim          | seg: N.A         |
| [ATLDSD][ATLDSD]                             | Apple     |     5 |  1,641 | med+sim      | seg: N.A         |

[//]: # (|                                              |           |       |        |              |                  |)



[Apple2020]: https://github.com/xml94/PPDRD/tree/main/data/Apple2020.md
[Apple2021]: https://github.com/xml94/PPDRD/tree/main/data/Apple2021.md
[ASDID]: https://github.com/xml94/PPDRD/tree/main/data/ASDID.md
[BRACOL]: https://github.com/xml94/PPDRD/tree/main/data/BRACOL.md
[PCApple2023]: https://github.com/xml94/PPDRD/tree/main/data/PCApple2023.md
[CLDCMakerere]: https://github.com/xml94/PPDRD/tree/main/data/CLDCMakerere.md
[CDRD]: https://github.com/xml94/PPDRD/tree/main/data/CDRD.md
[DhanShomadhan]: https://github.com/xml94/PPDRD/tree/main/data/DhanShomadhan.md
[IndonesiaRice240]: https://github.com/xml94/PPDRD/tree/main/data/IndonesiaRice240.md
[PaddyDoctor]: https://github.com/xml94/PPDRD/tree/main/data/PaddyDoctor.md
[Rice1426]: https://github.com/xml94/PPDRD/tree/main/data/Rice1426.md
[Rice5932]: https://github.com/xml94/PPDRD/tree/main/data/Rice5932.md
[WheatLong]: https://github.com/xml94/PPDRD/tree/main/data/WheatLong.md
[DhanShomadhan]: https://github.com/xml94/PPDRD/tree/main/data/DhanShomadhan.md
[MaizeCraze]: https://github.com/xml94/PPDRD/tree/main/data/MaizeCraze.md
[iCassava]: https://github.com/xml94/PPDRD/tree/main/data/iCassava.md
[PlantVillage]: https://github.com/xml94/PPDRD/tree/main/data/PlantVillage.md
[PlantConservation]: https://github.com/xml94/PPDRD/tree/main/data/PlantConservation.md
[CCMT]: https://github.com/xml94/PPDRD/tree/main/data/CCMT.md
[PlantDocCls]: https://github.com/xml94/PPDRD/tree/main/data/PlantDoc.md
[FieldPV]: https://github.com/xml94/PPDRD/tree/main/data/FieldPV.md
[GroundNutLeaf]: https://github.com/xml94/PPDRD/tree/main/data/GroundNutLeaf.md
[CLDD]: https://github.com/xml94/PPDRD/tree/main/data/CLDD.md
[CLDCAmanda]: https://github.com/xml94/PPDRD/tree/main/data/CLDCAmanda.md
[HuyDoRice]: https://github.com/xml94/PPDRD/tree/main/data/HuyDoRice.md
[iBean]: https://github.com/xml94/PPDRD/tree/main/data/iBean.md
[BisqueCorn]: https://github.com/xml94/PPDRD/tree/main/data/BisqueCorn.md
[RoCoLe]: https://github.com/xml94/PPDRD/tree/main/data/RoCoLe.md
[WheatLeafDataset]: https://github.com/xml94/PPDRD/tree/main/data/WheatLeafDataset.md
[TaiwanTomato]: https://github.com/xml94/PPDRD/tree/main/data/TaiwanTomato.md
[SoybeanMignoni]: https://github.com/xml94/PPDRD/tree/main/data/SoybeanMignoni.md
[GLFD]: https://github.com/xml94/PPDRD/tree/main/data/GLFD.md
[GFLDRauf]: https://github.com/xml94/PPDRD/tree/main/data/GFLDRauf.md
[CucumberNegm]: https://github.com/xml94/PPDRD/tree/main/data/CucumberNegm.md
[CitrusRauf]: https://github.com/xml94/PPDRD/tree/main/data/CitrusRauf.md
[ATLDSD]: https://github.com/xml94/PPDRD/tree/main/data/ATLDSD.md
[CornNLB]: https://github.com/xml94/PPDRD/tree/main/data/CornNLB.md
[PDD271]: https://github.com/xml94/PPDRD/tree/main/data/PDD271.md
[IDADP]: https://github.com/xml94/PPDRD/tree/main/data/IDADP.md
[NZDLPlantDiseaseV1]: https://github.com/xml94/PPDRD/tree/main/data/NZDLPlantDiseaseV1.md
[NZDLPlantDiseaseV2]: https://github.com/xml94/PPDRD/tree/main/data/NZDLPlantDiseaseV2.md
[FieldPlant]: https://github.com/xml94/PPDRD/tree/main/data/FieldPlant.md
[GrapevineDiseaseMalo]: https://github.com/xml94/PPDRD/tree/main/data/GrapevineDiseaseMalo.md


# Reference
Please consider cite our related papers if you think this project is useful.
```angular2html
@article{xu2023plant,
  title={Plant Disease Recognition Datasets in the Age of Deep Learning: Challenges and Opportunities},
  author={Xu, Mingle and Park, Ji Eun and Lee, Jaehwan and Yang, Jucheng and Yoon, Sook},
  journal={arXiv preprint arXiv:2312.07905},
  year={2023}
}
@article{meng2023known,
  title={Known and unknown class recognition on plant species and diseases},
  author={Meng, Yao and Xu, Mingle and Kim, Hyongsuk and Yoon, Sook and Jeong, Yongchae and Park, Dong Sun},
  journal={Computers and Electronics in Agriculture},
  volume={215},
  pages={108408},
  year={2023},
  publisher={Elsevier}
}
@article{xu2023embracing,
  title={Embracing limited and imperfect training datasets: opportunities and challenges in plant disease recognition using deep learning},
  author={Xu, Mingle and Kim, Hyongsuk and Yang, Jucheng and Fuentes, Alvaro and Meng, Yao and Yoon, Sook and Kim, Taehyun and Park, Dong Sun},
  journal={Frontiers in Plant Science},
  volume={14},
  year={2023},
  publisher={Frontiers Media SA}
}
@article{xu2022transfer,
  title={Transfer learning for versatile plant disease recognition with limited data},
  author={Xu, Mingle and Yoon, Sook and Jeong, Yongchae and Park, Dong Sun},
  journal={Frontiers in Plant Science},
  volume={13},
  pages={1010981},
  year={2022},
  publisher={Frontiers}
}
```