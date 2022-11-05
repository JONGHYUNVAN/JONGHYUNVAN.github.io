---
title: 객체
keywords: sample
summary: "This is just a sample topic..."
sidebar: product1_sidebar
permalink: p1_sample3.html
folder: product1
---

## 객체가 뭔데 ? 

이제 객체에 대해 좀 더 자세히 알아보자.    
클래스 설명할때 예로 든 김에 자동차의 예를 한번 더 들자면, 자동차에서 제일 핵심적인 일 하는 친구, 바퀴를 살펴보자.   
바퀴를 가장 간단하게 설명하면 '동그랗고, 굴러가는거' 라고 설명할 수 있겠다.   
이때 '동그랗다'는 바퀴가 가진 속성이라 할 수 있고, '굴러간다'는 바퀴의 기능이라 할 수 있는데, 이걸 컴퓨터가 인식하는 입장에서 보면 동그란건 바퀴의 필드(field), 굴러가는건 바퀴의 메소드(method)라 볼 수 있다.   
자바식 언어로 예를들면    
String shapeofwheels == "동그라미";   
int numberofwheels == 4;   
이런식으로 정의되는게 필드고   
void daegooldaegool()   
이런식으로 정의되는게 메소드다.   
항상 제일 위에 있는 String void가 뭘 의미히는지도 알면 좋다.



## 객체 생성

new 를 쓴다.   
예를들어
<pre>
<code>
1 Class 참조변수 = new 생성자();
</code>
</pre>
이 코드를 과정별로 쪼개면
<pre>
<code>
1 Class 참조변수;
2 참조변수 = new 생성자();
</code>
</pre>
이 코드를 읽고 컴퓨터는       
1번에서 Class 타입의 참조변수를 선언하고,   
2번에서 생성자를 통해 인스턴스를 생성하여 참조변수에 할당한다.   
참조 변수는 쉽게말해 '어디있는 정보인가?'를 가리키는 변수다.   
그럼 정보는 어디있나? 의문이 생기는데 데이터는 '힙(heap) 메모리'라는데 쓰인다.  
힙 메모리는 CPU가 자동으로 필요한만큼 할당하고 해제하는 영역이다.  
그렇다면 나머지들은 어디 저장되냐?   
Class는 클래스 영역, 참조변수는 스택 영역에 저장된다.   
어디 저장하는지가 왜 중요한가?   
어떤 객체/값이 어디까지 적용되는지가 결정되기 때문이다.

## 사용예시
<pre>
<code>
public class Periodic table {
    public static void main(String[] args) {
         element Hydrogen = new Hydrogen(1, 1, 1); // 객체 생성. 

        System.out.println("Hydrogen is " + Hydrogen.family + "족이고 " + "원자번호는 " + Hydrogen.atomicnumber + "입니다."); // 필드 호출
        Hydrogen.numberofprotons(); // 메서드 호출
        Hydrogen.numberofelectrons();
        Hydrogen.Valenceelectron();
    }
}

class Hydrogen {
    public int numberofprotons; // 필드 선언
    public int numberofelectrons;

    public Hydrogen(int numberofprotons, int numberofelectrons) {
        this.numberofprotons = 1;
        this.numberofelectrons = 1;
    }

    void numberofprotons() { // 메서드 선언
        System.out.println(numberofprotons+"개의 양성자가 있습니다.");
    }

    void numberofelectrons() {
        System.out.println(numberofelectrons+"개의 전자가 있습니다.");
    }

    void Valenceelectron(){
        int VE=numberofelectrons;
        while(VE>5){VE-=8}
        System.out.println(VE+"개의 최외각전자가 있습니다.");
    }
}

</code>
</pre>
{% include links.html %}
