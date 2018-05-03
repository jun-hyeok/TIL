#Structed Types
## List


## Tuples
변경 불가능한 리스트 -> 수정,추가,삭제 불가

~~~
score = (80, 70, 90, 60)
print (score) #(80, 70, 90, 60)
print (score[1]) #70
a,b,c,d = score #튜플의 대입연산
~~~

## Dictionaries
**키**와 **값**으로 구성된 비순차적 데이터 집합

키로 검색하며, **index에 접근이 불가능**함.

~~~
dic = {2015200:"Bob", 2015123:"Alice","KMU":"JeongReung"}
dic[2015400]="Carole"
dic.update({20181705:"HaJunHyeok"})
print(dic) 

result : {2015200:"Bob", 2015123:"Alice","KMU":"JeongReung",2015400:"Carole",20181705:"HaJunHyeok"}

#사전 전체 검색 방법
for key in dic :
for key,value in dic.items():

#키 존재 확인
<key> in <dic> : <key> 가 <dic>에 있다면 True, 없으면 False
<dic>.get(<key>) : <key> 가 <dic>에 있다면 <키>의 <값>을 리턴. 없으면 None을 리턴.

#삭제
del <dic> <key> : <key>를 <dic>에서 찾은 다음 <dic>에서 제거한다.
<dic>.pop(<key>) : <key>를 <dic>에서 찾은 항목을 반환한 다음 제거한다.
~~~

## Sets
유일한 값들로 구성된 비순차적 자료구조

수학에서의 집합

~~~
A = {'a','b','c',1,2}
B = {'a','c','d',3,4}
print(A|B) # 합집합 -> {1,2,3,4,'a','b','c','d'}
print(A&B) # 교집합 -> {'a','c'}
print(A-B) # 차집합 -> {1,2,'b'}
print(A^B) # 대칭차집합 -> {'d', 1, 2, 3, 4, 'b'}

#원소 추가
<집합>.add(<원소>) # <집합>에 <원소>를 넣는다.
<집합>.update([<원소>,<원소>],...)  # <집합>에 <원소> 리스트를 넣는다.

#원소 삭제
<집합>.discard(<원소>) # <원소>가 <집합>에 있으면 삭제한다.
<집합>.remove(<원소>) # <원소>가 <집합>에 있으면 삭제하고, 없으면 에러를 발생시킨다.
~~~