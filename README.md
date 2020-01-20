<h1 align="center">
  <a href="https://animejs.com"><img src="./documentation/assets/img/animejs-v3-header-animation.gif" width="250"/></a>
  <br>
  anime.js
</h1>

<h4 align="center">JavaScript 애니메이션 엔진 | <a href="https://animejs.com" target="_blank">animejs.com</a></h4>

<p align="center">
  <a href="https://www.npmjs.com/package/animejs" rel="nofollow"><img src="https://camo.githubusercontent.com/011820ee25bf1d3ddaf635d869903b98eccaeae7/68747470733a2f2f696d672e736869656c64732e696f2f6e706d2f762f616e696d656a732e7376673f7374796c653d666c61742d737175617265" alt="npm version" data-canonical-src="https://img.shields.io/npm/v/animejs.svg?style=flat-square" style="max-width:100%;"></a>
  <a href="https://www.npmjs.com/package/animejs" rel="nofollow"><img src="https://camo.githubusercontent.com/3e9b69d51aee25fad784a3097676696096621d47/68747470733a2f2f696d672e736869656c64732e696f2f6e706d2f646d2f616e696d656a732e7376673f7374796c653d666c61742d737175617265" alt="npm downloads" data-canonical-src="https://img.shields.io/npm/dm/animejs.svg?style=flat-square" style="max-width:100%;"></a>
</p>

<blockquote align="center">
  <b>Anime.js</b>는 간단하지만 강력한 API를 제공하는 가볍고 빠른 JavaScript 애니메이션 라이브러리입니다.<br>
  CSS 속성, SVG, DOM 속성 그리고 JavaScript 객체를 조작해 애니메이션을 구현합니다.
</blockquote>

<p align="center">
  <a href="#시작하기">시작하기</a>&nbsp;|&nbsp;<a href="#사용-설명서">사용 설명서</a>&nbsp;|&nbsp;<a href="#데모-및-예제">데모 및 예제</a>&nbsp;|&nbsp;<a href="#브라우저-호환성">브라우저 호환성</a>
</p>

## 시작하기

### 다운로드

[NPM](https://npmjs.com)을 사용해 다운로드 받을 경우, 아래 명령어를 터미널에 입력합니다.

```bash
$ npm install animejs --save
```

또는 직접 [다운로드](https://github.com/juliangarnier/anime/archive/master.zip)하여 사용할 수 있도 있습니다.

### 사용법

#### ES6 모듈

접미사 `es`가 포함된 파일을 호출하여 사용합니다.

```javascript
import anime from 'animejs/lib/anime.es.js';
```

#### CommonJS

Node.js의 `require()` 함수를 사용할 경우, 아래와 같이 입력합니다.

```javascript
const anime = require('animejs');
```

#### 파일 포함

HTML에 `anime.min.js`를 불러오는 코드를 추가합니다.

```html
<script src="anime.min.js"></script>
```

### 안녕! Anime.js

Anime.js 사용법은 매우 간단합니다. `anime()` 함수 인자로 옵션(객체)을 설정하여 애니메이션을 대상에 적용할 수 있습니다.

```javascript
anime({
  // 애니메이션을 적용할 대상 (CSS 선택자)
  targets: '.anime',
  // X축으로 100px 만큼 이동
  translateX: 100,
  // 1.5바퀴 회전
  rotate: '1.5turn',
  // 배경 색상 변경
  backgroundColor: '#fefefe',
  // 0.4초 동안 애니메이션 처리
  duration: 400
});
```

## [사용 설명서](https://animejs.com./documentation/)

Anime.js의 강력한 기능을 100% 활용하려면 다음의 각 개념을 이해하고 사용법에 대해 학습해야 합니다.

* [대상(Targets)](https://animejs.com./documentation/#cssSelector)
* [CSS 속성(Properties)](https://animejs.com./documentation/#cssProperties)
* [속성 매개변수(Property parameters)](https://animejs.com./documentation/#duration)
* [애니메이션 매개변수(Animation parameters)](https://animejs.com./documentation/#direction)
* [값(Values)](https://animejs.com./documentation/#unitlessValue)
* [키프레임(Keyframes)](https://animejs.com./documentation/#animationKeyframes)
* [스태거(Staggering)](https://animejs.com./documentation/#staggeringBasics)
* [타임라인(Timeline)](https://animejs.com./documentation/#timelineBasics)
* [컨트롤(Controls)](https://animejs.com./documentation/#playPause)
* [콜백과 프로미스(Callbacks and promises)](https://animejs.com./documentation/#update)
* [SVG 애니메이션(Animations)](https://animejs.com./documentation/#motionPath)
* [이징 함수(Easing functions)](https://animejs.com./documentation/#linearEasing)
* [헬퍼(Helpers)](https://animejs.com./documentation/#remove)

## [데모 및 예제](http://codepen.io/collection/b392d3a52d6abf5b8d9fda4e4cab61ab/)

* [CodePen 데모 및 예제](http://codepen.io/collection/b392d3a52d6abf5b8d9fda4e4cab61ab/)
* [juliangarnier.com](http://juliangarnier.com)
* [animejs.com](https://animejs.com)
* [텍스트 애니메이션](http://tobiasahlin.com/moving-letters/) by [@tobiasahlin](https://twitter.com/tobiasahlin)
* [그레디언트 지형 애니메이션](https://tympanus.net/Development/GradientTopographyAnimation/) by [@crnacura](https://twitter.com/crnacura)
* [유기적 도형 애니메이션](https://tympanus.net/Development/OrganicShapeAnimations/) by [@crnacura](https://twitter.com/crnacura)
* [피스 슬라이더](https://tympanus.net/Tutorials/PiecesSlider/) by [@lmgonzalves](https://twitter.com/lmgonzalves)
* [스태거 애니메이션](https://codepen.io/juliangarnier/pen/4fe31bbe8579a256e828cd4d48c86182?editors=0100)
* [이징 애니메이션](https://codepen.io/juliangarnier/pen/444ed909fd5de38e3a77cc6e95fc1884)
* [구체 애니메이션](https://codepen.io/juliangarnier/pen/b3bb8ca599ad0f9d00dd044e56cbdea5?editors=0010)
* [레이어 애니메이션](https://codepen.io/juliangarnier/pen/6ca836535cbea42157d1b8d56d00be84?editors=0010)
* [anime.js 로고 애니메이션](https://codepen.io/juliangarnier/pen/d43e8ec355c30871cbe775193255d6f6?editors=0010)


## 브라우저 호환성

| Chrome | Safari | IE / Edge | Firefox | Opera |
| --- | --- | --- | --- | --- |
| 24+ | 8+ | 11+ | 32+ | 15+ |

## <a href="https://animejs.com"><img src="./documentation/assets/img/animejs-v3-logo-animation.gif" width="150" alt="anime.js v3 로고"/></a>

[웹사이트](https://animejs.com/) | [사용 설명서](https://animejs.com./documentation/) | [데모 및 예제](http://codepen.io/collection/b392d3a52d6abf5b8d9fda4e4cab61ab/) | [MIT License](LICENSE.md) | © 2019 [Julian Garnier](http://juliangarnier.com).
