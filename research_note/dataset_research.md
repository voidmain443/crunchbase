# crunchbase data research papers 

그냥 현상을 나타내는 특성을 보일필요가 있는 것이 아니라. 
어떤 특성이 그 그룹의 요인들을 드러나게 하느냐 , 혹은 그 지점이 어디인지를 발견하는 것이나 사회과학의 특성은 이를 가치 value ladan 한 성질때문에 투자라는 성질을 어떻게 바라보았느냐 그리고 스타트업을기존 시장관느어떻게 다르게 보이는지에 대해서 혹으 ㄴ그 연결고리에 대해서 중점을 맞춰야할 필요가 있다. 

social network theory에서 자주 인용되는 부분인 social network 의 Weak tie와 Strong tie 에 대한 Granovetter의 주장인 weak tie의 의미의 중요성은 어떻게 투자자들 사이에서 나타나는가 ?

이미 아는 사람들인 같이 공부했던 사람들이 아닌 얼마나 시간에 지나며 멀어졌을떄 혹은 다른 분야의 사람이 인접하였을때 같은기업에 투자할 확률로 표현 할 수 있을 것인가 ? 
strong tie가 내부의 정보들을 빠르게 효율적으로공유한다면  weak Tie는 외부의 네트워크의 정보를 가져올 수 있다는 점이다. 사회적으로 힘이 강한 네트워크가 있다면 외부의 weak tie들의 연결이 그들의 행동 반경을 좁힐 수 있다는 것도 이론이다. 

small world network와 sacle free network 전부 hub 같은 노드를 가정하고 밝혔다. Connector로의 성격 을 가지는 weak tie로 볼 수 있으며 , 이 weak tie들이 어떠한 역할 을 수행할지 가 중요한 사회과학과는 다르게 이 weak tie가 네트워크 내에서 어떤 성질을 가지는 지 알아내는 것이 중요하지 않을까 싶다. 

시장을 아예 고전적 방법으로 바라보고 있는것은 아닐까 ? 
네트워크에서 본다면  기업의 발달에 있어 기업의 내부인이 초기멤버들의 strong tie가 어떠한 투자를 받을 것이라는 기대 혹은 노력이 어떤 phenomena 를 가져오는데 이것이 투자고 , 그 투자의 deposit 의 상한 과 하한이 그 기업이 이후에 연속사업을 할 수 있도록하는 것이 아닐까 ? 혹은 한번의 장사로만 끝낼 수 있는 사람들이 만들수 도 있기 때문에 어떤 아이디어를 실현하기 위해서 노력했을때 그 시도를위해  투자라는 보험을 들어두는 것일 수도 있다. 따라 이 투자를어떻게 받는지를 투자자의 community를 나눠볼수도 있고 , 아니라면 투자자들의 네투워크를 뚫는 것이 Network pressure로 시장에 의미없는 기업들을 솎아내는 refer check가 아닐까 ? 
네트워크가 그냥 이어지고 하는 것이 아니라 다른 네트워크가 하방과 상방에서의 압박을 가해 그 구조가 생성하되는 것이 아닌가 ? 사회의 규범으로 학생 때 부터 성인까지 그 규범을 지키는 것처럼 만약 그 규범을 지키지 않으면 ,그 규범들이 의미가 없어지기 때문에 (가치관) 이 달라지는 지점들로 향하는 것일수도 있다. 

기업의 발달과정을 알 수는 없다. 
스타트업의 성공과 실패에 대한 연구들은 있지만  스타트업에서 우리는 무엇을 보아야할까 네트워크 적으로 ? 통계 물리학적 관점을 유지할 수 있는걸까 ? 시장 자체가 그냥 무작위라면 ?

### reference 
Granovetter 1973 the strength of weak ties 미국사회학회   
Garton  Haythornthwaite Wellman 1997 Studing online social networks   
Turner JW , 2001 Developing an optimal match within online communities : an exploration of CMC support communities  and traditional support . 








|                            Study                             |                  Data Source                  |                            Sample                            |                    Outcomes (% Frequency)                    |                    # Predictive Variables                    |                       Methods Employed                       |
| :----------------------------------------------------------: | :-------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
| [Zbikowski and Antosiuk](https://www.mdpi.com/2227-7099/11/1/19#B31-economies-11-00019)([2021](https://www.mdpi.com/2227-7099/11/1/19#B31-economies-11-00019)) |                  Crunchbase                   |       213,171 ventures founded between 1995 and 2015.        |      ‘M&A, IPO or operating’ (12.2%); ‘closed’ (87.8%).      |       9 (only information known before funding rounds)       | Logistic regression, support vector machines, gradient boosted trees. |
| [Ferrati et al.](https://www.mdpi.com/2227-7099/11/1/19#B11-economies-11-00019)([2021](https://www.mdpi.com/2227-7099/11/1/19#B11-economies-11-00019)) |                  Crunchbase                   | 10,211 ventures located in USA and founded between 2000 and 2018. |     ‘M&A or IPO’ (37.5%); ‘operating or closed’ (62.5%).     | 15 (measures repeated for each of the first 10 years of life) |                       Neural networks.                       |
| [Shi et al.](https://www.mdpi.com/2227-7099/11/1/19#B25-economies-11-00019)([2020](https://www.mdpi.com/2227-7099/11/1/19#B25-economies-11-00019)) |           Crunchbase 2013 Snapshot            | 24,965 ventures located in the ten countries with most funds (foundation date not specified). | ‘operating’ (18.9%), ‘M&A’ (21.4%), ‘IPO’ (37.4%), ‘closed’ (22.2%). |                     Details not provided                     | Logistic regression, k-NN, naive Bayes, random forests, gradient boosted trees. |
| [Arroyo et al.](https://www.mdpi.com/2227-7099/11/1/19#B2-economies-11-00019)([2019](https://www.mdpi.com/2227-7099/11/1/19#B2-economies-11-00019)) |                  Crunchbase                   |       120,507 ventures founded between 2011 and 2015.        | ‘closed’ (0.6%), ‘M&A’ (2.7%), ‘at least one funding round’ (18.0%), ‘IPO’ (0.1%), ‘no funding rounds’ (78.6%). |     105 (referred to a 3-year window from 2015 to 2018)      | Support vector machines, random forests, extremely randomized trees, gradient boosted trees. |
| [Bento](https://www.mdpi.com/2227-7099/11/1/19#B3-economies-11-00019)([2018](https://www.mdpi.com/2227-7099/11/1/19#B3-economies-11-00019)) |                  Crunchbase                   | 86,588 ventures located in USA and founded between 1985 and 2017. |     ‘M&A or IPO’ (15.8%), ‘operating or closed’ (84.2%).     |                             158                              | Logistic regression, support vector machines, random forests. |
| [Krishna et al.](https://www.mdpi.com/2227-7099/11/1/19#B14-economies-11-00019) ([2016](https://www.mdpi.com/2227-7099/11/1/19#B14-economies-11-00019)) |                  Crunchbase                   |        11,000 ventures founded between 1999 and 2014.        |      ‘operating’ (9.4%), ‘M&A, IPO or closed’ (90.6%).       |                              13                              | Logistic regression, k-NN, naive Bayes, random forests, alternating decision trees, Bayesian networks. |
| [Xiang et al.](https://www.mdpi.com/2227-7099/11/1/19#B30-economies-11-00019)([2012](https://www.mdpi.com/2227-7099/11/1/19#B30-economies-11-00019)) | Crunchbase + TechCrunch (top words in topics) |        59,631 ventures founded between 1970 and 2012.        |      ‘M&A’ (9.4%), ‘IPO, operating or closed’ (90.6%).       |                              22                              |        Logistic regression, support vector machines.         |