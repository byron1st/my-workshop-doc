@Import
* {`AS01`, `AS02`, `AS04`} from [설계전략](https://github.com/byron1st/my-workshop-doc/blob/master/doc/arch.strategies.md)
* all from 시나리오 of [2레벨 시나리오 뷰](https://github.com/byron1st/my-workshop-doc/blob/master/doc/arch.views.2.scenario.md)
* all as `sc` from 도출된 요소들 of [2레벨 시나리오 뷰](https://github.com/byron1st/my-workshop-doc/blob/master/doc/arch.views.2.scenario.md)

# 레벨 2: 논리 뷰
## 다이어그램들
### LO02: `l.MainWindow` 분해
![LO02](https://github.com/byron1st/my-workshop-doc/blob/master/images/logical-view-lo02-2016-08-19.png)
* 설계 근거: `AS01`, `AS02`, `SC06`, `SC07`, `SC08`

### LO03: `l.App` 실행 시 구조
![LO03](https://github.com/byron1st/my-workshop-doc/blob/master/images/logical-view-lo03-2016-08-19.png)
* 설계 근거: `AS01`, `AS02`, `SC05`, `SC12`

### LO04: `l.App` 프로그램 로딩 시 구조
![LO04](https://github.com/byron1st/my-workshop-doc/blob/master/images/logical-view-lo04-2016-08-19.png)
* 설계 근거: `AS02`, `AS03`, `SC09`, `SC13`

## 도출된 요소들 및 레벨 1 설계로부터의 추적성
* 컴포넌트
  * `l.MainWindow`
    * `ReactUIComponents`
    * `Dispatcher`
    * `IPC`
    * `Store`
    * `Action`
  * `l.App`
    * `Dispatcher`
    * `IPC`
    * `Action`
    * `Main`
    * `MainMenu`
    * `DB`
    * `AppMode`
    * `Settings`
* 커넥터 (생략)