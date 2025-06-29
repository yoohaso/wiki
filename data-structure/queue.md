# 큐 (Queue)

#### 1. 정의
- 선입선출 방식으로 동작하는 선형 자료 구조입니다.

#### 2. 비유
- 사람들이 줄을 서고 나갈 때를 생각하면 됩니다.

#### 3. 기능 설명
- Enqueue(삽입)
	- 큐의 뒤에 데이터가 추가 됩니다.
	- 사람들이 줄의 뒤에 서는 것을 생각할 수 있습니다.
- Dequeue(삭제)
	- 큐의 앞에서 데이터가 삭제 됩니다.
	- 줄에서 앞사람이 빠져나가는 걸 생각할 수 있습니다.

#### 4. 실전 예시
- 브라우저의 Task queue
	- 비동기 작업의 콜백함수가 태스크 큐에 추가되고, 콜스택이 비면 이벤트 루프가 꺼내 콜스택에 추가
- BFS
	- 그래프 탐색 시, 방문 대기 중인 노드를 큐로 관리

#### 5. 구현
- 자바스크립트에서는 배열로 큐를 구현하는 경우가 많지만, 배열의 `shift(n)` 연산은 `O(n)`이므로 성능이 중요한 경우에 연결 리스트 기반으로 구현하는 것이 적절합니다.

#### 6. 시간 복잡도
- 삽입: O(1)
- 삭제: O(1)

#### 6. 자료구조 적용 판단 기준
- 데이터를 추가된 순서대로 처리해야할 때 고려할 수 있습니다.
