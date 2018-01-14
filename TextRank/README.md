# TextRank를 이용한 문서요약
자세한 내용은 블로그 [excelsior-cjh.tistory.com/TextRank를 이용한 문서요약](http://excelsior-cjh.tistory.com/entry/TextRank%EB%A5%BC-%EC%9D%B4%EC%9A%A9%ED%95%9C-%EB%AC%B8%EC%84%9C%EC%9A%94%EC%95%BD?category=918734)를 참고

### 목적

* 인터넷 뉴스 기사 및 내용이 긴 텍스트를 핵심 내용을 요약하기 위해 프로젝트를 진행
* 사용자가 검색한 문서들의 내용을 요약하여 빠르게 검토할 수 있도록 서비스를 제공하고자 함

### 내용

* TextRank 알고리즘을 이용한 중요 문장 추출(요약) 및 키워드 추출

1. **자연어처리(NLP)** : 텍스트 내 문장 분리 후 명사 추출
2. **TF-IDF 모델링** : 단어의 가중치 계산 후 TF-IDF Matrix 생성
3. **그래프 생성**: TF-IDF Matrix를 통해 Adjacency Matrix 생성
4. **TextRank 적용**: TextRank 를 계산하여 높은 순으로 문장 정렬

### 참고문헌

* 홍진표, 차정원. "TextRank 알고리즘을 이용한 한국어 중요 문장 추출." 한국정보과학회 학술발표논문집, 36.1C (2009.6): 311-314. 
* Page, Lawrence, et al. The PageRank citation ranking: Bringing order to the web. Stanford InfoLab, 1999. 
* Mihalcea, Rada, and Paul Tarau. "TextRank: Bringing order into texts." Association for Computational Linguistics, 2004. 
* LIN, Chin-Yew. Rouge: A package for automatic evaluation of summaries. In: Text summarization branches out: Proceedings of the ACL-04 workshop. 2004. 
* 파이썬 한글 형태소 분석기 패키지 KoNLPy - http://konlpy-ko.readthedocs.io/ko/v0.4.3/ 
* Twitter 형태소 분석기 - https://github.com/twitter/twitter-korean-text 