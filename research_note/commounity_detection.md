# community detection 

- referecne by Wonguk Cho M.S thesis 

- a comprehensive literature review on community detection : approaches and applications 
https://www.sciencedirect.com/science/article/pii/S1877050919305046

keyword : Community detection Inconsistency 

modularity가 높은 집단을 community라고 부릅니다. 


### Louvain algorithm

2008년도에 나온 Louvain 알고리즘을 사용할 수 있다. 보통 network community를 찾는 방법은 modularity를 찾는 방법을 많이 이용하게 되는데 이 방법은 계산시간이 길다는 단점이 존재합니다. 기존의 metwork modularity는 

$$ Q = \frac{1}{2m} \Sigma_{i,j} \biggr[ A_{ij} - \frac{k_{i}k_{j}}{2m}\Biggr] \delta(c_i,c_j)  $$

와 같이 계산됩니다. 
각 기호에 있어서는 

- $A_{ij}$ : i 와 j의 weight of the edge (연결)
- $k_i$ : 꼭지점 i 에 포함된 edgesdml weight 의 합 (i 가 지니는 링크의 개수)
- $C_i$ : vetex i가 해당하는 커뮤니티 
- $\delta (c_i,c_j)$ : 둘이 같으면 1 아니면 0인 것 
- m : 전체 링크의 개수 

기존의 모듈성에 대한 방법은 계산은 시간이 오래걸려 최적화 하는 방안이 필요하다. 
대규모 커뮤니티니는 자연적으로 커뮤니티 하위 커뮤니티로 나뉘어져 계층적 구조가 드러납니다. 이때 효과적인 modularity를 이용하기 위해서는 


 한 node의 원래의 community에서 빼내어서 다른 인접한 community에 재배치를 하고 이때 modulartiy를 측정합니다.   
 만약 이떄 modularity 가 커지는 community가 있으면 해당노드는 그  community에 속하기 된다.  
 modularity변화량 : 노드 i 가 community에 배속된 상태 modularity - i가 배속되지 않은상태의 modularity 

 $$ \Delta Q  = \Biggr[\frac{\Sigma_{in} + 2k_{i,in}}{2m} - \Biggr( \frac{\Sigma{tot} + k_i}{2m}\Biggr)^2  \Biggr] - \Biggr[ \frac{\Sigma_{in}}{2m} - \Biggr(\frac{\Sigma_{tot}}{2m} \Biggr)^2 -\Biggr(\frac{k_i}{2m} \Biggr)   \Biggr]$$

위 수식에 대해서는 
 - $\Sigma_{in}$ : C 의 내부 링크 weight의 합 
 - $\Sigma_{tot}$ : C 에서 발생한 모든 연결의 weight들의 합 
 - $k_i$ : node i에서 발생한 link의 weight의 합
 - $k_{i,in}$ : C에서 i에서 Node로 연결되는 weight의 합 
 - $m$ : 모든 link의 weight 합 

따라서 이 모듈성의 변화가 positive하면 해당 community로 이동하고 , negative 면 기존 community에 머무르게 한다. 

위 단계는 개선의 여지가 없을떄까지 반복합니다. 

이후 우리는 위의 단계에서 보인 community를 가지고 새로운 community를 구축합니다.  
새로운 노드들 사이의 weight of the links 는 두 커뮤니티 node 들 사이의 link weight의 합으로 계산됩니다.  
동일한 커뮤니티의 node 들 간의 link는 sef loop로 대체하고 이것이 끝나면 다시 위의 수식으로 돌아가 개선을 시작합니다. 
이 두 단계를 합쳐 pass라고 명명합니다. 

논문에서는 무역 데이터에 있어서 

alternative inconsistency problem ?

sleeping beauty measure ? 
https://www.pnas.org/doi/epdf/10.1073/pnas.1424329112
