# 💬 목차

[Array와 LinkedList의 특징과 차이](#array와-linkedlist의-특징과-차이)<br/>
[이진탐색트리(BST)](#이진탐색트리-bst)<br/>
[스택과 큐의 차이](#스택과-큐의-차이)<br/>
[버블정렬](#버블정렬)<br/>
[퀵정렬](#퀵정렬)

## Array와 LinkedList의 특징과 차이

둘 다 데이터를 저장하고 관리하는 자료구조

### Array

- **특정 크기만큼 연속된 메모리 공간에 데이터를 저장하는 구조**
- 인덱스를 통한 빠른 접근 가능
- 삽입 삭제가 대체로 오래 걸림
- 배열 중간의 데이터가 삭제되면 메모리 공간 낭비발생
- 빠른 탐색이 요구되고 데이터의 삽입과 삭제가 적을 때 사용

### LinkedList

- **각각의 데이터가 메모리 공간 상에 고유한 노드로 존재**
- 각 **노드**는 자신의 뒤에 있는 데이터에 대한 **주소를 기억**하고 있는 구조 ( 노드 : 본인의 데이터 + 뒤 데이터의 주소 )
- 임의접근이 불가능하여 처음부터 탐색을 해야함
- 삽입과 삭제 연산이 많고 검색의 빈도가 적을 때 사용

### 차이

두 자료구조 모두 선형자료구조이지만 배열은 물리적 메모리에 연속적으로 존재하기 때문에 인덱스를 통해 빠르게 접근이 가능한 반면에 연결리스트는 물리적인 메모리가 연속적이지 않지만 논리적으로 연결시켜 놓은 형태

배열과 링크드리스트는 데이터를 저장하는 구조가 다를 뿐더러 내부의 데이터에 대한 접근, 삽입, 삭제 속도에서 차이를 나타낸다


# 이진탐색트리 BST
![1](https://user-images.githubusercontent.com/97332044/228278258-4d778bef-6c23-410a-b049-4f33d08da93c.jpg)

## BST( Binary Search Tree )
- 이진 트리(Binary Tree)의 한 종류
- 이진 탐색의 효율성을 높이기 위한 자료구조
- 이진 탐색 : **정렬된 배열**에서 특정한 값을 검색하는 알고리즘

## 필수조건

- 각 노드의 키값은 해당 노드의 왼쪽 서브 트리에 있는 모든 노드의 키 값보다 크거나 같아야 하고 
해당 노드의 오른쪽 서브 트리에 있는 모든 노드의 키 값보다 작거나 같아야 함
- 각 노드는 왼쪽 서브 트리와 오른쪽 서브 트리를 가질 수 있음
- 노드는 중복된 키값을 허용하지 않음

## 특징

- 각 노드는 최대 두 개의 자식 노드를 가질 수 있음
- 정렬된 상태를 유지됨
- 트리의 균형을 유지하는 알고리즘이 사용된다면, 검색 시간이 보장
- 삽입, 삭제, 검색 등의 작업에서 최선 O(1) 평균 O(log n) 최악 O(n)의 시간복잡도를 가짐

# 스택과 큐의 차이

## 스택
- **후입선출(LIFO: Last-In-First-Out)** 방식으로 데이터를 저장하고 접근
- push()를 사용하여 데이터를 스택의 맨 위에 추가
- pop() 메서드를 사용하여 맨 위의 데이터에 접근

## 큐
- **선입선출(FIFO: First-In-First-Out)** 방식으로 데이터를 저장하고 접근
- offer() 메서드를 사용하여 데이터를 큐의 맨 뒤에 추가
- poll() 메서드를 사용하여 맨 앞의 데이터를 접근

# 버블정렬

인접한 두 원소의 대소를 비교하고 조건에 맞지 않으면 위치를 교환하면서 정렬하는 알고리즘

![bubble-sort-001](https://user-images.githubusercontent.com/97332044/233838605-b75a0ed4-ab3d-4a40-99cf-c7eebab03a36.gif)

## 자바로 구현한 예제

``` Java
public class BubbleSort {
    public static void main(String[] args) {
        int[] arr = {3, 1, 9, 6, 0, 7};

        for (int i = 0; i < arr.length - 1; i++) {
            for (int j = 0; j < arr.length - i - 1; j++) {
                if (arr[j] > arr[j+1]) {
                    int temp = arr[j];
                    arr[j] = arr[j+1];
                    arr[j+1] = temp;
                }
            }
        }
    }
}
```

## 장점

- 구현이 매우 간단
- 작은 데이터셋에서는 다른 알고리즘보다 빠를 수 있음

## 단점

- 최악의 경우 시간 복잡도가 O(n^2)으로 매우 느림
- 정렬할 데이터가 이미 **거의 정렬된 상태**라면 교환 작업을 최소화하기 어렵기 때문에 다른 알고리즘보다 성능이 떨어질 수 있음
- 데이터의 이동 횟수가 많기 때문에 데이터의 개수가 많을수록 메모리를 많이 사용하게 됨

## 시간복잡도

### 최선의 경우

입력 데이터가 이미 정렬되어 있는 경우

- 인접한 두 원소의 비교만으로 정렬이 완료 - **O(n)**

### 평균 및 최악의 경우

입력 데이터가 무작위로 주어지는 경우
 
- 모든 원소를 비교하며 교환해야 함 - **O(n^2)**

# 퀵정렬

분할 정복 방식을 사용하는 비교 기반 정렬 알고리즘

![퀵 정렬](https://user-images.githubusercontent.com/97332044/233842224-2a8aecf5-9617-421b-85e0-aee0d416b2cb.gif)

## 자바로 구현한 예제

``` Java
public class QuickSort {
    
    public static void main(String[] args) {
        int[] arr = { 9, 8, 7, 6, 5, 4, 3, 2, 1 };
        quickSort(arr, 0, arr.length - 1);
        for (int i = 0; i < arr.length; i++) {
            System.out.print(arr[i] + " ");
        }
    }

    public static void quickSort(int[] arr, int left, int right) { 
        if (left < right) {
            int pivotIndex = partition(arr, left, right);
            quickSort(arr, left, pivotIndex - 1);
            quickSort(arr, pivotIndex + 1, right);
        }
    }

    public static int partition(int[] arr, int left, int right) { // 분할
        int pivot = arr[right];
        int i = left - 1;
        for (int j = left; j < right; j++) {
            if (arr[j] < pivot) {
                i++;
                swap(arr, i, j);
            }
        }
        swap(arr, i + 1, right);
        return i + 1;
    }

    public static void swap(int[] arr, int i, int j) { // 정복(요소들의 위치 교환)
        int temp = arr[i];
        arr[i] = arr[j];
        arr[j] = temp;
    }
}

```
## 동작 방식

1. 정렬할 배열에서 하나의 원소를 선택하여 **기준값(pivot)** 으로 설정

2. 배열에서 기준값 제외한 나머지 원소들을 기준값을 기준으로 두 개의 부분 배열로 **분할** (작은 값은 왼쪽에 큰 값은 오른쪽에 위치하도록 분할)

3. 각 부분 배열을 재귀적으로 퀵 정렬을 수행 (기준값은 이미 정렬되어있어 부분 배열에 포함하지 않음)

4. 부분 배열들이 더 이상 분할되지 않는다면 부분 배열들을 하나의 배열로 합침(**정복**)

## 장점
- 불필요한 데이터의 이동을 최소화 → 다른 정렬 알고리즘보다 효율적

## 단점
- **정렬된 배열**에 대해서는 평균적인 경우와 같은 성능X
- 기준값 선택 방법에 따라 수행 시간이 크게 영향을 받음
- 안정 정렬이 아니므로 동일한 값을 가지는 원소들의 순서가 바뀔 수 있음

## 시간복잡도

### 최선의 경우

기준점을 기준으로 균등하게 분할되는 경우 - **O(n log n)**

### 평균의 경우

기준점이 균등하지 않은 경우 - 대부분의 경우 **O(n log n)** 에 가깝게 수행됨

### 최악의 경우

기준점이 항상 최소값이나 최대값으로 선택되는 경우 - **O(n^2)**

## 자바의 Arrays.sort() 메소드

Java 7 이전 버전에서는 **Quicksort** 을 사용
Java SE 7부터 **Dual-Pivot Quicksort** 을 사용함 

### Dual-Pivot Quicksort

기존 퀵 정렬보다 효율적이며 대부분의 경우 **O(n log n)** 시간복잡도를 가짐

pivot(기준점) 을 두 개로 선택하여 배열을 3개의 영역으로 구분하여 분할하며 각각 퀵정렬을 수행한다