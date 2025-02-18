---
layout: default
title: korean_parallel_corpora
---

# korean_parallel_corpora
{: .no_toc }

Korean Parallel corpora (of https://sites.google.com/site/koreanparalleldata/)

Jungyeul Park, Jeen-Pyo Hong and Jeong-Won Cha (2016) Korean Language Resources for Everyone. In Proceedings of the 30th Pacific Asia Conference on Language, Information and Computation (PACLIC 30). October 28 - 30, 2016. Seoul, Korea. https://www.aclweb.org/anthology/Y16-2002/

For more details, see <https://sites.google.com/site/koreanparalleldata/> and <https://github.com/jungyeul/korean-parallel-corpora>.

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Dataset Informations

* [See codes in GitHub](https://github.com/jeongukjae/tfds-korean/blob/main/tfds_korean/korean_parallel_corpora/korean_parallel_corpora.py)
* Version:
* Homepage: <https://github.com/jungyeul/korean-parallel-corpora>
* Citation:

  ```text
  @inproceedings{park-etal-2017-building,
      title = "Building a Better Bitext for Structurally Different Languages through Self-training",
      author = {Park, Jungyeul  and
        Dugast, Lo{\"\i}c  and
        Hong, Jeen-Pyo  and
        Shin, Chang-Uk  and
        Cha, Jeong-Won},
      booktitle = "Proceedings of the First Workshop on Curation and Applications of Parallel and Comparable Corpora",
      month = nov,
      year = "2017",
      address = "Taipei, Taiwan",
      publisher = "Asian Federation of Natural Language Processing",
      url = "https://www.aclweb.org/anthology/W17-5601",
      pages = "1--10",
      abstract = "We propose a novel method to bootstrap the construction of parallel corpora for new pairs of structurally different languages. We do so by combining the use of a pivot language and self-training. A pivot language enables the use of existing translation models to bootstrap the alignment and a self-training procedure enables to achieve better alignment, both at the document and sentence level. We also propose several evaluation methods for the resulting alignment.",
  }
  ```

## Configs


### korean_parallel_corpora/news-v1 (default)

None

* Dataset size: `28.08 MiB`
* Download size: `8.64 MiB`
* Features:

  ```python
  FeaturesDict({
      'en': Text(shape=(), dtype=tf.string),
      'ko': Text(shape=(), dtype=tf.string),
  })
  ```

* Splits:

  | Split Name | Num Examples        |
  |------------|--------------------:|
  |train  |94123|
  |dev  |1000|
  |test  |2000|

* Examples:

  | |ko|en|
  |---|---|---|
  |1|최근 해리포터 팬사이트에는 작가의 마음을 상하게 할 말한 여러 통의 메일이 전달된 것...|The author's comments came in response to an Ap...|
  |2|이후 론스타는 외환은행을 회복시켰고, 2년간 지분판매금지가 만료된 지난 2005년10...|Lone Star turned the bank around, and began loo...|
  |3|빙판길로 교통사고로 미시건주에서 2명, 위스콘신주에서 1명이 사망했다.|Slippery roads were blamed for two traffic deat...|
  |4|원문기사보기|"Now, come, travel back in time.|
  |5|[동영상]추신수 스리런 홈런 작렬!|Korea to double African aid by ...|
  |6|미국은 지난 2003년 이라크전 이래 소수의 난민만을 받아들여 비난받았다.|The United States has been criticized for accep...|
  |7|콜롬비아 보고타 학생들이 성조기를 태우며 오는 부시 미 대통령 방문에 반대하는 시위를...|Clashes between police and anti-Bush protesters...|
  |8|보건복지부에따르면 현재 기금 규모는 약 121조원이나 2010년에는 242조원, 20...|The pension fund amounts to about 121 trillion ...|
  |9|커넥티컷, 델라웨어, 메인, 메릴랜드, 메사츄세츠, 뉴햄프셔, 뉴저지, 뉴욕, 펜실바...|The governors of Connecticut, Delaware, Maine, ...|
  |10|그런가 하면 남북관계에 관한 어떠한 진보도 올 12월 19일에 치러질 대통령 선거에 ...|He said any progress in inter-Korean relations ...|

* Use this dataset

  ```python
  import tensorflow_datasets as tfds
  import tfds_korean.korean_parallel_corpora
  # Install tfds-korean with `pip install tfds-korean`

  dataset = tfds.load("korean_parallel_corpora/news-v1")
  ```


### korean_parallel_corpora/jhe-v1 

None

* Dataset size: `235.28 KiB`
* Download size: `154.27 KiB`
* Features:

  ```python
  FeaturesDict({
      'en': Text(shape=(), dtype=tf.string),
      'ko': Text(shape=(), dtype=tf.string),
  })
  ```

* Splits:

  | Split Name | Num Examples        |
  |------------|--------------------:|
  |dev  |720|
  |eval  |720|

* Examples:

  | |ko|en|
  |---|---|---|
  |1|그것 역시 나쁜 습관이다.|That is a bad habit, too.|
  |2|그러나 Lincoln은 “우리의 아이들은 전쟁터에서 싸우고 있지만, 우리는 그들을 도...|But Mr. Lincoln said, "Our boys are fighting in...|
  |3|그렇다면 내가 당신에게 특수 비료를 좀 주리다."|Then, I'll give you some special fertilizer."|
  |4|만약 당신이 매력적인 피부로의 회복을 굼꾸는 수백만 여성중에 속한다면, “Recove...|If you're among millions of women who dream of ...|
  |5|사람들이 비타민 C를 너무 많이 구입해서, 곧 구하기가 어려워질 정도였다.|People bought so much Vitamin C that it soon be...|
  |6|대부분의 쥬스용 오렌지는 Florida에서 재배된다.|Most of the oranges for juice grow in Florida.|
  |7|그 공원은 한강 옆에 있다.|The park is by the Han River.|
  |8|수미의 친구, 톰은 내일 미국에서 한국으로 올 것이다.|Su-mi's friend, Tom will come from America to K...|
  |9|그리고 또한 다른 많은 것들을 할 수 있습니다.|And I can do many other things, too.|
  |10|그녀는 경찰에 체포되었다.|She was arrested by the police.|

* Use this dataset

  ```python
  import tensorflow_datasets as tfds
  import tfds_korean.korean_parallel_corpora
  # Install tfds-korean with `pip install tfds-korean`

  dataset = tfds.load("korean_parallel_corpora/jhe-v1")
  ```


### korean_parallel_corpora/french-jim-v1 

None

* Dataset size: `99.60 KiB`
* Download size: `36.18 KiB`
* Features:

  ```python
  FeaturesDict({
      'fr': Text(shape=(), dtype=tf.string),
      'ko': Text(shape=(), dtype=tf.string),
  })
  ```

* Splits:

  | Split Name | Num Examples        |
  |------------|--------------------:|
  |train  |207|
  |test  |4|

* Examples:

  | |ko|fr|
  |---|---|---|
  |1|뭐가 문제지요? 갖기 싫으면 버리면 되는데? 또 봤어요. 물에서 기어나온 여자 귀신을...|C’est quoi le problème ? Si tu ne le veux pas, ...|
  |2|자랑이냐? 그럼? 말이 좋아 정신대지 내용을 알고 보면...|ieille dame. – Il n'y a pas de quoi se vanter. ...|
  |3|그 편지에 있는 주소로......|À l'adresse indiquée dans la lettre.|
  |4|나쁜 일이야 하셨겠어요? 편지만 감췄을 뿐이겠지요.|Il raille) – Non bien sûr, vous n'avez rien fai...|
  |5|미친 여자라니요?|La folle ?|
  |6|한달동안 배웠다니까... 문제는 팥앙금 내는 건데 내가 아주 잘 배웠거든. 모리나가 ...|J'ai mis un mois à l'apprendre… Le problème c'e...|
  |7|무슨?|. – Laquelle ?|
  |8|어쩌면 우리를 보내주지 않을지도 모른대.|. – Peut-être qu'ils ne nous ramènent pas en Co...|
  |9|할아버지는 오미나토에서도 한참 떨어진 마이츠루만 부근까지 가서 현장을 보고 오다가 아...|Mon grand-père m'a raconté qu’il avait fait tou...|
  |10|아직도 이것이 제 짐이라고 생각하십니까?|Vous pensez encore que ce fardeau est à moi ?|

* Use this dataset

  ```python
  import tensorflow_datasets as tfds
  import tfds_korean.korean_parallel_corpora
  # Install tfds-korean with `pip install tfds-korean`

  dataset = tfds.load("korean_parallel_corpora/french-jim-v1")
  ```


### korean_parallel_corpora/northkorean-news-v1 

None

* Dataset size: `954.30 KiB`
* Download size: `868.05 KiB`
* Features:

  ```python
  FeaturesDict({
      'en': Text(shape=(), dtype=tf.string),
      'nk': Text(shape=(), dtype=tf.string),
  })
  ```

* Splits:

  | Split Name | Num Examples        |
  |------------|--------------------:|
  |dev  |1000|
  |test  |2000|

* Examples:

  | |nk|en|
  |---|---|---|
  |1|이날 뉴욕상업거래소(NYMEX)에서 거래된 8월 인도분 서부텍사스산 중질유(WTI)는...|Light, sweet crude oil for August delivery sett...|
  |2|지난 25일에도 콴타스항공려객기가 기체에 구명이 생겨 필리핀 마닐라에 비상착륙했다.|The incident comes just three days after a Qant...|
  |3|정치적인 라이벌인 이들이 결선투표이후 한자리에 모습을 나타내는것은 이번이 처음이다.|It is the first time the bitter political rival...|
  |4|A U.S. envoy’s ‘ Korea, Japan and China meeting...|U.S. government prosecutors are against bail be...|
  |5|이에앞서 이란국영파스통신은 30명의 사형이 집행될것이라고 보도한바 있다.|Iran's semi-official Fars News Agency reported ...|
  |6|미네소타 미네아폴리스의 I-35W 교각의 일부가 지난 수요일 저녁 퇴근시간대에 붕괴되...|Some 50 vehicles were hurled into the water whe...|
  |7|데이비드 스레이 여론페이지편집장이 매케인 진영에 보낸 이메일에서 매케인의 원고를 받아...|In an e-mail to the McCain campaign, Opinion Pa...|
  |8|CNN이 지난 주말 실시한 여론조사에도 오바마는 이전 조사때보다 매케인과의 격차를 2...|Obama now holds a 6-point lead in CNN's average...|
  |9|현재 광부 400여명이 곰의 습격이 두려워 광산에서 마을로 돌아오지 못하고있다. 이타...|About 400 company workers have refused to retur...|
  |10|제너럴모터스(GM)의 연구원들은 도로에서 일어나는 상황을 실시간으로 알려주는 레이저,...|researchers are working on a windshield that co...|

* Use this dataset

  ```python
  import tensorflow_datasets as tfds
  import tfds_korean.korean_parallel_corpora
  # Install tfds-korean with `pip install tfds-korean`

  dataset = tfds.load("korean_parallel_corpora/northkorean-news-v1")
  ```


### korean_parallel_corpora/bible 

None

* Dataset size: `10.45 MiB`
* Download size: `9.56 MiB`
* Features:

  ```python
  FeaturesDict({
      'en': Text(shape=(), dtype=tf.string),
      'ko': Text(shape=(), dtype=tf.string),
  })
  ```

* Splits:

  | Split Name | Num Examples        |
  |------------|--------------------:|
  |train  |31103|

* Examples:

  | |ko|en|
  |---|---|---|
  |1|Ezekiel46.2  왕은 바깥 마당에서 이 문의 현관으로 들어와서, 문설주 곁에 ...|Ezekiel46.2  The prince is to enter from the ou...|
  |2|Numbers11.18  너는 또 백성에게 이렇게 말하여라. 내일을 맞이하여야 하니,...|Numbers11.18  "Tell the people: 'Consecrate you...|
  |3|Romans4.20  그는 끝내 하나님의 약속을 믿고 의심하지 않았을 뿐만 아니라, ...|Romans4.20  Yet he did not waver through unbeli...|
  |4|2_Chronicles6.29  주의 백성 이스라엘 가운데 어느 한 사람이나 혹은 주...|2_Chronicles6.29  and when a prayer or plea is ...|
  |5|Psalms48.8  우리가 들은 바 그대로, 우리는 만군의 주께서 계신 성, 우리 ...|Psalms48.8  As we have heard, so have we seen i...|
  |6|Jeremiah48.40  "나 주가 이렇게 말한다. 보아라, 적이 독수리처럼 날아와...|Jeremiah48.40  This is what the LORD says: "Loo...|
  |7|Jeremiah2.3  이스라엘은 나 주께 거룩하게 구별된 나의 농산물 가운데서 첫 ...|Jeremiah2.3  Israel was holy to the LORD, the f...|
  |8|2_Chronicles23.7  레위 사람들은 제각기 병기를 들고 왕을 호위하십시오....|2_Chronicles23.7  The Levites are to station th...|
  |9|Exodus16.25  모세가 말하였다. "오늘은 이것을 먹도록 하여라. 오늘은 주의...|Exodus16.25  "Eat it today," Moses said, "becau...|
  |10|Micah4.13  도성 시온아, 너의 원수에게 가서, 그들을 쳐라! 내가 네 뿔을 ...|Micah4.13  "Rise and thresh, O Daughter of Zion...|

* Use this dataset

  ```python
  import tensorflow_datasets as tfds
  import tfds_korean.korean_parallel_corpora
  # Install tfds-korean with `pip install tfds-korean`

  dataset = tfds.load("korean_parallel_corpora/bible")
  ```



## License

Korean Parallel corpora are made available under the terms of the Creative Commons Attribution Noncommercial No-Derivative-Works 3.0 US License.

<style> td {white-space: nowrap;} </style>
