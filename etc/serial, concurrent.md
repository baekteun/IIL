# 직렬, 동시

- 위에서 동기, 비동기로 보낸 그 작업들을 `순차적`으로 처리할 지 결정하는 것.
- 정확히는 직렬큐(순차처리큐) 또는 동시큐(순차고려x큐)의 맨뒤로 보내는 것.


## 직렬
- `단 하나의 쓰레드`로만 작업을 보내는 대기열
- GCD에서 mainQueue에서 mainThread로 보냄
- 즉 순차적으로 처리됨

## 동시
- `여러개의 다른 쓰레드`로 작업을 보내는 대기열
- GCD에서 globalQueue에서 customQueue에서 여러 스레드로 나눠 보냄
- 순서는 상관없게 됨

