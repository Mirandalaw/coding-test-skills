## *1. string sort*

<hr>

  ```#include<string> 
     #include<algorithm> 
     using namespace std;
     int main(){
      string str1="10";
      string str2="6";
      cout<<(str1<str2); //1반환 
      // 사전 순으로 10이 6보다 앞서 있기 때문에.
      string str3 = str1+str2;  // "106"
      string str4 = str2+str1;  // "610"
      cout<<(str3<str4);        //1반환
      //같은 자릿수로 받아진 정수 형태의 문자열 비교는 단순히 int형처럼 비교해도 무관
    }
```
    
## *example. programmers 가장 큰수 中*
 
 ``` bool cmp(string a,string){
        return a+b > b+a;
     }
 ```
 6, 10 이 있을 때 610, 106 중 더 큰 수 비교
 
 ```vector<string> tmp;
 sort(tmp.begin(),tmp.end(),emp);
 ```
