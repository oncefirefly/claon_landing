<template>
  <header class="header">
    <div class="header__container container">
      <div class="header__upper">
        <a href="#" class="header__logo logo">
          <img src="../assets/img/logo.svg" alt="claon logo" />
        </a>
        <form class="header__search search">
          <img
            src="../assets/img/icon_search.svg"
            alt="search icon"
            class="search__icon"
          />
          <input
            name="search"
            type="input"
            placeholder="합격을 함께할 강의를 찾아보세요"
          />
        </form>
        <div class="header__auth auth">
          <span class="auth__login">로그인</span>
          <span class="auth__register">회원가입</span>
        </div>
      </div>

      <nav class="header__nav nav">
        <a href="#" class="nav__link link">카테고리</a>
        <a href="#" class="nav__link link">라이브</a>
        <a href="#" class="nav__link link">이벤트</a>
        <a href="#" class="nav__link link">커뮤니티</a>
        <a href="#" class="nav__link link">Book Store</a>
        <a href="#" class="nav__link link">합격후기</a>
        <a href="#" class="nav__link link">클래온스토어</a>
        <a href="#" class="nav__link link">
          <img
            src="../assets/img/icon_store.svg"
            alt="store icon"
            class="link__icon"
          />
          입점사 센터 이동
        </a>
      </nav>
    </div>
  </header>

  <main class="main">
    <section class="hero">
      <div class="hero__container container">
        <div class="hero__slider slider">
          <img
            src="../assets/img/icon_arrow_left.svg"
            alt="arrow icon"
            class="slider__arrow"
          />
        </div>
        <div class="hero__text">
          <h1 class="hero__title">신한카드 결제 시즉시 할인 5%</h1>
          <p class="hero__description">4월 11일(월) 부터 최대 5만원 할인</p>
          <div class="hero__gauge gauge">
            <span class="gauge__from">02</span>
            <div class="gauge__bar">
              <div class="gauge__bar_filled"></div>
              <div class="gauge__bar_empty"></div>
            </div>
            <span class="gauge__to">03</span>
            <button class="gauge__pause">
              <img src="../assets/img/btn_pause.svg" alt="Pause" />
            </button>
          </div>
        </div>
        <div class="hero__img">
          <picture>
            <source srcset="../assets/img/img_banner.webp" type="image/webp" />
            <img src="../assets/img/img_banner.png" alt="banner image" />
          </picture>
        </div>
        <div class="hero__slider slider">
          <img
            src="../assets/img/icon_arrow_right.svg"
            alt="arrow icon"
            class="slider__arrow"
          />
        </div>
      </div>
    </section>

    <section class="interests">
      <div class="interests__container container">
        <h2 class="interests__title section-title">인기 관심분야</h2>
        <ul class="interests__list">
          <li>
            <div>
              <img src="../assets/img/interests1.svg" alt="interest" />
            </div>
            <span>공무원</span>
          </li>
          <li>
            <div>
              <img src="../assets/img/interests2.svg" alt="interest" />
            </div>
            <span>공인중개사</span>
          </li>
          <li>
            <div>
              <img src="../assets/img/interests3.svg" alt="interest" />
            </div>
            <span>운전직공무원</span>
          </li>
          <li>
            <div>
              <img src="../assets/img/interests4.svg" alt="interest" />
            </div>
            <span>전기기사</span>
          </li>
          <li>
            <div>
              <img src="../assets/img/interests5.svg" alt="interest" />
            </div>
            <span>소방공무원</span>
          </li>
          <li>
            <div>
              <img src="../assets/img/interests6.svg" alt="interest" />
            </div>
            <span>IT자격증</span>
          </li>
          <li>
            <div>
              <img src="../assets/img/interests7.svg" alt="interest" />
            </div>
            <span>세무사</span>
          </li>
          <li>
            <div>
              <img src="../assets/img/interests8.svg" alt="interest" />
            </div>
            <span>영어</span>
          </li>
        </ul>
      </div>
    </section>

    <section class="lectures">
      <div class="lectures__container">
        <div class="container">
          <h2 class="lectures__title section-title">사람들이 주목하는 강의</h2>
        </div>

        <div class="lectures__content">
          <div class="lectures__slider_left lectures__slider">
            <img
              src="../assets/img/icon_arrow_black.svg"
              alt="arrow icon"
              class="slider__arrow_right"
            />
          </div>

          <div class="lectures__cards cards">
            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail1.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail1.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">부동산 예즈덤</h3>
              <p class="card__description">공인중개사 자격증 합격의 시작!</p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account1.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account1.png" alt="publisher" />
                </picture>
                <p>부동산학개론 주형남</p>
              </div>
              <p class="card__price price">
                <span class="price__current">159,000원</span>
                <span class="price__crossed"></span>
                <span class="price__discount"></span>
              </p>

              <div class="card__marks" v-if="true">
                <mark
                  class="card__live"
                  v-if="true"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="false"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="false"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="false"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>

            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail2.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail2.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">나사렛</h3>
              <p class="card__description">
                너의 꿈을 이루게 해줄게! 이주왕의 합격의 신! 경찰이 된다!
              </p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account2.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account2.png" alt="publisher" />
                </picture>
                <p>경찰행정 이주왕 교수남</p>
              </div>
              <p class="card__price price">
                <span class="price__current">68,000원</span>
                <span class="price__crossed">100,000원</span>
                <span class="price__discount">42%</span>
              </p>
              <div class="card__marks" v-if="true">
                <mark
                  class="card__live"
                  v-if="false"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="true"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="true"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="false"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>

            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail2.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail2.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">포스트 공인중개</h3>
              <p class="card__description">포스트 공인중개사의 시작</p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account3.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account3.png" alt="publisher" />
                </picture>
                <p>공인중개사 김태평</p>
              </div>
              <p class="card__price price">
                <span class="price__current">117,000원</span>
                <span class="price__crossed"></span>
                <span class="price__discount"></span>
              </p>
              <div class="card__marks" v-if="false">
                <mark
                  class="card__live"
                  v-if="false"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="false"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="false"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="false"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>

            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail2.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail2.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">리메인</h3>
              <p class="card__description">R로 배우는 데이터 시각화 기초</p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account4.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account4.png" alt="publisher" />
                </picture>
                <p>문가든 개발자</p>
              </div>
              <p class="card__price price">
                <span class="price__current">132,000원</span>
                <span class="price__crossed">160,000원</span>
                <span class="price__discount">15%</span>
              </p>
              <div class="card__marks" v-if="true">
                <mark
                  class="card__live"
                  v-if="true"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="false"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="false"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="false"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>
          </div>

          <div class="lectures__slider_right lectures__slider">
            <img
              src="../assets/img/icon_arrow_black.svg"
              alt="arrow icon"
              class="slider__arrow_right"
            />
          </div>
        </div>
      </div>
    </section>

    <section class="custom-lectures">
      <div class="lectures__container">
        <div class="container">
          <h2 class="lectures__title section-title">고객 맞춤 추천 강의</h2>
        </div>

        <div class="lectures__content">
          <div class="lectures__slider_left lectures__slider">
            <img
              src="../assets/img/icon_arrow_black.svg"
              alt="arrow icon"
              class="slider__arrow_right"
            />
          </div>

          <div class="custom-lectures__cards cards">
            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail1.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail1.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">몰입코딩</h3>
              <p class="card__description">
                풀스택 리액트 개발자 취업을 위한 핵심 커리큘럼 by 몰입코딩
              </p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account5.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account5.png" alt="publisher" />
                </picture>
                <p>이은주 강사</p>
              </div>
              <p class="card__price price">
                <span class="price__current">80,000원</span>
                <span class="price__crossed"></span>
                <span class="price__discount"></span>
              </p>
              <div class="card__marks" v-if="true">
                <mark
                  class="card__live"
                  v-if="true"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="true"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="true"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="true"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="true"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>

            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail2.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail2.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">세무회계 문정</h3>
              <p class="card__description">세무사 황윤화 회계원리_입문</p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account6.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account6.png" alt="publisher" />
                </picture>
                <p>황윤화</p>
              </div>
              <p class="card__price price">
                <span class="price__current">135,000원</span>
                <span class="price__crossed">160,000원</span>
                <span class="price__discount">3%</span>
              </p>
              <div class="card__marks" v-if="true">
                <mark
                  class="card__live"
                  v-if="true"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="false"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="false"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="false"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>

            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail7.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail7.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">국가마스터</h3>
              <p class="card__description">국가고시 파이널 특강</p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account7.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account7.png" alt="publisher" />
                </picture>
                <p>국가고시 마스터 최홍철</p>
              </div>
              <p class="card__price price">
                <span class="price__current">245,000원</span>
                <span class="price__crossed">285,000원</span>
                <span class="price__discount">20%</span>
              </p>
              <div class="card__marks" v-if="true">
                <mark
                  class="card__live"
                  v-if="true"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="false"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="false"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="false"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>

            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail1.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail1.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">ELS 영어</h3>
              <p class="card__description">
                실리콘밸리에서 온 진짜 비즈니스 영어
              </p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account8.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account8.png" alt="publisher" />
                </picture>
                <p>유명현</p>
              </div>
              <p class="card__price price">
                <span class="price__current">149,000원</span>
                <span class="price__crossed"></span>
                <span class="price__discount"></span>
              </p>
              <div class="card__marks" v-if="true">
                <mark
                  class="card__live"
                  v-if="true"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="false"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="false"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="false"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>
          </div>

          <div class="lectures__slider_right lectures__slider">
            <img
              src="../assets/img/icon_arrow_black.svg"
              alt="arrow icon"
              class="slider__arrow_right"
            />
          </div>
        </div>
      </div>
    </section>

    <section class="banner">
      <div class="banner__container container">
        <picture>
          <source srcset="../assets/img/banner_inner.webp" type="image/webp" />
          <img src="../assets/img/banner_inner.png" alt="thumbnail" />
        </picture>
        <div class="banner__description">
          <p class="banner__subtitle">세모담 수강생에게 직접 물었습니다.</p>
          <h2 class="banner__title">강의 리얼 후기[IT자격증] 편</h2>
        </div>
        <button class="banner__more-btn">자세히 보기</button>
      </div>
    </section>

    <section class="week-lectures">
      <div class="lectures__container">
        <div class="container">
          <h2 class="lectures__title section__title">이번주 시작</h2>
        </div>

        <div class="lectures__content">
          <div class="lectures__slider_left lectures__slider">
            <img
              src="../assets/img/icon_arrow_black.svg"
              alt="arrow icon"
              class="slider__arrow_right"
            />
          </div>

          <div class="week-lectures__cards cards">
            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail9.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail9.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">한국 공인회계</h3>
              <p class="card__description">권오상의 공인회계 실무강의</p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account1.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account1.png" alt="publisher" />
                </picture>
                <p>공인회계 마스터 권오상</p>
              </div>
              <p class="card__price price">
                <span class="price__current">159,000원</span>
                <span class="price__crossed">242,000원</span>
                <span class="price__discount">25%</span>
              </p>
              <div class="card__marks" v-if="true">
                <mark
                  class="card__live"
                  v-if="true"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="false"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="false"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="false"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>

            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail10.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail10.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">잉글리쉬 큐브</h3>
              <p class="card__description">이준석의 영문법 패키지</p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account2.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account2.png" alt="publisher" />
                </picture>
                <p>이선미 강사</p>
              </div>
              <p class="card__price price">
                <span class="price__current">117,000원</span>
                <span class="price__crossed">150,000원</span>
                <span class="price__discount">14%</span>
              </p>
              <div class="card__marks" v-if="true">
                <mark
                  class="card__live"
                  v-if="true"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="false"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="false"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="false"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>

            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail11.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail11.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">국가마스터</h3>
              <p class="card__description">
                국가고시 마스터의 완전한 합격을 위한 9급 공무원 슈퍼패스
                입문+실전 완전체 강의
              </p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account3.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account3.png" alt="publisher" />
                </picture>
                <p>국가고시 마스터 최홍철</p>
              </div>
              <p class="card__price price">
                <span class="price__current">153,000원</span>
                <span class="price__crossed"></span>
                <span class="price__discount"></span>
              </p>
              <div class="card__marks" v-if="true">
                <mark
                  class="card__live"
                  v-if="true"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="false"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="false"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="false"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>

            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail12.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail12.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">디스커버G</h3>
              <p class="card__description">
                비전공자를 위한 개발자 취업 올인원 가이드
              </p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account4.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account4.png" alt="publisher" />
                </picture>
                <p>개발자 한정수</p>
              </div>
              <p class="card__price price">
                <span class="price__current">89,000원</span>
                <span class="price__crossed"></span>
                <span class="price__discount"></span>
              </p>
              <div class="card__marks" v-if="true">
                <mark
                  class="card__live"
                  v-if="true"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="false"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="false"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="false"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>

            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail13.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail13.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">시원스쿨</h3>
              <p class="card__description">
                독학으로 1달만에 토익 LC 만점 공부법 가이드북
              </p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account5.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account5.png" alt="publisher" />
                </picture>
                <p>그레이스</p>
              </div>
              <p class="card__price price">
                <span class="price__current">101,000원</span>
                <span class="price__crossed"></span>
                <span class="price__discount"></span>
              </p>
              <div class="card__marks" v-if="true">
                <mark
                  class="card__live"
                  v-if="true"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="false"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="false"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="false"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>

            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail14.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail14.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">시원스쿨</h3>
              <p class="card__description">영어회화 독학법</p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account6.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account6.png" alt="publisher" />
                </picture>
                <p>이지은 강사</p>
              </div>
              <p class="card__price price">
                <span class="price__current">99,000원</span>
                <span class="price__crossed">210,000원</span>
                <span class="price__discount">14%</span>
              </p>
              <div class="card__marks" v-if="true">
                <mark
                  class="card__live"
                  v-if="true"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="false"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="false"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="false"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>

            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail15.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail15.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">국가마스터</h3>
              <p class="card__description">대학생만을 위한 대학생 합격패스</p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account7.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account7.png" alt="publisher" />
                </picture>
                <p>전선혜</p>
              </div>
              <p class="card__price price">
                <span class="price__current">110,000원</span>
                <span class="price__crossed"></span>
                <span class="price__discount"></span>
              </p>
              <div class="card__marks" v-if="true">
                <mark
                  class="card__live"
                  v-if="true"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="false"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="false"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="false"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>

            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail16.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail16.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">ebs</h3>
              <p class="card__description">9급 공무원 기본서 행정학개론</p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account8.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account8.png" alt="publisher" />
                </picture>
                <p>9급 공무원 이종석</p>
              </div>
              <p class="card__price price">
                <span class="price__current">86,000원</span>
                <span class="price__crossed">100,000원</span>
                <span class="price__discount">5%</span>
              </p>
              <div class="card__marks" v-if="true">
                <mark
                  class="card__live"
                  v-if="true"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="false"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="false"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="false"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>
          </div>

          <div class="lectures__slider_right lectures__slider">
            <img
              src="../assets/img/icon_arrow_black.svg"
              alt="arrow icon"
              class="slider__arrow_right"
            />
          </div>
        </div>
      </div>
    </section>

    <section class="recomended-lectures">
      <div class="lectures__container">
        <div class="container">
          <h2 class="lectures__title section__title">MD 추천 강의</h2>
        </div>

        <div class="lectures__content">
          <div class="lectures__slider_left lectures__slider">
            <img
              src="../assets/img/icon_arrow_black.svg"
              alt="arrow icon"
              class="slider__arrow_right"
            />
          </div>

          <div class="recomended-lectures__cards cards">
            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail17.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail17.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">레주메빌더</h3>
              <p class="card__description">디지털 데이터 분석 용어 정리</p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account1.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account1.png" alt="publisher" />
                </picture>
                <p>공인회계 마스터 권오상</p>
              </div>
              <p class="card__price price">
                <span class="price__current">159,000원</span>
                <span class="price__crossed">300,000원</span>
                <span class="price__discount">40%</span>
              </p>
              <div class="card__marks" v-if="true">
                <mark
                  class="card__live"
                  v-if="true"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="false"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="true"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="true"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>

            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail18.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail18.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">나희수 공인중개</h3>
              <p class="card__description">출제문제를 정확하고 완벽한 정리!</p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account2.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account2.png" alt="publisher" />
                </picture>
                <p>이형준 강사</p>
              </div>
              <p class="card__price price">
                <span class="price__current">98,000원</span>
                <span class="price__crossed"></span>
                <span class="price__discount"></span>
              </p>
              <div class="card__marks" v-if="false">
                <mark
                  class="card__live"
                  v-if="false"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="false"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="false"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="false"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>

            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail19.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail19.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">국가마스터</h3>
              <p class="card__description">
                완전한 합격을 위한 9급 공무원 슈퍼패스 입문+실전 완전체 강의
              </p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account3.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account3.png" alt="publisher" />
                </picture>
                <p>국가고시 마스터 최홍철</p>
              </div>
              <p class="card__price price">
                <span class="price__current">153,000원</span>
                <span class="price__crossed">210,000원</span>
                <span class="price__discount">7%</span>
              </p>
              <div class="card__marks" v-if="true">
                <mark
                  class="card__live"
                  v-if="true"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="false"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="false"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="false"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>

            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail20.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail20.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">개발나라</h3>
              <p class="card__description">
                파이썬 웹크롤링을 통해 스스로 업무자동화 구현합시다
              </p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account4.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account4.png" alt="publisher" />
                </picture>
                <p>모원서</p>
              </div>
              <p class="card__price price">
                <span class="price__current">89,000원</span>
                <span class="price__crossed">100,000원</span>
                <span class="price__discount">4%</span>
              </p>
              <div class="card__marks" v-if="true">
                <mark
                  class="card__live"
                  v-if="true"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="false"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="false"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="true"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>

            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail21.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail21.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">데이터클라스</h3>
              <p class="card__description">MySQL 데이터베이스 입문 가이드북</p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account5.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account5.png" alt="publisher" />
                </picture>
                <p>신윤환</p>
              </div>
              <p class="card__price price">
                <span class="price__current">130,000원</span>
                <span class="price__crossed"></span>
                <span class="price__discount"></span>
              </p>
              <div class="card__marks" v-if="true">
                <mark
                  class="card__live"
                  v-if="true"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="false"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="false"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="false"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>

            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail22.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail22.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">Python</h3>
              <p class="card__description">데이터 분석을 위한 파이썬</p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account6.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account6.png" alt="publisher" />
                </picture>
                <p>윤인도</p>
              </div>
              <p class="card__price price">
                <span class="price__current">254,000원</span>
                <span class="price__crossed">280,000원</span>
                <span class="price__discount">4%</span>
              </p>
              <div class="card__marks" v-if="true">
                <mark
                  class="card__live"
                  v-if="true"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="false"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="false"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="false"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>

            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail23.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail23.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">국가고시 마스터 최홍철</h3>
              <p class="card__description">
                파이썬 기초부터 웹 스크래핑 및 업무 자동화
              </p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account7.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account7.png" alt="publisher" />
                </picture>
                <p>SJN</p>
              </div>
              <p class="card__price price">
                <span class="price__current">149,000원</span>
                <span class="price__crossed"></span>
                <span class="price__discount"></span>
              </p>
              <div class="card__marks" v-if="true">
                <mark
                  class="card__live"
                  v-if="true"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="false"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="false"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="false"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>

            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail16.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail16.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">개발자 한정수</h3>
              <p class="card__description">
                토익RC 동사만 제대로 알아도 절반은 끝!
              </p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account8.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account8.png" alt="publisher" />
                </picture>
                <p>Yu lee</p>
              </div>
              <p class="card__price price">
                <span class="price__current">100,000원</span>
                <span class="price__crossed"></span>
                <span class="price__discount"></span>
              </p>
              <div class="card__marks" v-if="true">
                <mark
                  class="card__live"
                  v-if="true"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="false"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="false"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="false"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>
          </div>

          <div class="lectures__slider_right lectures__slider">
            <img
              src="../assets/img/icon_arrow_black.svg"
              alt="arrow icon"
              class="slider__arrow_right"
            />
          </div>
        </div>
      </div>
    </section>

    <section class="best-lectures">
      <div class="lectures__container">
        <div class="container">
          <h2 class="lectures__title section-title">베스트</h2>
        </div>

        <div class="lectures__content">
          <div class="lectures__slider_left lectures__slider">
            <img
              src="../assets/img/icon_arrow_black.svg"
              alt="arrow icon"
              class="slider__arrow_right"
            />
          </div>

          <div class="best-lectures__cards cards">
            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail24.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail24.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">라라</h3>
              <p class="card__description">
                10년 차 개발자의 [게임 개발/앱 개발/프로그래밍]을 위한 C/C++
                입문
              </p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account1.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account1.png" alt="publisher" />
                </picture>
                <p>라라 개발자</p>
              </div>
              <p class="card__price price">
                <span class="price__current">159,000원</span>
                <span class="price__crossed">253,000원</span>
                <span class="price__discount">10%</span>
              </p>
              <div class="card__marks" v-if="true">
                <mark
                  class="card__live"
                  v-if="true"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="false"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="false"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="false"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>

            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail25.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail25.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">몰입코딩</h3>
              <p class="card__description">SQLD 자격증 대비 문제풀이</p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account2.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account2.png" alt="publisher" />
                </picture>
                <p>한정수 개발자</p>
              </div>
              <p class="card__price price">
                <span class="price__current">117,000원</span>
                <span class="price__crossed">280,000원</span>
                <span class="price__discount">14%</span>
              </p>
              <div class="card__marks" v-if="true">
                <mark
                  class="card__live"
                  v-if="true"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="false"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="false"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="false"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>

            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail26.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail26.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">우상 공인중개사</h3>
              <p class="card__description">핵심만 콕콕! 짚어주는 집중특강</p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account3.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account3.png" alt="publisher" />
                </picture>
                <p>김현민 강사</p>
              </div>
              <p class="card__price price">
                <span class="price__current">153,000원</span>
                <span class="price__crossed"></span>
                <span class="price__discount"></span>
              </p>
              <div class="card__marks" v-if="true">
                <mark
                  class="card__live"
                  v-if="true"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="false"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="false"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="false"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>

            <div class="cards__card card">
              <picture>
                <source
                  srcset="../assets/img/thumnail27.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail27.png" alt="thumbnail" />
              </picture>
              <h3 class="card__title">개발나라</h3>
              <p class="card__description">
                파이썬 웹크롤링을 통해 스스로 업무자동화 구현합시다
              </p>
              <div class="card__publisher">
                <picture>
                  <source
                    srcset="../assets/img/img_account4.webp"
                    type="image/webp"
                  />
                  <img src="../assets/img/img_account4.png" alt="publisher" />
                </picture>
                <p>모원서</p>
              </div>
              <p class="card__price price">
                <span class="price__current">89,000원</span>
                <span class="price__crossed">160,000원</span>
                <span class="price__discount">15%</span>
              </p>
              <div class="card__marks" v-if="true">
                <mark
                  class="card__live"
                  v-if="true"
                  :style="{ background: '#fc4631' }"
                  >Live</mark
                >
                <mark
                  class="card__package"
                  v-if="false"
                  :style="{ background: '#3170ff' }"
                  >패키지</mark
                >
                <mark
                  class="card__coupon"
                  v-if="false"
                  :style="{ background: '#ab48ff' }"
                  >쿠폰</mark
                >
                <mark
                  class="card__subscribe"
                  v-if="false"
                  :style="{ background: '#e4007f' }"
                  >구독</mark
                >
                <mark
                  class="card__offline"
                  v-if="false"
                  :style="{ background: '#808080' }"
                  >오프라인</mark
                >
              </div>
            </div>
          </div>

          <div class="lectures__slider_right lectures__slider">
            <img
              src="../assets/img/icon_arrow_black.svg"
              alt="arrow icon"
              class="slider__arrow_right"
            />
          </div>
        </div>
      </div>
    </section>

    <section class="reviews">
      <div class="reviews__container">
        <div class="container">
          <h2 class="reviews__title section-title">베스트 합격 후기</h2>
        </div>

        <div class="lectures__content">
          <div class="lectures__slider_left lectures__slider">
            <img
              src="../assets/img/icon_arrow_black.svg"
              alt="arrow icon"
              class="slider__arrow_right"
            />
          </div>

          <div class="reviews__cards cards">
            <div class="reviews__card card">
              <picture class="review__img">
                <source
                  srcset="../assets/img/thumnail28.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail28.png" alt="thumbnail" />
              </picture>
              <div class="review__quote">
                <img src="../assets/img/icon__quote.svg" alt="quote icon" />
              </div>

              <h3 class="review__title">
                군무원 시험 끝장강좌로 마무리하세요~ 저처럼 다들 좋은 결과가
                있기를!
              </h3>
              <p class="review__description">
                덕분에 시험에 합격을 했네요~! 강사님께서 알려주신 내용으로
                무난하게 합격할 수 있었습니다!!! 여러분들도 좋은 결과가
                있으셨으면 합니…
              </p>
              <div class="review__author author">
                <span class="author__username">semodan195</span>
                <div class="author__circle"></div>
                <span class="author__date">2일 전</span>
              </div>
            </div>

            <div class="reviews__card card">
              <img src="../assets/img/thumnail29.png" alt="thumbnail" />
              <div class="review__quote">
                <img src="../assets/img/icon__quote.svg" alt="quote icon" />
              </div>
              <h3 class="review__title">GOOD! 개발자 클라스~!</h3>
              <p class="review__description">
                개발에 대해서 처음엔 어렵게 느껴졌지만 수업을 통해서 조금 더
                쉽게 다가간 것 같아 뿌듯합니다.
              </p>
              <div class="review__author author">
                <span class="author__username">studyrank</span>
                <div class="author__circle"></div>
                <span class="author__date">1일 전</span>
              </div>
            </div>

            <div class="reviews__card card">
              <picture class="review__img">
                <source
                  srcset="../assets/img/thumnail30.webp"
                  type="image/webp"
                />
                <img src="../assets/img/thumnail30.png" alt="thumbnail" />
              </picture>
              <div class="review__quote">
                <img src="../assets/img/icon__quote.svg" alt="quote icon" />
              </div>
              <h3 class="review__title">게으름을 잡고 재미있게 공부했어요!</h3>
              <p class="review__description">
                정말 공부시작하기 전에는 크게 마음먹었지만 막상 시작하니까
                나태함이 찾아오더라구요… 그러다가 이 수업을 듣고 저의 나태함이
                또 다…
              </p>
              <div class="review__author author">
                <span class="author__username">studybookmaster</span>
                <div class="author__circle"></div>
                <span class="author__date">1일 전</span>
              </div>
            </div>
          </div>

          <div class="lectures__slider_right lectures__slider">
            <img
              src="../assets/img/icon_arrow_black.svg"
              alt="arrow icon"
              class="slider__arrow_right"
            />
          </div>
        </div>
      </div>
    </section>
  </main>

  <footer class="footer">
    <div class="footer__container container">
      <div class="footer__upper">
        <div class="footer__column">
          <h3 class="footer__title">Center</h3>
          <ul class="footer__list">
            <li class="footer__list-item">
              <a href="#" class="footer__link">강의개설</a>
            </li>
            <li class="footer__list-item">
              <a href="#" class="footer__link">스튜디오</a>
            </li>
          </ul>
        </div>

        <div class="footer__column">
          <h3 class="footer__title">Policies</h3>
          <ul class="footer__list">
            <li class="footer__list-item">
              <a href="#" class="footer__link">개인정보처리방침</a>
            </li>
            <li class="footer__list-item">
              <a href="#" class="footer__link">이용약관</a>
            </li>
          </ul>
        </div>

        <div class="footer__column">
          <h3 class="footer__title">Support</h3>
          <ul class="footer__list">
            <li class="footer__list-item">
              <a href="#" class="footer__link">단체 수강 문의</a>
            </li>
            <li class="footer__list-item">
              <a href="#" class="footer__link">공지사항</a>
            </li>
            <li class="footer__list-item">
              <a href="#" class="footer__link">자주 묻는 질문</a>
            </li>
          </ul>
        </div>

        <div class="footer__column">
          <h3 class="footer__title">고객센터 1588-1565</h3>
          <ul class="footer__list">
            <li class="footer__list-item">
              <p class="footer__info">
                운영시간 평일 10:00 ~ 18:00 (토 · 일 공휴일 휴무)
              </p>
            </li>
            <li class="footer__list-item">
              <p class="footer__info">점심시간 평일 13:00 ~ 14:00</p>
            </li>
          </ul>
          <button class="footer__contact">클래온에 문의하기</button>
        </div>
      </div>

      <hr class="footer__hr" />

      <div class="footer__lower">
        <div class="footer__contacts">
          <p>
            <span>상호명 : (주)세모담</span>
            <span>대표 : 홍길동</span>
            <span>사업자등록번호 : 111-64-15765</span>
            <span>통신판매업신고 2022-서울강남-4563호</span>
          </p>
          <p>
            <span class="tel"
              >Tel : <a href="tel:02-555-5199">02-555-5199</a></span
            >
            <span class="fax"
              >Fax : <a href="fax:02-557-5199">02-557-5199</a></span
            >
            <span>
              <address>
                주소 : 서울특별시 강남구 강남대로 140길 46(논현동 25번지)
                G&A학동파크 1, 2층
              </address>
            </span>
          </p>
        </div>

        <ul class="footer__socials">
          <li class="footer__socials-item">
            <a
              href="#"
              class="footer__socials-link footer__socials-link_fb"
              target="_blank"
              aria-label="FaceBook Link"
            ></a>
          </li>
          <li class="footer__socials-item">
            <a
              href="#"
              class="footer__socials-link footer__socials-link_inst"
              target="_blank"
              aria-label="Instagram Link"
            ></a>
          </li>
          <li class="footer__socials-item">
            <a
              href="#"
              class="footer__socials-link footer__socials-link_yt"
              target="_blank"
              aria-label="YouTube Link"
            ></a>
          </li>
          <li class="footer__socials-item">
            <a
              href="#"
              class="footer__socials-link footer__socials-link_naver"
              target="_blank"
              aria-label="Naver Link"
            ></a>
          </li>
        </ul>
      </div>

      <p class="footer__copy">COPYRIGHT ⓒ 2022 CLAON. ALL RIGHTS RESERVED.</p>
    </div>
  </footer>
</template>

<script>
export default {};
</script>
